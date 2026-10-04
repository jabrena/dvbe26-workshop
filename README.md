# Technical Workshop on AI-Native Tooling for Java Development 

https://m.devoxx.com/events/dvbe26/talks/8190/technical-workshop-on-ainative-tooling-for-java-development

## Start in 60 seconds

Install every skill for your preferred agent. Execute the command in a terminal:

```bash
npx skills add jabrena/plinth --skill '*' --agent cursor -y
npx skills add jabrena/plinth --skill '*' --agent claude-code -y
npx skills add jabrena/plinth --skill '*' --agent codex -y
```

Install every command for your prefered agent. Execute the command in your prefered agent:

```bash
install @004-commands-installation cursor
install @004-commands-installation claude-code
install @004-commands-installation codex
```

Install every agent for your prefered agent. Execute the command in your prefered agent:

```text
install @005-agents-installation cursor
install @005-agents-installation claude-code
install @005-agents-installation codex
```

### See it in action

You can use the project in 2 ways:

- Use the AI-Native development workflow
- Refactor your code with Skills

## Using the AI-Native development workflow

Prepare the repository with `/onboarding`, then identify an issue in your `Kanban` dashboard from `Atlasian Jira`, `Github Issues` or `Azure DevOps` and apply the following workflow:

```text
/onboarding
  |
  v
Issue
  |
  v
/update-issue --> /explore-problem --> /create-acceptance-criteria
  |
  v
/create-spec --> /explore-design
  |
  v
/implement-spec --> /close-spec
```

`/onboarding` establishes root `AGENTS.md` and one unambiguous OpenSpec project before issue selection. It preserves existing prerequisites; when OpenSpec is missing, you select its result path with `documentation/openspec` as the default.

##### Analysis & Design

Turn an idea into an actionable change with user stories, GitHub Issues or Jira, ADRs, diagrams, AI plan mode, and OpenSpec.

**Functional Specification:**

<table>
  <thead>
    <tr>
      <th>Command</th>
      <th>Explanation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>/onboarding</code></td>
      <td>Establish root repository guidance and one unambiguous OpenSpec project before issue work.</td>
    </tr>
    <tr>
      <td><code>/update-issue</code></td>
      <td>Update an existing GitHub or Jira issue with a structured user story, acceptance criteria, and resource content.</td>
    </tr>
    <tr>
      <td><code>/explore-problem</code></td>
      <td>Evaluate an issue from five perspectives and post a Functional Specification comment on the issue.</td>
    </tr>
    <tr>
      <td><code>/create-acceptance-criteria</code></td>
      <td>Derive Gherkin acceptance criteria from a Functional Specification and post them as a separate issue comment.</td>
    </tr>
  </tbody>
</table>

**Technical Specification:**

<table>
  <thead>
    <tr>
      <th>Command</th>
      <th>Explanation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>/create-adr</code> (Optional)</td>
      <td>Record an architectural decision, its alternatives, rationale, and consequences.</td>
    </tr>
    <tr>
      <td><code>/create-diagram</code> (Optional)</td>
      <td>Create a focused architecture or design diagram from approved artifacts.</td>
    </tr>
    <tr>
      <td><code>/create-spec</code> (OpenSpec)</td>
      <td>Create or update one or more validated OpenSpec changes.</td>
    </tr>
    <tr>
      <td><code>/explore-design</code></td>
      <td>Compare technical approaches and obtain an approved design direction.</td>
    </tr>
  </tbody>
</table>

##### Build

Implement and improve Java applications with Maven, design, coding, testing, security, documentation, Spring Boot, Quarkus, Micronaut, OpenAPI, and WireMock guidance.

<table>
  <thead>
    <tr>
      <th>Command</th>
      <th>Explanation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>/implement-spec</code></td>
      <td>Deliver an approved plan or validated OpenSpec task list through framework-aware delegation.</td>
    </tr>
    <tr>
      <td><code>/close-spec</code></td>
      <td>Archive an OpenSpec change by name using the OpenSpec CLI.</td>
    </tr>
  </tbody>
</table>

## Agenda

- Questionary
- Introduction to AI-Native Tooling
- 5 min break
- Example 1: REST API Development
- 10 min break
- Example 2: Database Development
- 10 min break
- Advanced topics
- Questions and Answers

## Prerrequisites

- Laptop
- IA tool like Claude Code, Cursor, Codex, Github Copilot
- Git
- SDKMAN installed
- Java 25 installed
- Maven 3.9.14 installed
- IDE like Intellij, VSCode or similar

## References

- https://github.com/jabrena/latency-problems
- https://github.com/jabrena/plinth