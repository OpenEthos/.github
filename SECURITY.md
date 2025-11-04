# Security Policy

## Our Commitment

OpenEthos is committed to ensuring the security of our projects and the safety of our users. We take security vulnerabilities seriously and appreciate the efforts of security researchers and users who help us maintain secure software.

## Supported Versions

We provide security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |
| < Latest| :x:                |

We recommend always using the latest version of our software to ensure you have the most recent security patches.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, please report them through one of the following methods:

### Preferred Method: GitHub Security Advisories

1. Navigate to the specific repository where you found the vulnerability
2. Go to the "Security" tab
3. Click "Report a vulnerability"
4. Fill out the advisory form with detailed information

### Alternative Method: Email

If you prefer, you can also email security concerns to:
- **Email**: [Create an issue in the repository and request private contact]

### What to Include

When reporting a vulnerability, please include:

- **Description**: A clear description of the vulnerability
- **Impact**: The potential impact and severity
- **Reproduction Steps**: Detailed steps to reproduce the issue
- **Affected Versions**: Which versions are affected
- **Proof of Concept**: If possible, include a proof of concept
- **Suggested Fix**: If you have ideas on how to fix it
- **Your Contact Information**: So we can follow up with questions

## Response Timeline

We aim to respond to security reports according to the following timeline:

- **Initial Response**: Within 48 hours
- **Confirmation and Assessment**: Within 7 days
- **Fix Development**: Varies based on complexity
- **Public Disclosure**: After a fix is available and deployed

## Security Update Process

1. **Acknowledgment**: We acknowledge receipt of your report
2. **Investigation**: We investigate and validate the vulnerability
3. **Fix Development**: We develop and test a fix
4. **Security Advisory**: We prepare a security advisory
5. **Release**: We release the fix
6. **Disclosure**: We publicly disclose the vulnerability after the fix is available

## Public Disclosure

We follow a coordinated disclosure approach:

- We will work with you to understand the vulnerability
- We will develop a fix as quickly as possible
- We will coordinate the disclosure timing with you
- We prefer to release fixes before public disclosure
- We will credit you for the discovery (unless you prefer to remain anonymous)

## Security Best Practices

When using OpenEthos projects:

### For Users

- Always use the latest version
- Keep dependencies up to date
- Follow the security guidelines in our documentation
- Enable security features like multi-factor authentication
- Review security advisories regularly

### For Contributors

- Follow secure coding practices
- Run security scans before submitting PRs
- Never commit secrets, tokens, or credentials
- Use security linters (bandit, safety, etc.)
- Review the CONTRIBUTING.md file for security requirements

## Security Features

Our projects include:

- **Dependency Scanning**: Automated checks for vulnerable dependencies
- **Code Scanning**: Static analysis security testing (SAST)
- **Secret Scanning**: Detection of committed secrets
- **Security Workflows**: Automated security testing in CI/CD

## Scope

This security policy applies to:

- All repositories under the OpenEthos organization
- All officially released versions
- All supported platforms and Python versions

Out of scope:

- Issues in third-party dependencies (please report to the respective maintainers)
- Social engineering attacks
- Denial of service attacks requiring unrealistic resources

## Recognition

We appreciate the security research community and will:

- Acknowledge your contribution in the security advisory
- Credit you in release notes (with your permission)
- Provide updates on the fix progress

## Contact

For security-related questions or concerns:

- Use GitHub Security Advisories (preferred)
- Create a private security report in the relevant repository
- For general security questions, use GitHub Discussions

## Additional Resources

- [GitHub Security Advisories](https://docs.github.com/en/code-security/security-advisories)
- [OpenEthos Contributing Guidelines](CONTRIBUTING.md)
- [OpenEthos Support](SUPPORT.md)

## Changes to This Policy

We may update this security policy from time to time. Please check back periodically for updates.

---

Thank you for helping keep OpenEthos and our users safe!
