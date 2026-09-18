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

**New performance test release: [v1.0.7-test.1](https://github.com/atl-terminal/atl-terminal/releases/tag/v1.0.7-test.1)**

[Download the Windows test installer](https://github.com/atl-terminal/atl-terminal/releases/download/v1.0.7-test.1/ATL-Terminal-1.0.7-test.1.exe)

This prerelease installs as **ATL Terminal Test**, alongside your existing ATL
Terminal installation. It does not replace that installation or copy its saved
connections, passwords, API keys, or chat history. Launch **ATL Terminal Test**
from the Start Menu to try the new native terminal performance improvements.

The build reduces repeated screen processing, creates scrollback text on demand,
and includes a native resize crash fix. Copying, chat context, and viewer-only
TV retain access to terminal text. See the [release notes and test checklist](releases/v1.0.7-test.1/RELEASE_NOTES.md).

[Previous public preview: v1.0.2](https://github.com/atl-terminal/atl-terminal/releases/tag/v1.0.2)
remains available. Both releases are previews, not stable releases.

## Highlights

- Multi-session SSH and Telnet terminal
- LLM chat and control modes for troubleshooting
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
Get-FileHash ".\ATL-Terminal-1.0.7-test.1.exe" -Algorithm SHA256
```

Compare the output with:

```text
AED83F87D59E597BC5C76EEC93E5CDF7130C32B2D5F85F4A54CA6AE6ABA7AD46  ATL-Terminal-1.0.7-test.1.exe
```

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
- The new test installer has passed local Windows installation and rendering
  checks. Fresh Windows 10 and Windows 11 VM testing remains outstanding.

## Privacy and Source

The test installer ships with sample connections and no bundled API key,
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
