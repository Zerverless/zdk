# Contributing

Thank you for your interest in contributing. We welcome contributions from the community — bug fixes, improvements, documentation, and new ideas are all appreciated.

---

## Before You Start

- Check existing [issues](../../issues) and [pull requests](../../pulls) to avoid duplicating work
- For significant changes, open an issue first to discuss what you'd like to change
- All contributions must align with the project's scope and design principles

---

## Development Setup

1. Fork the repository and clone your fork
2. Install dependencies:
   ```bash
   npm install
   ```
3. Make your changes in a new branch:
   ```bash
   git checkout -b feat/your-feature-name
   ```
4. Run tests before submitting:
   ```bash
   npm run test
   npm run lint
   ```

---

## Branch Naming

| Type | Pattern | Example |
|------|---------|---------|
| Feature | `feat/description` | `feat/serverless-queue` |
| Bug fix | `fix/description` | `fix/lambda-timeout` |
| Docs | `docs/description` | `docs/api-reference` |
| Chore | `chore/description` | `chore/update-deps` |

---

## Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add ServerlessQueue construct
fix: correct IAM policy for S3 bucket
docs: update ServerlessApi usage example
chore: bump aws-cdk-lib to 2.100.0
```

---

## Pull Request Guidelines

- Keep PRs focused — one feature or fix per PR
- Include a clear description of what changed and why
- Reference any related issues (`Closes #123`)
- All tests must pass
- New features must include tests
- Public APIs must include JSDoc

---

## Code Standards

- **Language:** TypeScript (strict mode)
- **Formatting:** Prettier (run `npm run lint` before committing)
- **Testing:** Jest — every construct and command must have unit tests
- **No wildcard IAM permissions** — ever
- **Production-grade defaults** — every new construct must be safe to use in production out of the box

---

## Reporting Issues

Use the issue templates provided:
- [Bug report](../../issues/new?template=bug_report.md)
- [Feature request](../../issues/new?template=feature_request.md)

---

## License

By contributing, you agree that your contributions will be licensed under the [Apache 2.0 License](./LICENSE).
