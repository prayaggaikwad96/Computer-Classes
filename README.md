# Computer Classes

A structured learning archive for computer-science and IT class notes, practical examples, exercises, and revision.

This repository is a study archive, not a single runnable application. Course materials are added as they are prepared; the subject folders described below are an organizational plan, not a claim that every folder already exists.

## How to use this repository

1. Open the subject and topic folder relevant to the material you are studying.
2. Start with that topic's `README.md`, when present, for prerequisites, learning objectives, and references.
3. Read the notes, then work through the examples and exercises yourself.
4. Check version-sensitive technical details against current official documentation and record the version or date where it matters.
5. Treat unfinished examples as learning material, not production-ready code.

## Current repository map

The root currently contains the repository guidance and project-maintenance files:

```text
.
├── .github/
│   ├── CODEOWNERS
│   ├── ISSUE_TEMPLATE/
│   ├── ISSUE_TEMPLATE.md
│   ├── dependabot.yml
│   ├── pull_request_template.md
│   └── workflows/
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── README.md
├── SECURITY.md
└── profile-readme-template.md
```

No subject-specific course folders are currently present at the repository root. Add them as actual material is published rather than documenting empty or hypothetical directories as existing content.

## Suggested subject organization

When notes are added, group them by subject. For example:

```text
.
├── programming/
├── databases/
├── networking/
└── operating-systems/
```

Within a subject, keep each topic focused. A topic can include a short `README.md`, notes, source-code examples, exercises, and references. Create only the sections that are useful for that topic.

## Content quality

- Prefer clear explanations, small examples, and meaningful filenames.
- Separate concepts, worked examples, exercises, and solutions where practical.
- State prerequisites and include setup/run instructions when an example needs tools or dependencies.
- Show expected output and explain important edge cases.
- Verify notes against reliable primary sources, especially for version-dependent behavior.
- Cite external material and preserve the attribution and license terms that apply to it.
- Add tests for executable examples when practical; do not imply an example was tested unless it was run.

## Good repository hygiene

- Use descriptive filenames and dated folders only when dates help readers understand the material.
- Keep credentials, API keys, passwords, private records, and real `.env` files out of Git.
- Use `.env.example` for non-secret configuration templates.
- Never commit personal data or private class records without permission.
- Review dependency updates before merging them; do not blindly accept major-version changes.
- Rotate any exposed credential. Deleting a file from a later commit does not revoke it.

## Automation, quality, and security

- **Default branch:** `main`. Use focused branches and pull requests for changes.
- **CodeQL:** [The checked-in workflow](.github/workflows/codeql.yml) runs on pushes, pull requests, a weekly schedule, and manual dispatch. Its current configuration analyzes GitHub Actions workflows; it is not a general-purpose scan of every possible language or learning example.
- **Dependabot:** [The configuration](.github/dependabot.yml) checks GitHub Actions dependencies weekly. Review and test dependency pull requests before merging.
- **Branch rules:** verify current branch protection, rulesets, and required status checks in GitHub Settings. A README or the presence of a workflow does not prove that a branch is protected or that checks are required.
- **Exact commits:** before merging, inspect the latest workflow run for the exact pull-request head SHA. A configured workflow does not prove that a particular commit passed.
- **Security reporting:** follow [SECURITY.md](SECURITY.md) for private vulnerability disclosure. Do not publish credentials or exploitable details in public issues.

## Contributing and community standards

- Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing structural or content changes.
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md).
- Use the repository's issue templates to report a reproducible problem or suggest a topic.
- The [CODEOWNERS file](.github/CODEOWNERS) identifies the configured code owners.

## Status and maintenance

This is a growing learning archive. Some topics may be incomplete or awaiting review. Verify technical notes against current official documentation whenever behavior, APIs, or tool versions may have changed.

Maintained by [Prayag Gaikwad](https://github.com/prayaggaikwad96).
