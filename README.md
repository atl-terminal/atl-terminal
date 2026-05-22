# ATL Terminal

ATL Terminal is a Windows SSH/Telnet terminal for network engineers, system
administrators, DevOps, and security teams who live inside remote shells,
routers, jump boxes, logs, configs, and troubleshooting sessions.

It combines a practical terminal workspace with optional LLM assistance,
session awareness, file transfer, memory, and plugin-based helpers for devices,
tools, TUI programs, and code inspection.

## Public Preview

Latest public preview: `v1.0.1`

Download from the GitHub Releases page:

- `ATL-Terminal-Portable.zip`
- `ATL-Terminal-Setup.exe`
- `SHA256SUMS.txt`
- `RELEASE_NOTES.md`

## Highlights

- Multi-session SSH and Telnet terminal
- LLM chat and control modes for troubleshooting
- OpenAI-compatible local model support
- SFTP file transfer
- Session awareness and memory
- Plugin Center for device, tool, TUI, and code helpers
- Cisco IOS, Linux, Nmap, Vim, nano, and code-inspection plugin examples
- Portable ZIP and Windows installer
- Windows 10 and Windows 11 support

## Verify Downloads

Always verify downloads before installing or extracting.

```powershell
Get-FileHash ".\ATL-Terminal-Portable.zip" -Algorithm SHA256
Get-FileHash ".\ATL-Terminal-Setup.exe" -Algorithm SHA256
```

Compare the output with:

```text
289EE069C0DA8BB261EF2EE2DBFA0A9F7346BAD34B3DE555E81CFACFE61EEF5A  ATL-Terminal-Portable.zip
CF9363F98FEFF352AE2B2B7A75E9BF1CC27060B43814DFA94E96EC16A7B0287C  ATL-Terminal-Setup.exe
```

## Preview Notes

This is an early public preview. Feedback is welcome, especially from people
using SSH, Telnet, Cisco/Linux devices, SFTP transfer, local LLM endpoints, and
Plugin Center workflows in real troubleshooting environments.

Known preview status:

- Nano automation is marked unstable.
- Vim automation is beta and should use deterministic helper actions.
- New unsigned installers may trigger SmartScreen or antivirus warnings.

## Public Repositories

- Documentation: https://github.com/atl-terminal/atl-terminal-docs
- Plugin SDK: https://github.com/atl-terminal/atl-terminal-plugin-sdk
- Curated plugins: https://github.com/atl-terminal/atl-terminal-plugins

## Security

Please report security-sensitive issues privately. See [SECURITY.md](SECURITY.md).
