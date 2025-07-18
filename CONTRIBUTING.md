# Contributing to ABsmartly

First off, thank you for considering contributing to ABsmartly! 🎉 

It's people like you that make ABsmartly such a great tool for the developer community. This document provides guidelines for contributing to the various ABsmartly repositories.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How Can I Contribute?](#how-can-i-contribute)
  - [Reporting Bugs](#reporting-bugs)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Your First Code Contribution](#your-first-code-contribution)
  - [Pull Requests](#pull-requests)
- [Development Process](#development-process)
- [Style Guides](#style-guides)
  - [Git Commit Messages](#git-commit-messages)
  - [Code Style](#code-style)
  - [Documentation Style](#documentation-style)
- [Community](#community)

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code. Please be respectful and considerate in all interactions.

## Getting Started

ABsmartly consists of multiple repositories:

- **SDKs**: Language-specific implementations (Java, JavaScript, Python, etc.)
- **Tools**: Chrome Extension, MCP Server, CLI
- **Documentation**: Guides and API references

Each repository may have specific setup instructions in their README files. Please check the repository you're interested in contributing to.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, please include:

- **Clear and descriptive title**
- **Detailed description** of the issue
- **Steps to reproduce** the problem
- **Expected behavior** vs actual behavior
- **Screenshots** if applicable
- **Environment details** (OS, browser, SDK version, etc.)

**Example Bug Report:**
```markdown
### Bug: JavaScript SDK throws error when treatment name contains spaces

**Description:**
When calling `context.getTreatment("my experiment")`, the SDK throws an InvalidArgumentError.

**Steps to Reproduce:**
1. Initialize ABsmartly SDK
2. Create context with valid units
3. Call `context.getTreatment("my experiment")`

**Expected:** Should return treatment value
**Actual:** Throws InvalidArgumentError

**Environment:**
- SDK Version: 1.2.3
- Node Version: 18.0.0
- OS: macOS 13.0
```

### Suggesting Enhancements

Enhancement suggestions are welcome! Please provide:

- **Use case** - Why is this enhancement needed?
- **Proposed solution** - How do you envision it working?
- **Alternatives considered** - What other solutions did you think about?
- **Additional context** - Any other relevant information

### Your First Code Contribution

Unsure where to begin? Look for issues labeled:

- `good first issue` - Simple issues perfect for beginners
- `help wanted` - Issues where we need community help
- `documentation` - Documentation improvements

### Pull Requests

1. **Fork the repository** and create your branch from `main`
2. **Write clear, focused commits** following our commit message guidelines
3. **Add tests** for any new functionality
4. **Update documentation** as needed
5. **Ensure all tests pass** before submitting
6. **Submit a pull request** with a clear description

**Pull Request Template:**
```markdown
## Description
Brief description of what this PR does

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
- [ ] Unit tests pass
- [ ] Integration tests pass
- [ ] Manual testing completed

## Checklist
- [ ] My code follows the project style guidelines
- [ ] I've added tests for my changes
- [ ] I've updated relevant documentation
- [ ] All new and existing tests pass
```

## Development Process

### 1. Setting Up Your Development Environment

Most SDKs follow a similar setup pattern:

```bash
# Clone the repository
git clone https://github.com/absmartly/[repository-name]
cd [repository-name]

# Install dependencies
npm install  # for JavaScript projects
pip install -r requirements.txt  # for Python projects
mvn install  # for Java projects

# Run tests
npm test
pytest
mvn test
```

### 2. Making Changes

1. Create a feature branch: `git checkout -b feature/your-feature-name`
2. Make your changes
3. Write/update tests
4. Run the test suite
5. Commit your changes

### 3. Testing

All contributions must include appropriate tests:

- **Unit tests** for individual functions/methods
- **Integration tests** for feature workflows
- **End-to-end tests** for critical paths

### 4. Documentation

Update documentation for:

- New features or APIs
- Changed behavior
- Configuration options
- Usage examples

## Style Guides

### Git Commit Messages

Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
type(scope): subject

body

footer
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Test additions or corrections
- `chore`: Maintenance tasks

**Examples:**
```
feat(sdk): add support for custom attributes

fix(javascript): handle undefined treatment gracefully

docs(readme): update installation instructions for npm
```

### Code Style

Each language has its own style guide:

#### JavaScript/TypeScript
- Use ESLint configuration provided
- Prefer `const` over `let`
- Use meaningful variable names
- Add JSDoc comments for public APIs

#### Python
- Follow PEP 8
- Use type hints where applicable
- Document functions with docstrings

#### Java
- Follow standard Java conventions
- Use JavaDoc for public methods
- Maintain consistent indentation

#### Go
- Run `go fmt` before committing
- Follow effective Go guidelines
- Keep functions focused and small

### Documentation Style

- Use clear, concise language
- Include code examples
- Explain the "why" not just the "how"
- Keep README files up to date
- Use proper markdown formatting

## Community

### Getting Help

- **Documentation**: https://docs.absmartly.com
- **Issues**: GitHub issues in relevant repository
- **Email**: support@absmartly.com

### Recognition

Contributors are recognized in several ways:

- Listed in repository contributors
- Mentioned in release notes for significant contributions
- Featured in our blog for major features

## Repository-Specific Guidelines

Some repositories may have additional guidelines:

### SDKs
- Maintain backward compatibility
- Follow semantic versioning
- Include migration guides for breaking changes

### Chrome Extension
- Test across multiple Chrome versions
- Ensure compatibility with Manifest V3
- Consider performance impact

### MCP Server
- Follow Model Context Protocol specifications
- Ensure tool descriptions are clear
- Test with multiple MCP clients

## Questions?

Feel free to open an issue for any questions about contributing. We're here to help make your contribution experience smooth and enjoyable!

Thank you for contributing to ABsmartly! 🚀