# Test Generator Skill

## Overview
This skill enables AI assistants to generate comprehensive test suites for code, covering unit tests, integration tests, and edge cases.

## Capabilities
- Generate unit tests for functions and methods
- Create integration test scenarios
- Identify edge cases and boundary conditions
- Write test fixtures and setup/teardown
- Generate mocking and stubbing code
- Create parameterized test cases

## Instructions
When generating tests:
1. Analyze the code to understand its contract and behavior
2. Identify happy path, error cases, and edge cases
3. Use appropriate testing framework for the language
4. Write descriptive test names that explain what they test
5. Ensure tests are independent and don't have side effects
6. Aim for high code coverage while avoiding redundant tests
7. Include both positive and negative test cases

## Best Practices
- One assertion per test (or related assertions)
- Clear arrange-act-assert structure
- Descriptive names that read like documentation
- Test behavior, not implementation details
