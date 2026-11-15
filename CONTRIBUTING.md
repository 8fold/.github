<!--
Maintained and synced from 8fold/.github, do not update outside of the 8fold/.github repository
-->

# Contributing

Contributions are **welcome** and will be **credited**. We accept contributions via pull requests to the GitHub project repository.

---

## Discussions & Submitting Issues

We use GitHub Discussions and Issues to manage project updates, triage bugs, and plan new capabilities.

* **Discussions**: Use Discussions for open-ended questions, design proposals, or architectural ideas before opening a formal issue.
* **Submitting Issues**: When reporting a bug or requesting a feature, describe objective system states and behaviors rather than assigning fault or making assumptions.
* **Prioritization & Triage**: We leverage GitHub's labeling system to prioritize issues. Security and accessibility are always the highest priority within the applicable scope of the project.

---

## Commit & PR Discipline

Pull requests must maintain clear history, strict commit separation, and full template compliance:

* **Single-Classification Commits**: A single commit should either be Refactoring or Re-engineering changes, not both.
* **Conventional Commits Syntax**:
  * `refactor:` Internal restructuring without behavior changes (**Refactoring**).
  * `feat:`, `fix:`, `perf:` Observable capabilities or contract updates (**Re-engineering**).
  * `docs:`, `test:`, `chore:` Maintenance, verification, or documentation.
  * `BREAKING CHANGE:` Include in the footer for breaking contract updates.
* **PR Template Compliance**: Inspect the pull request template (`PULL_REQUEST_TEMPLATE.md`), complete all required sections, and classify each meaningful change in the PR body.

---

## Code Quality & Engineering Principles

Our codebases adhere to strict architectural governance, foundational design principles, and minimal API surface areas:

* **YAGNI (You Ain't Gonna Need It)**: Do not build features until they are explicitly required and requested. Avoid speculative abstractions.
* **Single Responsibility Principle**: Each class or component should have one reason to change.
* **Interface Segregation Principle**: Prefer focused, client-specific interfaces over generic catch-all interfaces.
* **Dependency Inversion Principle**: Depend upon abstractions, not concrete implementations.
* **The Community Principle**: If you create or acquire code or dependencies, you help maintain them.
* **Code Promotion**: Capabilities must be implemented at a low, concrete level before being promoted to higher, more abstract levels.
* **Code Access & Visibility**: Access levels (variables, constants, methods) MUST begin at the most strict setting (`private`) and become less restrictive only out of functional necessity. (Creating unit tests does not constitute a necessity.) This minimizes the public API surface area and makes classes easier to consume.