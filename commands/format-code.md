---
description: Format codebase according to project style guide
tags: [formatting, linting, code-style]
category: Development
---

# Code Formatting Command

## Overview
Automatically format code to match the project's style guide using standardized tooling.

## Tools Used

- **Prettier**: JavaScript, TypeScript, JSON, CSS, Markdown
- **Black**: Python
- **Go fmt**: Go language
- **Eslint --fix**: Additional linting fixes

## Execution

```bash
npm run format      # Format all supported files
npm run format:check # Check formatting without changes
npm run lint:fix    # Apply linting fixes
```

## Scope

Formats files in:
- `src/**/*` - Source code
- `tests/**/*` - Test files
- `*.config.js` - Configuration files
- `*.md` - Documentation

Excludes:
- `node_modules/`
- `.dist/`
- `build/`
- Generated files

## Configuration

Formatting rules are defined in:
- `.prettierrc` - Prettier configuration
- `.eslintrc.js` - ESLint rules
- `pyproject.toml` - Python formatting

## Pre-commit Integration

This command runs automatically before commits via Git hooks to ensure consistent formatting.

## IDE Integration

Most IDEs can be configured to run formatting on save. See project README for IDE setup instructions.
