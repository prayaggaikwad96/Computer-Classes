# Computer Classes

A structured learning archive for computer-class notes, exercises, and revision.

## Contents

- **Class notes:** organize material by subject and topic.
- **Practice work:** keep examples small, named clearly, and easy to revisit.
- **Revision:** add a short topic README when a folder needs context or setup instructions.

## Suggested structure

```text
.
├── README.md
├── programming/
├── databases/
├── networking/
└── operating-systems/
```

Use this as an optional structure; keep existing files where they belong until you have reviewed them.

## Good repository hygiene

- Use descriptive filenames and dated folders only when dates help.
- Keep credentials, API keys, passwords, private records, and real `.env` files out of Git.
- Use `.env.example` for non-secret configuration templates.
- Verify notes against the original class material before relying on them.
- Add setup steps to examples that need dependencies.
- Review dependency updates before merging them; do not blindly accept major-version changes.

## Quality, security, and maintenance

- The default branch is `main`.
- GitHub reports branch protection enabled for `main`; the branch metadata currently shows no required status checks. Configure required checks after confirming their stable names in GitHub Actions.
- [CodeQL](.github/workflows/codeql.yml) runs on pushes, pull requests, a weekly schedule, and manual dispatch. Its current workflow is configured to analyze GitHub Actions workflows.
- [Dependabot](.github/dependabot.yml) checks GitHub Actions dependencies weekly. Review and test dependency pull requests before merging.
- [Contributing guide](CONTRIBUTING.md) describes branch, content-quality, and review expectations.
- [Security policy](SECURITY.md) explains private vulnerability reporting and credential-handling rules.
- Never commit secrets. Rotate any exposed credential; deleting a file does not revoke a credential.

A workflow being configured does not prove that all checks passed for a particular commit. Verify the exact commit SHA and latest run before merging.

## Status

This is a learning archive. Materials may be incomplete and are intended for learning and revision. Verify technical notes against current official documentation where version-sensitive behavior matters.

---

Maintained by [Prayag Gaikwad](https://github.com/prayaggaikwad96).
