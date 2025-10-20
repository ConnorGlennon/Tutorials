# Conventional Commits

Conventional commits offer a standardised format for commit messages where the conventions are both human and machine-readable.

Some benefits include:

- automatic changelog generation
- easier semantic versioning (SemVer)
- easier to understand project history

**The format**: `<type>(<scope>): <description>`
**Example**: `feat(auth): add JWT token refresh logic`

Table of standard `<type>` values:

| Type         | Meaning                                                       |
| ------------ | ------------------------------------------------------------- |
| **feat**     | A new feature                                                 |
| **fix**      | A bug fix                                                     |
| **docs**     | Documentation changes only                                    |
| **style**    | Code style / formatting changes (no logic changes)            |
| **refactor** | Code refactoring that doesn’t fix a bug or add a feature      |
| **perf**     | Performance improvement                                       |
| **test**     | Adding or fixing tests                                        |
| **build**    | Changes to build system, dependencies, or package managers    |
| **ci**       | CI/CD or automation configuration changes                     |
| **chore**    | Maintenance tasks (e.g., renaming files, updating .gitignore) |
| **revert**   | Revert a previous commit                                      |

Some optional parts:

| Part       | Description                                                                     |
| ---------- | ------------------------------------------------------------------------------- |
| **scope**  | What area/module the change affects (e.g. `ui`, `backend`, `schemas`)           |
| **!**      | Breaking change indicator (e.g. `feat!: remove legacy API`)                     |
| **body**   | (After a blank line) Explains *why* the change was made                         |
| **footer** | References issues or breaking changes (e.g. `BREAKING CHANGE:` or `Closes #42`) |
