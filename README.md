# Workflows

[![Lint code base][lintbadge]][lintworkflow]

[lintbadge]:    <https://github.com/bewuethr/workflows/actions/workflows/linter-caller.yml/badge.svg>
[lintworkflow]: <https://github.com/bewuethr/workflows/actions/workflows/linter-caller.yml>

This repo hosts reusable workflows.

- `addtoproject.yml`: wraps [*actions/add-to-project*][atp] and takes the same
  parameters as the action
- `linter.yml`: wraps [*github/super-linter/slim*][sl], providing default style
  files for markdowlint, shfmt, yamllint, and stylelint (CSS) if a repo doesn't
  provide them. ShellCheck, Bash exec, actionlint, gitleaks, copy-paste
  detection, markdownlint, shfmt, and yamllint are run by default; optionally,
  also stylelint (CSS), hadolint (Dockerfiles), eslint (JSON), and luacheck can
  be run.
- `releasetracker.yml`: wraps [*bewuethr/release-tracker-action*][rt] and takes
  the same parameters as the action (but with modified defaults)

[atp]: <https://github.com/actions/add-to-project>
[sl]: <https://github.com/github/super-linter>
[rt]: <https://github.com/bewuethr/release-tracker-action>
