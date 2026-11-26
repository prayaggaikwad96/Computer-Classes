# Branch Protection Policy

**Live status checked: 26 November 2026**

GitHub's branch listing currently reports:

| Branch | Role | GitHub protected flag |
| --- | --- | --- |
| `main` | Default branch | `true` |
| `Developer` | Development branch | `false` |

The `main` branch is protected at the branch level. This does **not** prove that every recommended setting is enabled: the connected GitHub integration cannot read the detailed classic branch-protection rules (the endpoint returned 403). The repository-level rulesets endpoint returned an empty list.

## Recommended policy

Keep `main` protected. If `Developer` remains an active integration branch, protect it as well.

For each active protected branch:

- Require pull requests before merging.
- Require independent approval when another qualified reviewer is available; never treat the PR author's own review as approval.
- Dismiss stale approvals after new commits and require review conversations to be resolved.
- Require only status checks that actually run reliably for the branch and its pull requests. This repository currently has a CodeQL workflow; verify its exact check context before making it mandatory.
- Block force pushes and branch deletion.
- Include administrators in protection and restrict bypass to documented emergencies.

Do not invent CI checks for this learning archive or require checks that do not run on every relevant PR.

## Apply and verify

Use **Repository Settings → Rules → Rulesets** or **Settings → Branches**. This file records policy and observed status; it does not turn protection on or modify GitHub settings.

After applying any rule to `Developer`, verify the effective settings and a real pull request before marking the branch protected.
