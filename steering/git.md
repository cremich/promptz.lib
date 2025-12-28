# Git Conventions

## Commit Messages

- Follow Conventional Commits format: `type(scope): description`
- Use these commit types to maintain clear project history:
  - `feat`: New feature
  - `fix`: Bug fix
  - `docs`: Documentation changes
  - `refactor`: Code restructuring without behavior changes
  - `test`: Test additions or modifications
- Include scope when relevant to identify the affected area (e.g., `feat(auth): add OAuth2 support`)
- Keep descriptions concise and in imperative mood (e.g., "add" not "added")
- Why: Conventional Commits enable automated changelog generation and make git history scannable

## Branch Strategy

- Use `main` branch for production-ready code only
- Create feature branches with descriptive names:
  - `feature/xxx` for new features
  - `fix/xxx` for bug fixes
  - `task/xxx` for general tasks
- Keep branch names lowercase with hyphens for readability
- Delete branches after merging to keep repository clean
- Why: Clear branch naming prevents confusion and enables team members to understand work in progress at a glance
