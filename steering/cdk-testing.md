# CDK Testing

# CDK Testing Rules

## General

- Follow a test-driven development approach.
- Keep tests simple and focused on one aspect of behavior
- Use Jest as the testing framework
- Use the AWS CDK assertions module for testing CDK constructs
- Use the Arrange-Act-Assert pattern
- Organize tests by construct or stack
- Use descriptive test names that explain the expected behavior
- Aim for high test coverage (at least 80%)
- Focus on testing critical infrastructure components
- Ensure all resource properties are tested

## Unit Tests

- Use fine-grained assertions to test specific aspects of resources
- Use `hasResourceProperties` for partial matching and `exactlyMatchTemplate` for exact matching
- Use snapshot testing to detect unintended changes in CloudFormation templates
- Update snapshots only when changes are intentional
- Don't rely solely on snapshots; combine with fine-grained assertions

## Integration Tests

- Use the `integ-tests-alpha` module for integration testing
- Create separate integration test files with the `.integ.ts` suffix
- Define integration tests as CDK applications
- Test that resources are created successfully
- Test interactions between resources
- Clean up resources after tests complete
