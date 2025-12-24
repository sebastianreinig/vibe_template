---
description: Update the changelog and SBOM after making changes to the project
---

# Update Changelog Workflow

Follow these steps to properly document changes in the changelog and update the SBOM.

## Prerequisites
- Changes have been made to the codebase
- You understand what category the changes fall into (see `rules/changelog-tracking.md`)

## Steps

### 1. Determine Version Bump Type

Analyze the changes and determine the version bump:

| Change Type | Version Bump | Example |
|-------------|--------------|---------|
| Breaking changes | MAJOR (X.0.0) | Removed API endpoint |
| New features | MINOR (0.X.0) | Added new page |
| Bug fixes | PATCH (0.0.X) | Fixed login bug |

### 2. Read Current Changelog

Read the current `changelog.md` to understand the current version and format:

```
View file: changelog.md
```

### 3. Add New Entry

Add a new entry at the TOP of the changelog (under the header), following this format:

```markdown
## [X.Y.Z] - YYYY-MM-DD

### Category
- Description of change with relevant details
```

Categories (use only applicable ones):
- **Added** - New features
- **Changed** - Changes in existing functionality
- **Deprecated** - Soon-to-be removed features
- **Removed** - Removed features
- **Fixed** - Bug fixes
- **Security** - Security patches

### 4. Update SBOM (if dependencies changed)

If any dependencies were added, updated, or removed:

1. Read current `sbom.md`
2. Update the dependencies table
3. Note any license changes

For each dependency, document:
- Package name
- Version
- License
- Purpose/Usage

### 5. Verify Changes

Review your changelog entry:
- [ ] Version number is correct
- [ ] Date is today's date
- [ ] Category is appropriate
- [ ] Description is clear and complete
- [ ] No typos or formatting issues

### 6. Summary

After completing the update, summarize:
- Previous version → New version
- Number of changes per category
- Any breaking changes or migration notes

## Example

Before:
```markdown
## [1.2.0] - 2024-01-15
### Added
- User profile page
```

After adding a bug fix:
```markdown
## [1.2.1] - 2024-01-20
### Fixed
- Resolved crash when uploading large profile images (>5MB)

## [1.2.0] - 2024-01-15
### Added
- User profile page
```
