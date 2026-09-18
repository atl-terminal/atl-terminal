# ATL Terminal v1.0.7-test.1

## Native Terminal Performance Preview

This prerelease focuses on terminal responsiveness during typing, scrolling,
resizing, and multi-session output. It installs as **ATL Terminal Test** alongside
the normal application, without replacing that installation or its settings.

### What's Improved

- **Less repeated screen processing.** The native terminal engine tracks changed
  rows and prepares the visible area without rebuilding the entire screen and
  scrollback on every update.
- **Faster text serialization.** Matching ASCII text is processed in runs while
  preserving the separate path for wide and combining Unicode characters.
- **On-demand history.** Full text remains available for copying, chat context,
  and viewer-only TV. Disconnected panes retain their scrollback for inspection.
- **Resize stability.** Includes a fix for an out-of-bounds access during native
  terminal resizing.

### Download and Install

Download `ATL-Terminal-1.0.7-test.1.exe`, verify its SHA256, and run the installer.
The Windows runtime is bundled; no separate Perl installation is required.
Open **ATL Terminal Test** from the Start Menu, not your existing ATL Terminal
shortcut. Add a test connection and configure your model provider as needed.

```text
AED83F87D59E597BC5C76EEC93E5CDF7130C32B2D5F85F4A54CA6AE6ABA7AD46  ATL-Terminal-1.0.7-test.1.exe
```

### Validation

Local verification passed 1,034 assertions across 37 regular test files,
45 GUI assertions, and 42 upstream libvterm conformance test files. Packaged
and installed runtime checks passed all 12 smoke assertions. Tests compare
text, Unicode widths, colors, attributes, and full versus incremental rendering.
Local synthetic workloads showed lower CPU usage; results vary by workload.

Fresh Windows 10 and Windows 11 VM testing remains outstanding. This is an
unsigned test release, not a production stability guarantee.

### What to Test

1. Type, backspace, use command history, and resize an SSH session.
2. Open and close top, nano, and Vim manually; check that the shell returns normally.
3. Use several terminal panes and scroll back while other panes receive output.
4. Copy selections and history, include terminal context in chat, and try viewer-only TV.
5. Disconnect, then scroll and copy from the disconnected pane.

### Privacy and Known Limitations

The package contains clean sample connections and no personal credentials,
API keys, chats, memory databases, or debug logs. The default model remains
`gpt-5.4-mini`. Existing settings are not copied into the test installation.

This release improves the terminal engine, not the model's editor-control
planning. Nano automation remains unstable; Vim automation remains beta.
Unsigned downloads may trigger SmartScreen or antivirus warnings.

Please report reproducible issues through
[GitHub Issues](https://github.com/atl-terminal/atl-terminal/issues), with private
details removed. Existing public preview downloads remain available.
