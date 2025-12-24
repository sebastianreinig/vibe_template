# Changelog Tracking Rule

> [!IMPORTANT]
> This rule defines how to maintain the project changelog. All changes MUST be documented according to these guidelines.

## Overview

The changelog follows [Keep a Changelog](https://keepachangelog.com/) format with semantic versioning. Every meaningful change to the codebase should be recorded.

## Version Types

### MAJOR Version (X.0.0)
Increment when making **breaking changes**:
- Removing or renaming public APIs
- Changing function signatures in breaking ways
- Removing features
- Major architectural changes that affect integrations
- Database schema changes requiring migrations with data loss

### MINOR Version (0.X.0)
Increment when adding **new functionality** in a backward-compatible manner:
- New features
- New API endpoints
- New UI components or pages
- New configuration options
- Non-breaking database additions

### PATCH Version (0.0.X)
Increment for **backward-compatible bug fixes**:
- Bug fixes
- Performance improvements
- Documentation updates
- Refactoring without behavior changes
- Security patches

## Change Categories

Always use these exact category headers in this order:

### Added
New features, APIs, components, or capabilities.
```markdown
### Added
- New user authentication system with OAuth2 support
- Dashboard widget for real-time analytics
- API endpoint `GET /api/v2/users/{id}/preferences`
```

### Changed
Modifications to existing functionality.
```markdown
### Changed
- Updated login form to use new design system
- Improved database query performance for user lookups (3x faster)
- Refactored authentication middleware for better error handling
```

### Deprecated
Features that will be removed in future versions.
```markdown
### Deprecated
- `GET /api/v1/users` - Use `GET /api/v2/users` instead
- `legacyConfig` option in config.js - Will be removed in v3.0
```

### Removed
Features or code that has been removed.
```markdown
### Removed
- Legacy authentication endpoints (`/auth/legacy/*`)
- Unused CSS utility classes
- Support for Node.js 14
```

### Fixed
Bug fixes.
```markdown
### Fixed
- Resolved issue where login failed after password reset (#123)
- Fixed memory leak in WebSocket connection handler
- Corrected timezone handling in date picker component
```

### Security
Security-related changes. **Always include CVE if applicable.**
```markdown
### Security
- Updated dependencies to patch CVE-2024-XXXXX
- Fixed XSS vulnerability in comment submission
- Added rate limiting to prevent brute force attacks
```

## Entry Format

### Required Elements
Each entry MUST include:
1. **Action verb** - What was done (Added, Fixed, Changed, etc.)
2. **Component/Area** - Where the change was made
3. **Description** - What specifically changed
4. **Impact** - How it affects users (if applicable)

### Good Examples ✅
```markdown
- Added dark mode toggle to user settings with system preference detection
- Fixed pagination bug in user list that caused duplicate entries on page 2
- Changed password requirements: minimum 12 characters, must include number
- Removed deprecated `v1/legacy` API endpoints (see migration guide in docs)
```

### Bad Examples ❌
```markdown
- Fixed bug          # Too vague
- Updated stuff      # No description
- Changes            # Not actionable
- Did some work      # Meaningless
```

## Detailed Change Documentation

For significant changes, include additional context:

```markdown
### Changed
- **Authentication System Overhaul**
  - Migrated from session-based to JWT authentication
  - Added refresh token rotation for enhanced security
  - Updated all API endpoints to use Bearer token
  - **Breaking:** Existing sessions will be invalidated
  - **Migration:** Run `npm run migrate:auth` before deploying
```

## When to Update

Update the changelog when:
- ✅ Adding new features
- ✅ Fixing bugs
- ✅ Making breaking changes
- ✅ Deprecating functionality
- ✅ Security patches
- ✅ Significant performance improvements

Do NOT update for:
- ❌ Minor code formatting
- ❌ Comment changes
- ❌ Internal refactoring with no behavior change
- ❌ Test-only changes (unless fixing broken tests)

## File Location

The changelog MUST be maintained at:
- `changelog.md` (root directory)

## SBOM Updates

When dependencies change, also update `sbom.md`:
- New dependencies
- Updated dependencies
- Removed dependencies
- License changes
