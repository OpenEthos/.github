# OpenEthos .github Repository

This is the `.github` meta-repository for the **OpenEthos** organization. It contains default community health files, workflow templates, and organizational configurations that are automatically applied to all repositories in the OpenEthos organization.

## 🎯 Purpose

This repository serves as:

- **Default Community Health Files**: Provides default templates for issues, pull requests, and community guidelines
- **Workflow Templates**: Reusable GitHub Actions workflows for Python projects
- **Organizational Standards**: Defines standards and best practices for all OpenEthos projects
- **Security Policies**: Centralized security reporting and policies

## 📁 Repository Structure

```
.github/
├── workflow-templates/          # Reusable GitHub Actions workflows
│   ├── python-ci.yml           # Python CI with linting and testing
│   ├── python-security-scan.yml # Security scanning with Bandit, CodeQL
│   ├── python-publish.yml      # Package publishing to PyPI
│   └── python-dependency-update.yml # Automated dependency updates
├── .github/
│   ├── ISSUE_TEMPLATE/         # Issue templates
│   │   ├── config.yml         # Issue template configuration
│   │   ├── bug_report.yml     # Bug report template
│   │   ├── feature_request.yml # Feature request template
│   │   ├── chore.yml          # Chore/maintenance template
│   │   ├── question.yml       # Question template
│   │   ├── security.yml       # Security issue template
│   │   └── workflow.yml       # Workflow issue template
│   ├── PULL_REQUEST_TEMPLATE.md # Pull request template
│   ├── CODEOWNERS             # Code ownership definitions
│   └── FUNDING.yml            # Funding information
├── SECURITY.md                 # Security policy
├── SUPPORT.md                  # Support information
├── CONTRIBUTING.md             # Contribution guidelines
├── CODE_OF_CONDUCT.md          # Code of conduct
└── profile/
    └── README.md              # Organization profile README
```

## 🔄 Workflow Templates

Our workflow templates provide ready-to-use CI/CD configurations for Python projects:

### Python CI (`python-ci.yml`)
Comprehensive CI workflow with:
- Code linting (flake8, black, pylint)
- Type checking (mypy)
- Testing across multiple Python versions (3.9-3.12)
- Multi-platform testing (Ubuntu, Windows, macOS)
- Code coverage reporting

### Python Security Scan (`python-security-scan.yml`)
Security-focused workflow with:
- Bandit security scanning
- Safety dependency vulnerability checks
- pip-audit for dependency auditing
- CodeQL analysis
- Scheduled weekly scans

### Python Package Publishing (`python-publish.yml`)
Package publishing workflow with:
- Automated building and packaging
- PyPI publishing with trusted publishing
- TestPyPI support for testing
- Release-triggered publishing

### Python Dependency Update (`python-dependency-update.yml`)
Automated dependency management:
- Weekly dependency updates
- Automated PR creation
- pip-tools integration
- Dependency compilation and upgrades

## 📋 Issue Templates

We provide comprehensive issue templates for:

- **Bug Reports**: Detailed bug reporting with environment information
- **Feature Requests**: Feature suggestions with priority levels
- **Chores**: Maintenance tasks and housekeeping
- **Questions**: General questions and help requests
- **Security Issues**: Security concerns (non-vulnerabilities)
- **Workflow Issues**: CI/CD and GitHub Actions problems

## 🔐 Security

### Reporting Vulnerabilities

**Do not create public issues for security vulnerabilities.**

Please report security vulnerabilities through:
1. GitHub Security Advisories (preferred)
2. Private security reports in the relevant repository

See [SECURITY.md](SECURITY.md) for complete details.

### Security Features

All OpenEthos projects benefit from:
- Automated security scanning
- Dependency vulnerability checks
- CodeQL analysis
- Secret scanning
- Security advisories

## 🤝 Contributing

We welcome contributions to improve our templates and standards!

### How to Contribute

1. Review our [Contributing Guidelines](CONTRIBUTING.md)
2. Check existing issues and pull requests
3. Submit your improvements via pull request
4. Follow our [Code of Conduct](CODE_OF_CONDUCT.md)

### What to Contribute

- Improvements to workflow templates
- New issue templates
- Documentation updates
- Best practice suggestions
- Bug fixes

## 📚 Community Health Files

These files are automatically available in all OpenEthos repositories:

- **CODE_OF_CONDUCT.md**: Our commitment to an inclusive community
- **CONTRIBUTING.md**: How to contribute to our projects
- **SECURITY.md**: Security policy and vulnerability reporting
- **SUPPORT.md**: How to get help and support

## 🎓 Best Practices

### For Repository Maintainers

1. **Use Workflow Templates**: Start new projects with our workflow templates
2. **Follow Issue Templates**: Encourage use of issue templates
3. **Review CODEOWNERS**: Keep CODEOWNERS file updated
4. **Security First**: Enable security features in all repositories
5. **Documentation**: Maintain comprehensive documentation

### For Contributors

1. **Read Guidelines**: Review CONTRIBUTING.md before contributing
2. **Use Templates**: Use appropriate issue/PR templates
3. **Follow Standards**: Adhere to coding standards
4. **Test Thoroughly**: Test your changes before submitting
5. **Security Aware**: Follow security best practices

## 🔗 Resources

### GitHub Documentation

- [Creating Default Community Health Files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [Workflow Templates](https://docs.github.com/en/actions/using-workflows/creating-starter-workflows-for-your-organization)
- [Issue Templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests)
- [Security Advisories](https://docs.github.com/en/code-security/security-advisories)

### OpenEthos Projects

- [SecurityGuard](https://github.com/OpenEthos/securityguard): Security and compliance tool
- [Organization Page](https://github.com/OpenEthos): All OpenEthos projects

## 📝 License

All files in this repository are released under the [MIT License](LICENSE).

## 🆘 Support

Need help?

- Check our [Support Guide](SUPPORT.md)
- Visit [GitHub Discussions](https://github.com/orgs/OpenEthos/discussions)
- Review project documentation

## 🙏 Acknowledgments

Thank you to all contributors who help maintain these standards and templates!

## 📞 Contact

- GitHub Issues: For bugs and feature requests
- GitHub Discussions: For questions and community interaction
- Security: Use GitHub Security Advisories for vulnerabilities

---

**OpenEthos** - Building secure, compliant Python applications through automation and best practices.
