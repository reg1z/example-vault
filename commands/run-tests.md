---
name: run-tests
description: Run the test suite and generate coverage reports
---

# Test Execution Command

## Overview
Execute the complete test suite with coverage reporting and formatted output.

## Command Options

- `--unit` - Run only unit tests
- `--integration` - Run only integration tests
- `--coverage` - Generate coverage report
- `--watch` - Watch mode for continuous testing
- `--parallel` - Run tests in parallel
- `--verbose` - Detailed output for each test

## Execution

```bash
npm test           # Run all tests
npm test -- unit   # Run unit tests only
npm test -- --cov  # With coverage
```

## Expected Output

- Test results summary (passed/failed/skipped)
- Coverage percentage by file/folder
- Failed test details with stack traces
- Execution time

## Coverage Thresholds

- Line coverage: 80%
- Branch coverage: 75%
- Function coverage: 80%
- Statement coverage: 80%

## Common Issues

**Tests timeout**: Increase timeout in jest config
**Import errors**: Check module resolution setup
**Coverage gaps**: Review untested code paths

## Integration with CI/CD

This command runs automatically on:
- Pull request creation
- Merge to main branch
- Pre-deployment validation
