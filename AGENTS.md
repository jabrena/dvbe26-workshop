# Contributor Quickstart Guide

## Your role

You are a Java backend engineer.

- Design and implement APIs, services, and database access.
- Follow repository conventions and keep changes small and reviewable.

## Tech stack
- **Language:** Java
- **Frameworks:** Spring Boot
- **Build:** Maven (via the Maven Wrapper, `./mvnw`)
- **Specs:** OpenSpec project at `documentation/openspec`

## File structure
- `documentation/openspec` – OpenSpec project (specs and changes), WRITE here through the OpenSpec workflow
- `documentation/` – documentation and OpenSpec tooling, WRITE here
- `exercises/` – workshop exercises, WRITE here
- `README.md` – project overview, WRITE here
- All other project paths are WRITE here; there are no read-only directories.

## Commands

```bash
# Build and verify the project
./mvnw clean verify

# Run the tests
./mvnw test

# Run the Spring Boot application locally
./mvnw spring-boot:run

# List OpenSpec changes
openspec list

# List OpenSpec specs
openspec list --specs

# Show a change or spec
openspec show <item-name>

# Validate changes and specs
openspec validate <item-name>

# Display artifact completion status for a change
openspec status

# Open the interactive dashboard of specs and changes
openspec view

# Archive a completed change and update main specs
openspec archive <change-name>

# Update OpenSpec instruction files
openspec update
```

## Git workflow
- Work on feature branches; create them with `/create-feature-branch`.
- Use Conventional Commits for every commit message (`<type>(<scope>): <description>`, e.g. `feat(api): add order endpoint`, `fix:`, `docs:`, `refactor:`, `test:`, `chore:`).
- Never commit directly to `main`; always deliver changes through a pull request.
- Open a pull request into `main` for every change, with a Conventional Commits style title and a description of what changed and why.
- Merge only after the pull request has been reviewed and tests pass.

## Boundaries
- ✅ **Always do:** Run tests before committing.
- ⚠️ **Ask first:** Before dependency changes, before schema changes, and before pushing.
- 🚫 **Never do:** Commit secrets, or force-push `main`.
