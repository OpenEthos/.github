# Contributing to OpenEthos

Thank you for your interest in contributing to OpenEthos! We welcome contributions from everyone and are grateful for even the smallest of improvements.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Development Workflow](#development-workflow)
- [Coding Standards](#coding-standards)
- [Testing](#testing)
- [Documentation](#documentation)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before contributing.

## Getting Started

### Prerequisites

- Python 3.9 or higher
- Git
- A GitHub account
- Familiarity with Git workflows

### Setting Up Your Development Environment

1. **Fork the repository** on GitHub

2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/REPOSITORY_NAME.git
   cd REPOSITORY_NAME
   ```

3. **Add the upstream repository**:
   ```bash
   git remote add upstream https://github.com/OpenEthos/REPOSITORY_NAME.git
   ```

4. **Create a virtual environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

5. **Install dependencies**:
   ```bash
   pip install -e ".[dev]"
   # or
   pip install -r requirements-dev.txt
   ```

6. **Install pre-commit hooks**:
   ```bash
   pre-commit install
   ```

## How to Contribute

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include:

- Clear and descriptive title
- Detailed description of the issue
- Steps to reproduce the behavior
- Expected vs actual behavior
- Environment details (OS, Python version, package version)
- Relevant logs, error messages, or screenshots

Use our [Bug Report Template](.github/ISSUE_TEMPLATE/bug_report.yml).

### Suggesting Enhancements

We welcome feature requests and enhancement suggestions! Please:

- Check if the enhancement has already been suggested
- Provide a clear and detailed explanation
- Explain why this enhancement would be useful
- Include examples of how it would work

Use our [Feature Request Template](.github/ISSUE_TEMPLATE/feature_request.yml).

### Your First Contribution

Unsure where to begin? Look for issues labeled:

- `good first issue` - Good for newcomers
- `help wanted` - Extra attention is needed
- `documentation` - Improvements or additions to documentation

## Development Workflow

### Branching Strategy

We use Git Flow:

- `main` - Production-ready code
- `develop` - Integration branch for features
- `feature/*` - New features
- `bugfix/*` - Bug fixes
- `hotfix/*` - Urgent production fixes

### Creating a Branch

```bash
git checkout develop
git pull upstream develop
git checkout -b feature/your-feature-name
```

### Making Changes

1. **Make your changes** in your feature branch
2. **Write or update tests** for your changes
3. **Update documentation** if needed
4. **Run tests and linters** locally
5. **Commit your changes** with clear commit messages

### Commit Message Guidelines

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types**:
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks
- `security`: Security improvements

**Examples**:
```
feat(auth): add multi-factor authentication support

Implements MFA using TOTP for enhanced security.

Closes #123
```

```
fix(parser): handle edge case in rule validation

Fixes issue where certain regex patterns would cause validation to fail.

Fixes #456
```

## Coding Standards

### Python Style Guide

We follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) with some modifications:

- Maximum line length: 100 characters (docstrings: 72)
- Use type hints for function signatures
- Use docstrings for all public modules, functions, classes, and methods

### Code Quality Tools

We use the following tools (configured in `pyproject.toml`):

- **Black**: Code formatting
- **isort**: Import sorting
- **flake8**: Linting
- **pylint**: Additional linting
- **mypy**: Type checking
- **bandit**: Security checks

Run all checks:
```bash
# Format code
black .
isort .

# Lint
flake8 .
pylint src/

# Type check
mypy src/

# Security scan
bandit -r src/
```

### Security Considerations

- Never commit secrets, API keys, or credentials
- Run security scans before submitting PRs
- Follow the principle of least privilege
- Validate and sanitize all inputs
- Use parameterized queries for database operations
- Keep dependencies up to date

## Testing

### Writing Tests

- Write tests for all new features and bug fixes
- Use pytest for testing
- Aim for high test coverage (>80%)
- Write both unit tests and integration tests
- Test edge cases and error conditions

### Running Tests

```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=src --cov-report=html

# Run specific test file
pytest tests/test_module.py

# Run specific test
pytest tests/test_module.py::test_function
```

### Test Organization

```
tests/
├── unit/           # Unit tests
├── integration/    # Integration tests
├── fixtures/       # Test fixtures
└── conftest.py     # Pytest configuration
```

## Documentation

### Documentation Requirements

- Update README.md if needed
- Add docstrings to all public APIs
- Update relevant documentation files
- Include examples for new features
- Update CHANGELOG.md

### Docstring Format

We use Google-style docstrings:

```python
def function_with_types(param1: int, param2: str) -> bool:
    """Summary line.

    Extended description of function.

    Args:
        param1: Description of param1
        param2: Description of param2

    Returns:
        Description of return value

    Raises:
        ValueError: When param1 is negative
    """
    pass
```

## Pull Request Process

### Before Submitting

- [ ] Tests pass locally
- [ ] Code is formatted and linted
- [ ] Documentation is updated
- [ ] Commit messages follow conventions
- [ ] Changes are rebased on latest develop

### Submitting a Pull Request

1. **Push your branch** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request** on GitHub:
   - Use a clear and descriptive title
   - Fill out the PR template completely
   - Link related issues
   - Request review from maintainers

3. **Respond to feedback**:
   - Address all review comments
   - Make requested changes
   - Push updates to your branch
   - Re-request review when ready

### PR Review Process

- Maintainers will review your PR
- CI/CD checks must pass
- At least one approval is required
- Changes may be requested
- Once approved, maintainers will merge

### After Merging

- Delete your feature branch
- Pull the latest changes:
  ```bash
  git checkout develop
  git pull upstream develop
  ```

## Community

### Getting Help

- GitHub Discussions for questions
- GitHub Issues for bugs and features
- Review existing documentation

### Recognition

Contributors are recognized in:
- CHANGELOG.md
- Release notes
- Project documentation

### License

By contributing, you agree that your contributions will be licensed under the same license as the project (MIT License).

## Additional Resources

- [GitHub Flow](https://guides.github.com/introduction/flow/)
- [Python Packaging Guide](https://packaging.python.org/)
- [PEP 8 Style Guide](https://www.python.org/dev/peps/pep-0008/)
- [Conventional Commits](https://www.conventionalcommits.org/)

## Questions?

If you have questions about contributing:

- Check our [Support Guide](SUPPORT.md)
- Ask in GitHub Discussions
- Review existing issues and PRs

---

Thank you for contributing to OpenEthos! Together, we're building better security tools for the Python community.
