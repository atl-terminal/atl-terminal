# ATL Terminal

ATL Terminal is an AI-assisted SSH/Telnet terminal and PuTTY alternative for
Windows, built for network engineers, system administrators, DevOps, and
security teams who live inside remote shells, routers, jump boxes, logs,
configs, and troubleshooting sessions.

It combines a practical terminal workspace with optional LLM assistance,
session awareness, file transfer, memory, and plugin-based helpers for devices,
tools, TUI programs, and code inspection.

Use it when you want a Windows terminal for SSH, Telnet, Cisco/Linux operations,
SFTP transfer, local or OpenAI-compatible LLM chat, and safer command planning in
real troubleshooting sessions.

## Public Preview

**Latest version: [v1.0.7](https://github.com/atl-terminal/atl-terminal/releases/tag/v1.0.7)**

[Download ATL Terminal for Windows](https://github.com/atl-terminal/atl-terminal/releases/download/v1.0.7/ATL-Terminal-Setup.exe)

This public preview installs as **ATL Terminal** and updates an existing ATL
Terminal installation. Close the app before upgrading. Existing connection and
model settings are retained; a new installation starts with clean sample settings.
An earlier separate preview installation is not automatically migrated.

Version 1.0.7 improves native terminal responsiveness, strengthens handling of
large and malformed output, and adds detachable, resizable chat. Chat explanations
stay on white while commands use dark, syntax-colored snippets. Automatic
follow-ups are tied to their original session, and clearing chat cancels pending work.
See the [release notes](releases/v1.0.7/RELEASE_NOTES.md).

Earlier versions remain available on the [Releases page](https://github.com/atl-terminal/atl-terminal/releases).

## Highlights

- Multi-session SSH and Telnet terminal
- LLM chat and control modes for troubleshooting
- Detachable chat window and adjustable chat width
- Native terminal rendering with on-demand scrollback processing
- OpenAI-compatible local model support for LM Studio, Ollama-style gateways,
  and compatible `/v1/chat/completions` endpoints
- SFTP file transfer
- Session awareness and memory
- Plugin Center for device, tool, TUI, and code helpers
- Cisco IOS, Linux, Nmap, Vim, nano, and code-inspection plugin examples
- Windows installer with bundled runtime
- Windows 10 and Windows 11 support

## Verify Downloads

Always verify downloads before installing.

```powershell
Get-FileHash ".\ATL-Terminal-Setup.exe" -Algorithm SHA256
```

Compare the output with [SHA256SUMS.txt for v1.0.7](releases/v1.0.7/SHA256SUMS.txt).

Release assets also include `SHA256SUMS.txt` and `release.json`. Verify against
the checksum for the exact version you downloaded, not a different release.

## Preview Notes

This is an early public preview. Feedback is welcome, especially from people
using SSH, Telnet, Cisco/Linux devices, SFTP transfer, local LLM endpoints, and
Plugin Center workflows in real troubleshooting environments.

Known preview status:

- Nano automation is marked unstable.
- Vim automation is beta and should use deterministic helper actions.
- New unsigned installers may trigger SmartScreen or antivirus warnings.
- Automated runtime, rendering, and session-flow checks have passed on the
  development Windows machine. Fresh Windows 10 and Windows 11 VM validation
  remains outstanding.

## Privacy and Source

The installer ships with sample connections and no bundled API key,
personal connection profiles, saved passwords, private keys, chat history, or
memory database. Configure your own connections and model provider after
installation. The default model remains `gpt-5.4-mini`.

This public repository hosts release information and downloads, not the private
application core. GitHub's automatically generated source archives contain this
repository's public files; they are not application installers. Plugin SDK,
plugin examples, and documentation are available in the repositories below.

## Feedback

[Report a bug](https://github.com/atl-terminal/atl-terminal/issues/new) with the
app version, Windows version, reproduction steps, and expected versus actual
behavior. Remove credentials, host details, and private terminal output from
screenshots or logs before sharing. Report sensitive issues privately using
[SECURITY.md](SECURITY.md).

## Search Keywords

SSH client, Telnet client, PuTTY alternative, AI terminal, LLM terminal
assistant, OpenAI-compatible terminal, local LLM terminal, SFTP client, Cisco
terminal, Linux admin, network troubleshooting, DevOps terminal, security
operations.

## Public Repositories

- Documentation: https://github.com/atl-terminal/atl-terminal-docs
- Plugin SDK: https://github.com/atl-terminal/atl-terminal-plugin-sdk
- Curated plugins: https://github.com/atl-terminal/atl-terminal-plugins

## Security

Please report security-sensitive issues privately. See [SECURITY.md](SECURITY.md).
