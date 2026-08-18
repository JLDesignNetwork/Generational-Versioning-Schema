# JLDN Generational Versioning Schema Usage & Integration

> **Document:** `docs/usage.md`  
> **Author:** Jeff Langdon (JL Design Network)  

---

## 1. Automated CI/CD Validation Snippets

### Bash / Shell Validation
```bash
GVS_REGEX='^([0-9]{2}(0[1-9]|1[0-2]))\.([0-9]+)\.([0-9]+)-(a|as|b|bs|l|s|ts|z)$'
VERSION="2607.2.0-s"

if [[ $VERSION =~ $GVS_REGEX ]]; then
    echo "✅ Valid GVS Version: $VERSION"
else
    echo "❌ Invalid GVS Version: $VERSION" >&2
    exit 1
fi
```

### Python 3 Validation
```python
import re

GVS_PATTERN = re.compile(r'^(\d{2}(?:0[1-9]|1[0-2]))\.(\d+)\.(\d+)-(a|as|b|bs|l|s|ts|z)$')

def is_valid_gvs(version_str: str) -> bool:
    return bool(GVS_PATTERN.match(version_str))

assert is_valid_gvs("2607.2.0-s") == True
assert is_valid_gvs("2607.2.0-invalid") == False
```

### PHP 8.4+ Validation
```php
declare(strict_types=1);

function isValidGvs(string $version): bool
{
    $pattern = '/^(\d{2}(?:0[1-9]|1[0-2]))\.(\d+)\.(\d+)-(a|as|b|bs|l|s|ts|z)$/';
    return (bool) preg_match($pattern, $version);
}
```

---

## 2. Changelog Guidelines

Structure project changelogs adhering to "Keep a Changelog" grouped by Generational Epoch:

```markdown
# Changelog

## [2607.2.0-s] - 2026-08-18

### Added
- Feature details...

### Fixed
- Bug fixes...
```
