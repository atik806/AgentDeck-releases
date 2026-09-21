# AgentDeck — downloads

**AgentDeck** is a desktop panel for running several coding agents side by side —
multiple terminals in one window, isolated git worktrees per agent, plugins for
GitHub, Jira, Linear, Google Drive and more.

This repository hosts the **released builds and the auto-update feed** only.
The application source is private.

## Download

| Platform | File | How |
|---|---|---|
| Windows | `AgentDeck-win-Setup.exe` | Run it. Per-user install to `%LOCALAPPDATA%\AgentDeck` — no admin prompt. |
| Windows (no installer) | `AgentDeck-win-Portable.zip` | Unzip and run `AgentDeck.exe`. |
| Linux | `AgentDeck-Linux-Install.sh` | `bash AgentDeck-Linux-Install.sh` |

Grab the newest from **[Releases](https://github.com/atik806/AgentDeck-releases/releases/latest)**.

Once installed, AgentDeck updates itself — the Update button in the app reads
this repository's release feed.

## Verifying a download

Every release carries `SHA256SUMS.txt` (Windows) and `SHA256SUMS-linux.txt`.
Compare before running:

```powershell
Get-FileHash .\AgentDeck-win-Setup.exe -Algorithm SHA256
```

```bash
sha256sum AgentDeck-Linux-Install.sh
```

Windows builds are signed when the release pipeline has its signing
credentials; an unsigned build still installs, but SmartScreen will ask you to
choose **More info → Run anyway**.

## Links

- Website: <https://vibeflow.tech/agentdeck>
- Issues and feedback: <https://github.com/atik806/AgentDeck-releases/issues>
