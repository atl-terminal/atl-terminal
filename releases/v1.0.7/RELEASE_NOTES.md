# ATL Terminal v1.0.7

Released: 2026-09-18

A smoother terminal workspace with detachable chat, clearer command presentation,
and stronger safeguards for multi-session troubleshooting.

## Downloads

- **ATL-Terminal-Setup.exe**: Windows x64 installer with the bundled runtime.
- **SHA256SUMS.txt**: checksums for the installer and release metadata.
- **release.json**: version, platform, download URL, and installer checksum.

No separate Perl installation is required. GitHub's source archives contain the
public release repository, not the application or its private core.

## What's New

- **Detachable, resizable chat.** Move chat into its own window or drag the divider
  to adjust its width. Drafts, selections, conversation history, and pending
  responses survive docking. Closing the detached window returns chat to the
  main workspace.
- **Cleaner chat presentation.** Explanations use a white background; commands and
  internal notices appear in dark snippets with syntax coloring. The docked chat
  and terminal align at the top, and detached window borders match the panel.
- **More responsive terminal input.** Reduced work on the input path, incremental
  native viewport snapshots, on-demand history generation, and batched native
  row serialization reduce repeated processing.
- **Output resilience.** Improvements cover resize handling, malformed input,
  large output bursts, and long lines, with regression checks for Unicode,
  colors, attributes, and multiple terminal panes.
- **Bounded code inspection.** Helpers prefer ripgrep with a bounded Perl fallback
  where supported, and limit file sizes, output, and scan duration. File-editing
  helpers use explicit actions and fingerprint checks instead of raw editor input.
- **Safer session flow.** Automatic follow-ups stay tied to their original
  connection. Responses do not execute after the active session or Chat/Control
  mode changes. Clearing chat cancels pending work and discards late replies.
- **Useful failure feedback.** Invalid helper blocks are rejected without shell
  fallback, and the model receives format guidance on the following turn.

## Installation And Upgrade

Close ATL Terminal before running the installer. Version 1.0.7 installs as
**ATL Terminal** and updates the normal ATL Terminal installation. Existing
connection and model settings are retained. A fresh installation includes only
sample connections and no API key, saved password, private key, chat history,
or memory database.

An earlier separate preview installation is not automatically migrated. Chat is
still one shared conversation; the detached title identifies the active terminal.
Independent per-session conversation histories are not part of this release.

## Preview Notes

- Nano automation remains **unstable**; Vim automation remains **beta**. Prefer
  deterministic helper actions for editing, and review important changes.
- The installer is unsigned. Windows may show a SmartScreen warning; verify the
  checksum against this official release before running it.
- Automated source and bundled-runtime checks have passed on the development
  Windows machine. Clean Windows 10 and Windows 11 VM validation remains pending.

Report reproducible issues with the app version, Windows version, and steps to
reproduce. Remove credentials and private terminal output before sharing logs
or screenshots.
