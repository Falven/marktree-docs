# Change Log

All notable changes to the "marktree" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [0.8.5] - 2026-01-29

Consolidate problem-copy commands into a quick-pick selector.

## [0.8.4] - 2026-01-22

Consolidate "Copy Tab(s) as Markdown" commands.

## [0.8.3] - 2025-12-19

- Rename “Copy Active File as Markdown” to “Copy Active Tab as Markdown” and handle diffs within tab copy flows.

## [0.8.2] - 2025-12-19

- Updated CHANGELOG.md.

## [0.8.1] - 2025-12-19

- Fix multi-cursor selection headers by labeling each selected line range instead of collapsing to a single span.

## [0.8.0] - 2025-12-15

- Add a quick-pick scope selector for “Copy Tabs as Markdown” (all/left/right of the active tab).
- Add structured copy-worker logging with configurable log level and log path settings.
- Improve Copilot Proxy request normalization, tool handling, and streaming output for Anthropic/OpenAI routes.
- Package docs assets in published artifacts and streamline build/pack scripts.

## [0.7.5] - 2025-12-10

- Add “Copy Active Diff as Markdown” with quick-pick to copy merged changes, added-only, or removed-only lines from the active diff editor.

## [0.7.5] - 2025-12-10

- Run the Copilot proxy in its own high-performance external process for better responsiveness.

## [0.7.4] - 2025-12-10

- Add Copilot proxy start/stop/show commands, settings, and docs for 0.7.4.

## [0.7.3] - 2025-12-08

- Refresh docs submodule and version metadata for the 0.7.3 release.

## [0.7.2] - 2025-12-08

- Publish the 0.7.2 patch release.

## [0.7.1] - 2025-12-08

- Update docs submodule and package metadata for 0.7.1.

## [0.7.0] - 2025-12-08

- Add an option to include file paths in Markdown copy output.

## [0.6.6] - 2025-12-07

- Skip binary files when `ignoreBinary` is enabled by detecting binaries with `isbinaryfile`.

## [0.6.5] - 2025-12-06

- Add tokenizer selection and chunk size prompts for chunking flows.

## [0.6.4] - 2025-12-06

- Add a live token counter with OpenRouter model caching.

## [0.6.3] - 2025-12-05

- Bump version to repair documentation packaging for 0.6.3.

## [0.6.2] - 2025-12-04

- Add Pro model-based chunking and refresh the documentation.

## [0.6.1] - 2025-05-30

- Number selected lines, trim trailing blanks, and expose the selected-lines copy in the context menu.

## [0.6.0] - 2025-05-22

- Rewrite the tree parser with explicit root paths and flexible comments.

## [0.5.9] - 2025-05-16

- Add a license to the distribution.

## [0.5.8] - 2025-05-06

- Keep build artifacts at the repo root while ignoring them in git.

## [0.5.7] - 2025-05-06

- Keep generated artifacts in `dist/` for packaging.

## [0.5.6] - 2025-05-06

- Fix fallback root handling.

## [0.5.5] - 2025-05-06

- Package Clipboardy fallback binaries for Windows.

## [0.5.4] - 2025-04-30

- Respect user notification settings in the copy-selected terminal flow.

## [0.5.3] - 2025-04-26

- Fix importing VS Code from the worker.

## [0.5.2] - 2025-04-25

- Fix bundle output issues.

## [0.5.1] - 2025-04-25

- Add a “Copy All Problems” command and densify diagnostics output.

## [0.5.0] - 2025-04-24

- Correct `.gitignore` filtering in the scanner in preparation for 0.5.0.

## [0.4.9] - 2025-04-22

- Add a Pro feature to scaffold workspace structures from a clipboard tree.

## [0.4.8] - 2025-04-17

- Update the README.

## [0.4.7] - 2025-04-17

- Add privacy policy content for this release.

## [0.4.5] - 2025-04-16

- Release housekeeping and version bump to 0.4.5.

## [0.4.4] - 2025-04-16

- Update the README.

## [0.4.3] - 2025-04-16

- Add “Copy as Markdown” for terminal selection and refactor Markdown code block generation.

## [0.4.2] - 2025-04-16

- Redo the 0.4.2 release packaging.

## [0.3.9] - 2025-04-14

- Migrate the build from TSC to tsup, refresh extension configs, and remove LICENSE.

## [0.3.8] - 2025-04-09

- Add a “Copy Symbol” command and document the feature.

## [0.3.6] - 2025-03-27

- Add a “Copy Selected as Markdown” command and document/register it.

## [0.3.5] - 2025-03-21

- Fix package availability in the worker.

## [0.3.4] - 2025-03-20

- Add a “Copy Problems from Active File” command.

## [0.3.3] - 2025-03-20

- Improve command error handling with top-level try/catch and add a `vscode-uri` utility.
- Update ESLint packages and refactor copy/worker code paths.

## [0.3.2] - 2025-03-20

- Refactor scanning to gather ignores from the workspace root and simplify path handling.

## [0.3.1] - 2025-03-20

- Start partial tree scans at the workspace root and prefix Markdown paths with the workspace name.

## [0.3.0] - 2025-03-19

- Use the active workspace folder for paths and prepend the workspace name to outputs.

## [0.2.9] - 2025-03-19

- Make Markdown paths relative to the workspace root.

## [0.2.8] - 2025-03-19

- Rename the Git commits flow to a unified `copyGitCommits` command.

## [0.2.7] - 2025-03-19

- Handle empty multi-selection in “Copy Md Tree & Files.”

## [0.2.6] - 2025-03-19

- Add “Copy Git Diffs for Selected Commits” and fix a `shellCommands` typing issue.

## [0.2.5] - 2025-03-17

- Recursively copy directories in “Copy Files” and default to the workspace when none are selected.

## [0.2.4] - 2025-03-16

- Refactor the `copyActiveFileMd` command.

## [0.2.3] - 2025-03-16

- Add multi-selection support across copy commands and improve ignore updates.
- Treat Git diff ranges as inclusive and clarify related messaging.
- Improve ignore editing feedback and general error handling.

## [0.2.2] - 2025-02-27

- Add commands to view Git diff ranges.

## [0.2.1] - 2025-02-26

- Implement copying staged Git changes as Markdown.

## [0.2.0] - 2024-12-15

- Differentiate copy logic between the context menu and command palette.

## [0.1.9] - 2024-12-14

- Fix an unclosed code block in the README.

## [0.1.8] - 2024-12-14

- Add copy tabs functionality.

## [0.1.7] - 2024-12-14

- Add the ability to copy open tabs as Markdown.

## [0.1.6] - 2024-12-13

- Add quick add/remove controls for Markdown ignores.

## [0.1.5] - 2024-12-13

- Add `copyActiveFileMd` and expand default ignores.

## [0.1.4] - 2024-12-09

- Bug fixes and expanded error logging.

## [0.1.3] - 2024-12-09

- Add defaults to configuration.

## [0.1.2] - 2024-12-09

- Update the default ignore list.

## [0.1.1] - 2024-12-09

- Default command paths to the workspace root instead of erroring.

## [0.1.0] - 2024-12-09

- Add command categories.

## [0.0.9] - 2024-12-09

- Fix the single selection case.

## [0.0.8] - 2024-12-08

- Fix handling of `additionalIgnores`.

## [0.0.7] - 2024-12-08

- Fix informational message handling.

## [0.0.6] - 2024-12-08

- Add lockfiles to the default ignore list.

## [0.0.5] - 2024-12-08

- Fix a bug with copied messages.

## [0.0.4] - 2024-12-08

- Add settings for informational messages.

## [0.0.3] - 2024-12-08

- Use worker threads, improve recursion, and add binary ignore plus extension-scoped gitignores.

## [0.0.1] - 2024-12-06

- Initial release.
