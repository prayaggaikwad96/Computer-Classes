# Branch protection policy

The `Developer` branch is a protected integration branch and must follow the same protection standard as `main`.

Configure the branch protection rule in **Settings → Branches → Add branch protection rule**:

- Branch name pattern: `Developer`
- Require a pull request before merging.
- Require at least one approval when independent reviewers are available; for a solo-maintained repository, use CODEOWNERS/required checks as the quality gate rather than a fictitious approval.
- Dismiss stale approvals when new commits are pushed.
- Require conversation resolution.
- Require status checks before merging, selecting only checks that are actually emitted by the workflows in this repository.
- Require branches to be up to date before merging when the required check set is stable.
- Require linear history if the repository's merge strategy supports it.
- Block force pushes and branch deletion.
- Do not allow bypassing the rules except for a documented emergency.

**Important:** This file documents the desired policy; it does not itself enable GitHub branch protection. Apply the settings in repository Settings (the connected GitHub integration cannot administer branch protection for this account).
