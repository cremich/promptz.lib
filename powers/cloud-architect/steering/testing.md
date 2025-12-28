---
inclusion: always
---

# Testing Strategy

The testing strategy is built upon the **remocal testing** concept, combining the speed of local execution with the confidence of real AWS service integration. This approach enables effective TDD while maintaining high confidence in our serverless infrastructure.

## Testing Pyramid

1. **Unit Tests** (`tests/unit/`): Pure business logic with mocks
   - Fast execution (<1s)
   - Test individual functions and classes

2. **Integration Tests** (`tests/integration/`): AWS Services such as lambda functions that integrate with other AWS services
   - Execute Lambda code locally (1-5s)
   - Connect to real DynamoDB, S3, SNS, etc.
   - Enable full debugging with breakpoints
   - Test AWS service integrations without deployment
