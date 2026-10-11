# Stoic Browser Releases

This repository hosts the installers and update manifests for [Stoic Browser](https://stoicbrowser.com), the command center browser for founders who run several products at once.

## About Stoic Browser

**One browser. Every product. Every dashboard.**

Stoic Browser gives each product its own workspace with isolated logins, tabs, pinned dashboards and metrics, then adds the tools a founder reaches for every day:

| Feature | Description |
|---------|-------------|
| **Workspaces** | One workspace per product, each with its own session, so accounts never bleed into each other |
| **Split panes** | Two pages, a dashboard or an automation side by side in one window |
| **Metrics dashboard** | Pulls numbers from the dashboards you already use and keeps a history |
| **Daily digest** | A summary of what changed across every workspace since yesterday |
| **Automation harness** | Record steps, add variables and schedules, and let runs happen unattended |
| **Agent chat** | Drive Claude Code, Codex, OpenCode and other local coding CLIs with browser tools over MCP |
| **MCP access** | Expose the browser to external MCP clients such as Claude Code, Cursor and Claude Desktop, with per-connection scopes |
| **Reader, dark mode and media controls** | Browser-native comforts without extensions |

## Downloads

Grab the latest installer from the [Releases](https://github.com/stoicsoft/stoicbrowser-releases/releases/latest) page.

| Platform | File |
|----------|------|
| macOS (Apple Silicon) | `Stoic-Browser-{version}-mac-arm64.dmg` |
| macOS (Intel) | `Stoic-Browser-{version}-mac-x64.dmg` |
| Windows installer | `Stoic-Browser-{version}-windows-setup.exe` |
| Windows portable | `Stoic-Browser-{version}-windows-portable.exe` |
| Linux AppImage | `Stoic-Browser-{version}-linux-x86_64.AppImage` |
| Linux Debian / Ubuntu | `Stoic-Browser-{version}-linux-amd64.deb` |

## Auto-updates

Stoic Browser checks this repository for a newer version a few seconds after launch and every six hours after that, using [electron-updater](https://www.electron.build/auto-update). When one is available you see a pill in the window; Settings → Updates shows the release notes, downloads the update and restarts into it. Auto-download, install-on-quit and the check interval are all settings, and any version can be skipped.

Every release carries the manifests the updater reads:

```
latest-mac.yml        macOS (x64 and arm64, updated through the .zip)
latest.yml            Windows (NSIS installer)
latest-linux.yml      Linux (AppImage and deb)
```

The Windows portable build does not update itself.

## Verifying downloads

- **macOS**: signed with a Developer ID certificate and notarized by Apple.
- **Windows**: not yet code-signed. SmartScreen may warn the first time; choose "More info" → "Run anyway".
- **Linux**: SHA512 checksums for every file are in the `latest*.yml` manifests.

## System requirements

| Platform | Minimum |
|----------|---------|
| macOS | 11 Big Sur or later |
| Windows | Windows 10 or later |
| Linux | Ubuntu 20.04, Debian 11 or equivalent |

## License

Stoic Browser is proprietary software with a free plan and a one-time Pro purchase.

- **Free**: a capped number of workspaces, external sources and automations.
- **Pro**: every cap removed, paid once, with 12 months of updates. From $29 for one device.

## Support

- **Issues**: [GitHub Issues](https://github.com/stoicsoft/stoicbrowser-releases/issues)
- **Email**: hello@stoicsoft.com

## Links

- [Website](https://stoicbrowser.com)
- [StoicSoft](https://stoicsoft.com)

---

Built by [StoicSoft](https://stoicsoft.com)
