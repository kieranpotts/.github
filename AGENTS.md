# .github

Shared issue and PR templates, and other GitHub community health files for
Kieran Potts' personal repositories. This repo has no application code — it
holds config and Markdown templates consumed by GitHub itself and by GitHub
Actions workflows in other repositories.

The capitalized words REQUIRED, MUST, MUST NOT, RECOMMENDED, SHOULD,
SHOULD NOT, OPTIONAL, and MAY are to be interpreted as described in
[IETF RFC 2119](https://www.ietf.org/rfc/rfc2119.txt).

## Project structure

- **[.github/ISSUE_TEMPLATE/](./.github/ISSUE_TEMPLATE/)** \
  Issue templates shared across repositories (bug, epic, feature, incident,
  task, etc.).

- **[.github/PULL_REQUEST_TEMPLATE.md](./.github/PULL_REQUEST_TEMPLATE.md)** \
  Default PR description template.

- **[.github/labels.json](./.github/labels.json)** \
  Source-of-truth for GitHub labels. The `push-labels` workflow syncs this
  file to this repo's labels; other repositories then sync overnight to
  match.

- **[.github/workflows/](./.github/workflows/)** \
  GitHub Actions workflows: `push-labels`, `flag-stale-issues`,
  `validate-commit-messages`.

## Rules

- MUST keep `.github/labels.json` as the single source of truth for labels.
  Do not hand-edit labels in individual repositories.

- Issue and PR templates SHOULD stay generic enough to apply across all of
  Kieran Potts' personal repositories, since they are shared community
  health files.

- Changes to `.github/workflows/` MUST be tested carefully, since these
  workflows also drive label/state sync in other repositories.

## References

The following technical standards (TS) govern this project. Fetch and ingest
the relevant standards as-and-when required for the task at hand.

- [**TS-8: Issue Tracking**](https://kieranpotts.com/standards/008) \
  Use when creating, triaging, or reviewing issues in an issue tracker, or
  when designing issue-tracking workflows and boards.

- [**TS-9: Version Control**](https://kieranpotts.com/standards/009) \
  Use when working with Git. Covers commits, branching, merging, integration
  strategies, cutting releases, and configuring Git/PR/CI tooling.

- [**TS-60: GitHub Actions**](https://kieranpotts.com/standards/060) \
  Use when designing, authoring, reviewing, or securing GitHub Actions workflows
  or custom actions.

- [**TS-61: AI Tools**](https://kieranpotts.com/standards/061) \
  Use when planning or executing coding tasks, managing your own context,
  authoring AGENTS.md files or agent skills, calling tools, or handling
  untrusted content.
