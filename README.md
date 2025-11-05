# .github

Community health files and default configurations for [Sage.is](https://sage.is) repositories.

## About

This repository contains default community health files that are automatically used across all repositories in the Sage-is organization. These files help maintain consistency, quality, and community standards across all our projects.

## What's Included

### Community Health Files

- **[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)** - Our community guidelines and standards
- **[CONTRIBUTING.md](CONTRIBUTING.md)** - How to contribute to our projects
- **[SECURITY.md](SECURITY.md)** - Security policy and vulnerability reporting
- **[SUPPORT.md](SUPPORT.md)** - How to get help and support

### Documentation

- **[CHANGELOG.md](CHANGELOG.md)** - Version history and changes
- **[CONTRIBUTORS.md](CONTRIBUTORS.md)** - List of project contributors
- **[AUTHORS.md](AUTHORS.md)** - Project authors and maintainers
- **[ACKNOWLEDGMENTS.md](ACKNOWLEDGMENTS.md)** - Acknowledgments and credits

### GitHub Configuration

- **[CODEOWNERS](CODEOWNERS)** - Defines code ownership for automatic review requests
- **[.github/ISSUE_TEMPLATE/](.github/ISSUE_TEMPLATE/)** - Issue templates for bugs, features, and documentation
- **[.github/PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md)** - Pull request template
- **[.github/workflows/](.github/workflows/)** - GitHub Actions workflows for automation
- **[.github/dependabot.yml](.github/dependabot.yml)** - Dependabot configuration for dependency updates
- **[.github/FUNDING.yml](.github/FUNDING.yml)** - Funding and sponsorship information

### Metadata

- **[CITATION.cff](CITATION.cff)** - Citation metadata for academic references
- **[LICENSE](LICENSE)** - GNU Affero General Public License v3.0

## How It Works

GitHub automatically applies these files to all repositories in the Sage-is organization that don't have their own versions. This ensures:

- Consistent contributor experience across all projects
- Standardized issue and PR templates
- Unified community guidelines
- Automated workflows and processes

## Repository-Specific Overrides

Individual repositories can override any of these defaults by including their own versions of these files. This allows projects with special requirements to maintain their own policies while still benefiting from organization-wide defaults.

## Workflows

This repository includes several GitHub Actions workflows:

- **Lint** - Validates Markdown and YAML files
- **CodeQL** - Security scanning for vulnerabilities
- **Dependency Review** - Reviews dependency changes in PRs
- **Stale** - Manages stale issues and PRs
- **Greetings** - Welcomes first-time contributors
- **Auto Label** - Automatically labels PRs based on changes
- **Release** - Automates the release process

## Usage

### For Contributors

If you're contributing to any Sage.is project:

1. Read the [Code of Conduct](CODE_OF_CONDUCT.md)
2. Review the [Contributing Guidelines](CONTRIBUTING.md)
3. Check the [Support Documentation](SUPPORT.md) if you need help
4. Report security issues following the [Security Policy](SECURITY.md)

### For Maintainers

If you're maintaining a Sage.is project:

1. These files are automatically available in your repository
2. Override them by creating your own versions if needed
3. Keep CODEOWNERS up to date with your team structure
4. Customize issue templates for project-specific needs

## Development

### Local Testing

You can test these configurations locally:

```bash
# Clone the repository
git clone https://github.com/Sage-is/.github.git
cd .github

# Test workflows (requires act)
act -l

# Lint Markdown files
npx markdownlint '**/*.md' --config .markdownlint.json

# Lint YAML files
yamllint -c .yamllint.yml .
```

### Making Changes

1. Create a feature branch
2. Make your changes
3. Test thoroughly
4. Submit a pull request
5. Wait for review and approval

## Links

- **Website**: [https://sage.is](https://sage.is)
- **Organization**: [https://github.com/Sage-is](https://github.com/Sage-is)
- **Documentation**: See individual files in this repository

## License

This repository is licensed under the [GNU Affero General Public License v3.0](LICENSE).

## Questions?

If you have questions about these community health files or how they're used:

1. Check the [Support Guide](SUPPORT.md)
2. Open an [issue](https://github.com/Sage-is/.github/issues)
3. Visit [https://sage.is](https://sage.is)

---

Made with ❤️ by the Sage.is community