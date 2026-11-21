# GitHub account remediation audit — 2026-11-21

The cross-repository audit summary is maintained in the Full-Stack-Development repository at:
`docs/github-account-remediation-audit-2026-11-21.md`

## Computer-Classes live result
- Default branch: `main`.
- PR #10 merged by squash into `main` at `a0ecfea2c63098e03a537551c9ed2063b79c9abe`.
- The merged change adds weekly GitHub Actions Dependabot updates and documents repository maintenance, CodeQL scope, dependency review and security/contribution guidance.
- The exact PR head was `778f0db94617b655e692917758aa4d19c02b4d4c`; CodeQL was observed successful.
- Existing SECURITY.md, CONTRIBUTING.md, CODEOWNERS, issue templates and CodeQL workflow remain present.
- `Developer` is not synchronized with `main`: comparison showed Developer 1 commit ahead and 7 commits behind, diverged, with `.github/BRANCH_PROTECTION.md` on Developer. This branch must not be force-reset or merged without examining its intended governance purpose.
- GitHub branch-protection settings could not be inspected through the connected integration (403); no protection settings were changed.
- Audit branch created: `sync/main-to-developer-2026-11-21-audit`. No primary branch moved.
