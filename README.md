# .github

Community health files and default configurations for [Sage.is](https://sage.is) repositories.

## About

This repository contains default community health files that GitHub automatically makes available to all public
repositories in the Sage-is organization. Using GitHub's
[default community health files feature](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file),
these files help maintain consistency, quality, and community standards across all our projects.

**Important**: This is not a repository that needs to be cloned or manually integrated. GitHub automatically uses
these files as fallbacks for any repository in the organization that doesn't have its own versions.

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

This repository leverages GitHub's
[default community health files feature](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).
When a repository named `.github` exists in an organization, GitHub automatically makes its community health files
available to all public repositories in that organization.

**No cloning or setup required!** GitHub automatically:

- Displays these files when they're accessed in repositories that don't have their own versions
- Shows links to them in repository insights and community profile
- Makes issue and PR templates available when creating new issues or pull requests
- Applies CODEOWNERS rules for automated review requests

This ensures:

- Consistent contributor experience across all projects
- Standardized issue and PR templates
- Unified community guidelines
- Automated workflows and processes

**Note**: This is different from using a `.github` repository for organization branding (profile README). This
repository serves as a **fallback** for community health files across all organization repositories.

## Repository-Specific Overrides

Individual repositories can override any of these defaults by including their own versions of these files. This
allows projects with special requirements to maintain their own policies while still benefiting from
organization-wide defaults.

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

1. **No action needed** - These files are automatically available via GitHub's feature (no cloning required)
2. Your repository will use these defaults unless you create your own versions
3. To override: Simply create your own version of any file in your repository
4. Keep CODEOWNERS up to date with your team structure
5. Customize issue templates for project-specific needs

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

## Frequently Asked Questions

### Do I need to clone this repository?

**No.** This repository uses GitHub's built-in feature for default community health files. GitHub automatically
provides these files to all repositories in the Sage-is organization. You don't need to clone, fork, or manually
copy anything.

### How is this different from organization branding?

While a `.github` repository can be used for organization branding (like a profile README), this repository
primarily serves as a **central location for default community health files**. GitHub automatically uses these
files as fallbacks across all organization repositories.

### What files are automatically used?

GitHub automatically provides the following files from this repository to other repos in the organization:

- CODE_OF_CONDUCT.md
- CONTRIBUTING.md
- SECURITY.md
- SUPPORT.md
- FUNDING.yml
- Issue and PR templates
- Workflow files (for organization-wide automation)

### How do I customize for my specific repository?

Simply create your own version of any file in your repository. Your local version will always take precedence over
the organization default.

## License

This repository is licensed under the [GNU Affero General Public License v3.0](LICENSE).

## Questions?

If you have questions about these community health files or how they're used:

1. Check the [Support Guide](SUPPORT.md)
2. Open an [issue](https://github.com/Sage-is/.github/issues)
3. Visit [https://sage.is](https://sage.is)

---

Made with ❤️ by the Sage.is community
