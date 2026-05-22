# ATL Terminal v1.0.1 Public Preview

Released: 2026-05-22

## Downloads

- `ATL-Terminal-Setup.exe`
- `SHA256SUMS.txt`

## SHA256

```text
CF9363F98FEFF352AE2B2B7A75E9BF1CC27060B43814DFA94E96EC16A7B0287C  ATL-Terminal-Setup.exe
```

## Highlights

- Protected Windows build for public preview.
- Windows 10 and Windows 11 installer build.
- Bundled Perl runtime, so users do not need to install Perl separately.
- SSH, Telnet, SFTP file transfer, LLM chat/control, ATL Brain memory, and Plugin Center.
- Default LLM model is `gpt-5.4-mini`, with no API key bundled.
- TUI helper status is shown in Plugin Center: nano is marked unstable, Vim is marked beta.

## Privacy

The release package is built with clean sample settings. It excludes private API
keys, app state, crash logs, brain sessions, and plain first-party source.

## Known Preview Notes

- Nano automation is intentionally marked unstable.
- Vim automation should use deterministic `VIM_*` helper actions instead of raw
  cursor/edit-key recipes.
- Some antivirus or SmartScreen systems may warn on a new unsigned installer.
  Verify the official checksum before running it.
