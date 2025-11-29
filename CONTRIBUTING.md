# Contributing to Doctype

Thank you for your interest in contributing to Doctype! We welcome contributions from the community and are grateful for your support.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Commit Guidelines](#commit-guidelines)

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title and description**
- **Steps to reproduce** the behavior
- **Expected behavior** vs actual behavior
- **Environment details** (OS, Node version, etc.)
- **Code samples** or error messages if applicable

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear and descriptive title**
- **Provide a detailed description** of the suggested enhancement
- **Explain why this enhancement would be useful**
- **Include examples** of how the feature would work

### Pull Requests

We actively welcome your pull requests:

1. Fork the repo and create your branch from `main`
2. If you've added code that should be tested, add tests
3. Ensure the test suite passes
4. Make sure your code lints
5. Update documentation as needed
6. Issue that pull request!

## Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/doctypedev/doctype.git
   cd doctype
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   - Copy `.env.example` to `.env` (if applicable)
   - Add your OpenAI API key if testing AI features

4. **Run tests**
   ```bash
   npm test
   ```

5. **Build the project**
   ```bash
   npm run build
   ```

## Pull Request Process

1. **Update documentation** - Ensure README.md and any relevant docs are updated
2. **Add tests** - New features should include appropriate test coverage
3. **Follow coding standards** - See below
4. **Update CHANGELOG** - Add a note about your changes
5. **One feature per PR** - Keep pull requests focused on a single concern
6. **Descriptive commits** - Write clear commit messages (see below)

### PR Checklist

- [ ] Code follows the project's coding standards
- [ ] Tests pass locally
- [ ] New tests added for new functionality
- [ ] Documentation updated
- [ ] No breaking changes (or clearly documented if necessary)
- [ ] Commit messages follow guidelines

## Coding Standards

### TypeScript

- Use **TypeScript** for all new code
- Enable strict mode
- Avoid `any` types when possible
- Use meaningful variable and function names
- Add JSDoc comments for public APIs

### Code Style

- **Indentation**: 2 spaces
- **Quotes**: Single quotes for strings
- **Semicolons**: Required
- **Line length**: Maximum 100 characters when practical
- **Naming conventions**:
  - `camelCase` for variables and functions
  - `PascalCase` for classes and types
  - `UPPER_CASE` for constants

### Testing

- Write unit tests for new features
- Maintain test coverage above 80%
- Use descriptive test names
- Follow AAA pattern (Arrange, Act, Assert)

## Commit Guidelines

We follow conventional commits for clear history:

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting, etc.)
- **refactor**: Code refactoring
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```
feat(parser): add support for JSDoc comments

Implement JSDoc parsing to extract documentation
from TypeScript source files.

Closes #123
```

```
fix(git): resolve auto-commit race condition

Ensure git operations are properly queued to prevent
concurrent modifications.
```

## Questions?

Feel free to open an issue with the `question` label, or reach out to the maintainers.

Thank you for contributing to Doctype!
