# 社区治理文档模板库

> 以下模板可直接使用或根据项目情况定制。提供给用户时，提醒他们替换所有 `[占位符]` 内容。

## 目录

1. [CONTRIBUTING.md 模板](#1-contributingmd-模板)
2. [CODE_OF_CONDUCT.md 模板](#2-code_of_conductmd-模板)
3. [Bug Report Issue 模板](#3-bug-report-issue-模板)
4. [Feature Request Issue 模板](#4-feature-request-issue-模板)
5. [Pull Request 模板](#5-pull-request-模板)
6. [SECURITY.md 模板](#6-securitymd-模板)

---

## 1. CONTRIBUTING.md 模板

```markdown
# Contributing to [项目名]

First off, thank you for considering contributing to [项目名]! 🎉

## How Can I Contribute?

### Reporting Bugs

Before creating a bug report, please check existing issues to avoid duplicates.

When filing a bug report, include:
- **Environment**: OS, language version, [项目名] version
- **Steps to reproduce**: Minimal steps to trigger the issue
- **Expected behavior**: What you expected to happen
- **Actual behavior**: What actually happened
- **Screenshots/Logs**: If applicable

### Suggesting Features

Feature requests are welcome! Please:
1. Check existing issues/discussions first
2. Describe the problem you're trying to solve
3. Explain your proposed solution
4. Consider alternatives you've considered

### Submitting Pull Requests

1. Fork the repo and create your branch from `main`:
   ```bash
   git checkout -b feat/your-feature
   ```
2. Make your changes and add tests if applicable
3. Ensure all tests pass:
   ```bash
   [测试命令，如 make test / npm test / go test ./...]
   ```
4. Follow the existing code style
5. Write a clear PR description using our [PR template](.github/PULL_REQUEST_TEMPLATE.md)

### Development Setup

```bash
# Clone the repo
git clone https://github.com/[org]/[项目名].git
cd [项目名]

# Install dependencies
[安装命令]

# Run tests
[测试命令]

# Run locally
[本地运行命令]
```

## Code Style

- [描述代码风格要求，如 lint 工具、格式化规则]
- Run `[lint 命令]` before submitting

## Commit Message Convention

We follow [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `style:` Code style changes (formatting, no logic change)
- `refactor:` Code refactoring
- `test:` Adding or updating tests
- `chore:` Build process or auxiliary tool changes

Example: `feat(auth): add JWT token refresh mechanism`

## Code of Conduct

This project follows our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to abide by its terms.

## Questions?

Feel free to open a [Discussion](https://github.com/[org]/[项目名]/discussions) or reach out via [沟通渠道].

## License

By contributing, you agree that your contributions will be licensed under the project's [LICENSE](LICENSE).
```

---

## 2. CODE_OF_CONDUCT.md 模板

```markdown
# Code of Conduct

## Our Pledge

We as members, contributors, and leaders pledge to make participation in our
community a harassment-free experience for everyone, regardless of age, body
size, visible or invisible disability, ethnicity, sex characteristics, gender
identity and expression, level of experience, education, socio-economic status,
nationality, personal appearance, race, religion, or sexual identity and orientation.

## Our Standards

Examples of behavior that contributes to a positive environment:

- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

Examples of unacceptable behavior:

- Trolling, insulting/derogatory comments, and personal or political attacks
- Public or private harassment
- Publishing others' private information without explicit permission
- Other conduct which could reasonably be considered inappropriate

## Enforcement

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported to the project team at [联系邮箱]. All complaints will be reviewed
and investigated promptly and fairly.

## Attribution

This Code of Conduct is adapted from the [Contributor Covenant](https://www.contributor-covenant.org/), version 2.1.
```

---

## 3. Bug Report Issue 模板

文件路径: `.github/ISSUE_TEMPLATE/bug_report.md`

```markdown
---
name: Bug Report
about: Report a bug to help us improve
title: '[Bug] '
labels: bug
assignees: ''
---

## Describe the Bug

A clear and concise description of the bug.

## Steps to Reproduce

1. Go to '...'
2. Run '...'
3. See error

## Expected Behavior

What you expected to happen.

## Actual Behavior

What actually happened.

## Environment

- OS: [e.g., macOS 14.0, Ubuntu 22.04]
- [项目名] Version: [e.g., v1.2.3]
- [语言] Version: [e.g., Go 1.22, Python 3.11]

## Screenshots / Logs

If applicable, add screenshots or error logs.

## Additional Context

Any other context about the problem.
```

---

## 4. Feature Request Issue 模板

文件路径: `.github/ISSUE_TEMPLATE/feature_request.md`

```markdown
---
name: Feature Request
about: Suggest an idea for this project
title: '[Feature] '
labels: enhancement
assignees: ''
---

## Problem Statement

A clear description of the problem you're trying to solve.
Example: "I'm always frustrated when..."

## Proposed Solution

A clear description of what you want to happen.

## Alternatives Considered

Describe any alternative solutions or features you've considered.

## Additional Context

Add any other context, mockups, or examples about the feature request.
```

---

## 5. Pull Request 模板

文件路径: `.github/PULL_REQUEST_TEMPLATE.md`

```markdown
## Description

Brief description of the changes in this PR.

## Related Issue

Closes #[issue number]

## Type of Change

- [ ] 🐛 Bug fix (non-breaking change that fixes an issue)
- [ ] ✨ New feature (non-breaking change that adds functionality)
- [ ] 💥 Breaking change (fix or feature that would cause existing functionality to change)
- [ ] 📖 Documentation update
- [ ] 🧹 Refactoring (no functional changes)

## Checklist

- [ ] My code follows the project's code style
- [ ] I have added tests that prove my fix/feature works
- [ ] All new and existing tests pass
- [ ] I have updated the documentation accordingly
- [ ] I have read the [CONTRIBUTING](CONTRIBUTING.md) guide

## Screenshots (if applicable)

Before | After
--- | ---
[screenshot] | [screenshot]
```

---

## 6. SECURITY.md 模板

```markdown
# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| >= 1.0  | ✅         |
| < 1.0   | ❌         |

## Reporting a Vulnerability

If you discover a security vulnerability, please report it responsibly:

1. **Do NOT** create a public GitHub issue
2. Email us at [安全邮箱]
3. Include:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

We will acknowledge your email within 48 hours and provide a detailed response within 7 days.

## Disclosure Policy

- We will work with you to understand and resolve the issue
- We will credit you in the security advisory (unless you prefer anonymity)
- We aim to release a fix within 30 days of confirmation
```

---

## 使用提醒

向用户提供这些模板时，务必提醒：

⚠️ **请替换以下占位符后再使用：**
- `[项目名]` → 你的项目名称
- `[org]` → GitHub 组织名或用户名
- `[联系邮箱]` / `[安全邮箱]` → 项目维护者的联系邮箱
- `[沟通渠道]` → Discord/Slack/微信群等社区链接
- `[语言]` → 项目使用的编程语言
- `[测试命令]` / `[安装命令]` / `[本地运行命令]` / `[lint 命令]` → 项目实际使用的命令
