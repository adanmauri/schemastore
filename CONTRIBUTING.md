# Contributing to Schema Store Repository

[![ColPrac: Contributor's Guide on Collaborative Practices for Community Packages](https://img.shields.io/badge/ColPrac-Contributor's%20Guide-blueviolet)](https://github.com/SciML/ColPrac)

We follow the [ColPrac Guide](https://github.com/SciML/ColPrac) for collaborative practices. Please review it before contributing. Below are additional practices specific to this repository.

---

## 📜 Reporting Issues

- **Search First**: Check existing issues for similar reports or context before creating a new one.
- **Be Specific**: Provide minimal reproducible examples or detailed descriptions.

---

## 🚀 Contributing Guidelines

### Getting Started
- Fork the repository and create a feature branch:
  ```bash
  git checkout -b feature/new-schema
  ```
- Make changes relevant to the project, keeping commits atomic and descriptive.

### Submitting Pull Requests
- Open PRs against the `main` branch.
- Avoid working on your fork's `main` branch; use a feature branch instead.
- Rebase your branch on the latest `main` to resolve conflicts:
  ```bash
  git fetch origin
  git rebase origin/main
  ```
- Use `[BREAKING]` in PR titles for breaking changes.
- If your PR is a work in progress, mark it as a draft.

### Best Practices
- **Formatting**: Adhere to JSON and YAML linting standards.
- **Descriptive Commits**: Clearly explain changes in commit messages.
- **CI Efficiency**: Avoid pushing excessive small commits to minimize CI job queueing.
- **Scope**: Limit unrelated changes in a single PR.

---

## 🔧 Development Workflow

- **Schema Development**: Ensure new schemas are complete, documented, and validate correctly.
- **Testing**: Use tools like [AJV](https://ajv.js.org/) for JSON and [YAML Lint](https://yaml-lint.com/) to validate schemas.

---

## 🗂 Folder Structure

- `json/`: JSON schemas.
- `yaml/`: YAML schemas.
- Add new schemas in the appropriate directory.

---

## 🌟 Tips for First-Time Contributors

- Unsure where to start? Open an issue, and we’ll guide you toward a suitable first contribution.
- Start with improving documentation or adding tests.

---

## 🢞 Community Standards

- Be respectful and constructive in all interactions.
- Follow the repository’s code of conduct (coming soon).

Thank you for contributing to the Schema Store Repository! Your efforts help simplify development workflows and improve best practices.

