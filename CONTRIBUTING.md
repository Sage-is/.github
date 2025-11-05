# Contributing to Sage.is

Thank you for your interest in contributing to Sage.is! We welcome contributions from the community and are grateful for your support.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Process](#development-process)
- [Style Guidelines](#style-guidelines)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to conduct@sage.is.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the issue tracker to avoid duplicates. When creating a bug report, include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples** to demonstrate the steps
- **Describe the behavior you observed and what you expected**
- **Include screenshots or animated GIFs** if relevant
- **Note your environment** (OS, version, etc.)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear and descriptive title**
- **Provide a detailed description** of the proposed enhancement
- **Explain why this enhancement would be useful**
- **List any similar features** in other projects

### Your First Code Contribution

Unsure where to begin? Look for issues labeled:

- `good first issue` - Good for newcomers
- `help wanted` - Extra attention needed

### Pull Requests

- Fill in the pull request template
- Follow the style guidelines
- Include tests if applicable
- Update documentation as needed
- Ensure all tests pass

## Development Process

### Setting Up Your Development Environment

1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/REPOSITORY.git
   cd REPOSITORY
   ```
3. Add upstream remote:
   ```bash
   git remote add upstream https://github.com/Sage-is/REPOSITORY.git
   ```
4. Create a branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Making Changes

1. Make your changes in your feature branch
2. Test your changes thoroughly
3. Commit your changes (see [Commit Messages](#commit-messages))
4. Push to your fork
5. Open a pull request

### Running Tests

```bash
# Install dependencies
npm install  # or pip install -r requirements.txt, etc.

# Run tests
npm test     # or pytest, cargo test, etc.

# Run linters
npm run lint # or pylint, etc.
```

## Style Guidelines

### General Guidelines

- Write clear, readable code
- Comment complex logic
- Follow the existing code style
- Keep functions small and focused
- Write descriptive variable and function names

### Language-Specific Guidelines

- **JavaScript/TypeScript**: Follow the project's ESLint configuration
- **Python**: Follow PEP 8
- **Go**: Use `gofmt` and `golint`
- **Rust**: Use `rustfmt` and `clippy`

### Documentation

- Update README.md if you change functionality
- Add JSDoc/docstrings for new functions
- Update relevant documentation files
- Include code examples where appropriate

## Commit Messages

Write clear, meaningful commit messages:

### Format

```
type(scope): subject

body

footer
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
feat(api): add user authentication endpoint

Implement JWT-based authentication for API endpoints.
Includes token generation and validation.

Closes #123
```

```
fix(ui): correct button alignment in mobile view

The submit button was misaligned on screens smaller than 768px.
Updated CSS to use flexbox for proper alignment.
```

## Pull Request Process

1. **Update Documentation**: Ensure documentation reflects your changes
2. **Update CHANGELOG**: Add your changes to CHANGELOG.md under [Unreleased]
3. **Pass CI Checks**: All automated tests must pass
4. **Get Reviews**: Request reviews from maintainers
5. **Address Feedback**: Respond to review comments
6. **Squash Commits**: Consider squashing commits before merge (if requested)

### Pull Request Template

When you open a PR, fill in all sections of the template:

- Description of changes
- Motivation and context
- Types of changes
- Testing performed
- Checklist items

## Community

### Getting Help

- Read the [Support Guide](SUPPORT.md)
- Check existing issues and discussions
- Ask questions in GitHub Discussions

### Recognition

Contributors are recognized in:

- [CONTRIBUTORS.md](CONTRIBUTORS.md)
- Release notes
- Project documentation

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (see [LICENSE](LICENSE)).

## Questions?

Don't hesitate to ask! Open an issue or reach out through our community channels.

Thank you for contributing to Sage.is! 🎉
