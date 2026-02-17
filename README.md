# VibeInProd GitHub Defaults

This repository contains organization-wide GitHub community health files and defaults used across VibeInProd repositories.

## What this repo controls

- Pull request guidance and review checklist defaults
- Issue intake templates and form configuration defaults
- Security disclosure and reporting policy
- Organization profile content shown on GitHub

## Repository structure

- `PULL_REQUEST_TEMPLATE.md` — default pull request template for repositories that do not override it
- `ISSUE_TEMPLATE/` — default issue forms/templates and issue creation configuration
- `SECURITY.md` — default security policy and vulnerability reporting process
- `profile/README.md` — public organization profile README
- `profile/images/` — assets referenced by the profile README

## How precedence works

GitHub uses repository-local files first. This repo provides defaults when a target repository does not define its own equivalents.

In practice:

- A repo-level `SECURITY.md` overrides this default
- A repo-level pull request template overrides this default
- A repo-level issue template/form configuration overrides these defaults

## Updating these defaults

1. Make focused changes with clear rationale in the pull request.
2. Keep language actionable and consistent with existing policy tone.
3. Validate links, image paths, and markdown rendering before merge.
4. Note rollout impact in the PR (which repositories/users are affected).

## Related docs

- Security policy: `SECURITY.md`
- PR template: `PULL_REQUEST_TEMPLATE.md`
- Issue templates/forms: `ISSUE_TEMPLATE/`
- Org profile content: `profile/README.md`

## Notes

- This repository does not ship application code.
- Changes here primarily affect contributor workflows, governance, and organization presentation.