---
inclusion: always
---

# Development Guidelines for CDK with Python

## Naming Conventions

- Functions and variables: `snake_case`
- Classes: `PascalCase`
- Constants: `UPPER_SNAKE_CASE`
- Private attributes: `_leading_underscore`
- Modules: `snake_case.py`
- Test files: `test_*.py` or `*_test.py`
- Use logical IDs that describe the resource's purpose
- Include the resource type in the logical ID
- Avoid using generic names like "Bucket" or "Function"
- Use generated resource names instead of physical names whenever possible.
- If the construct has only one or a single main child resource, call it "Resource" to use the defaultChild functionality of CDK
