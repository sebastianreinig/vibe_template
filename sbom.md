# Software Bill of Materials (SBOM)

> [!NOTE]
> This document tracks all dependencies and their licenses used in this project. Update this file whenever dependencies change.

## Overview

| Category | Count | Last Updated |
|----------|-------|--------------|
| Frontend Dependencies | 0 | 2024-12-24 |
| Backend Dependencies | 0 | 2024-12-24 |
| Development Tools | 0 | 2024-12-24 |

---

## Frontend Dependencies

| Package | Version | License | Purpose |
|---------|---------|---------|---------|
| *No dependencies yet* | - | - | - |

### Frontend Dev Dependencies

| Package | Version | License | Purpose |
|---------|---------|---------|---------|
| *No dependencies yet* | - | - | - |

---

## Backend Dependencies

| Package | Version | License | Purpose |
|---------|---------|---------|---------|
| *No dependencies yet* | - | - | - |

### Backend Dev Dependencies

| Package | Version | License | Purpose |
|---------|---------|---------|---------|
| *No dependencies yet* | - | - | - |

---

## Development Tools

| Tool | Version | License | Purpose |
|------|---------|---------|---------|
| Docker | Latest | Apache-2.0 | Containerization |
| VS Code | Latest | MIT | IDE |

---

## License Summary

| License | Count | Packages |
|---------|-------|----------|
| MIT | 0 | - |
| Apache-2.0 | 1 | Docker |
| ISC | 0 | - |
| BSD-3-Clause | 0 | - |

---

## Update History

| Date | Change | Packages Affected |
|------|--------|-------------------|
| 2024-12-24 | Initial SBOM creation | - |

---

## How to Update

When adding or updating dependencies:

1. **Add new dependency**: Add a row to the appropriate table
2. **Update version**: Update the version column
3. **Check license**: Verify the license is compatible
4. **Update counts**: Update the overview table counts
5. **Log change**: Add an entry to Update History

### Generating SBOM Automatically

For Node.js projects:
```bash
npx license-checker --json > licenses.json
```

For Python projects:
```bash
pip-licenses --format=markdown > licenses.md
```
