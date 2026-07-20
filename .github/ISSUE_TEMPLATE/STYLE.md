---
name: Style
about: Suggest code formatting improvements (whitespace, indentation, style).
title: ""
labels: STYLE
assignees: ""
---

Write a concise description of the formatting issues in the codebase.

> **Note**: This issue type covers low-level code formatting concerns only—whitespace, indentation, line wrapping, and code style. For structural improvements to code design, logic, or architecture, use the `REFACTORING` issue type instead.

## Scope

List the specific files, directories, or code sections targeted for formatting improvements. Examples:

- Apply `prettier` to `src/` directory.
- Enforce consistent indentation in test files.
- Standardize import order across the codebase.
- Format docstrings to match style guide.

## Current state

Describe the formatting inconsistencies or issues, eg.:

- Lines exceeding the column limit.
- Inconsistent whitespace or indentation.
- Deviations from the project's style guide.
- Formatter (eg. `prettier`, `black`, `gofmt`) would produce changes.

## Desired state

Specify the desired formatting standard after improvements, eg.:

- All code formatted by `prettier` with project config.
- Consistent 2-space indentation throughout.
- Line length capped at 80 characters.
- Adherence to style guide rules.

## Automated tooling

List any formatting tools or linters that could automate this work, eg.:

- `prettier` for JavaScript/TypeScript.
- `black` for Python.
- `gofmt` for Go.
- `eslint --fix` for code style.

If automation is available, describe whether a single tool run can fix all issues, or if manual adjustments will be needed afterward.

## Impact

Briefly describe any impact on the codebase:

- No behavioral changes expected (formatting only).
- May affect line counts in blame/history.
- Potential merge conflicts with in-flight feature branches.

## Additional notes

Add any other context, style guide references, or links to discussions about formatting standards.
