# SOL Commander

One product for ChatGPT and an authorized Windows PC. You install **one Windows Setup EXE** per PC; the ChatGPT plugin is a separate connected software component, not another Windows installer.

## Current public Windows download

**Current default public Windows download: v0.1.6** (Cloudflare stable channel; GitHub currently labels this release a Beta/prerelease).

[Download SOL Commander for Windows (Setup EXE)](https://github.com/serwansergo-sudo/sol-commander-releases/releases/download/v0.1.6/SOL-Commander-Setup-v0.1.6.exe)

- File: `SOL-Commander-Setup-v0.1.6.exe`
- Size: `49,567,744` bytes
- SHA-256: `4852f8eacb847e2ab756cf882a6c95ee74b2596059579e20ae434dd4aedb92d4`
- Official product website: https://sol-commander-public-core.serwanboba.workers.dev/

For the stable experience, download from the verified link above. Follow the Windows installer prompts and review Windows security warnings. SOL requires explicit local permissions and an authorized pairing before it can work with your computer.

## Public beta v0.1.7 — independently tested, still unsigned

[View v0.1.7 Beta release and setup download](https://github.com/serwansergo-sudo/sol-commander-releases/releases/tag/v0.1.7)

- Windows beta Setup: `SOL-Commander-Setup-v0.1.7.exe` — 49,583,616 bytes, SHA-256 `16c3f87a09a6d7f39dbe717e648f76fc275a4f62856d61e9b02ef844a9364bba`.
- GitHub Actions independently verified exact Setup SHA-256, clean installation/uninstallation, upgrade from v0.1.6, and preservation of synthetic user data on disposable Windows Server 2022: [PASS report](https://github.com/serwansergo-sudo/sol-commander-releases/actions/runs/42020532912).
- **Beta only, unsigned.** Windows security warnings may appear. Do not disable security protections. Automatic updates are NOT enabled for this beta. It is not the recommended stable download.
- Publishing the Windows beta does not publish the OpenAI ChatGPT directory plugin or switch Cloudflare's existing public site.

## Release channels and version numbers

| Component | Version/status | Meaning |
| --- | --- | --- |
| Default public Windows Setup | `0.1.6` | Configured via Cloudflare stable channel; GitHub release itself is marked Beta |
| Windows beta installer | `0.1.7` — unsigned prerelease | Published beta; isolated installation/upgrade PASS; not stable auto-update |
| Private ChatGPT development plugin | `1.0.9` | Plugin package version, not the Windows Agent version |
| Public ChatGPT plugin | Not submitted or published | A separate review and approval process |

The different version numbers are intentional: ChatGPT plugin package, Windows Agent and hosted MCP tools evolve independently. They remain **one SOL Commander product**. Installing a separate ZIP or developer plugin is not necessary for a normal Windows user.

## Updates

The Windows updater checks the public stable release metadata and independently verifies installer size, SHA-256, trusted Authenticode signature and a pinned publisher certificate before installing an update. Until trusted signing is configured, unsigned beta installers **cannot be installed automatically** by that updater.

After a ChatGPT plugin is published, its hosted MCP tools can be rescanned and made available to users following OpenAI's validation. Package metadata and bundled skill updates still require a plugin package update.

The GitHub `v0.1.7` release is an **explicitly labeled public prerelease** with current verified beta candidate bytes. The default public download remains v0.1.6. Both existing GitHub release records are currently marked prerelease, so GitHub's `/releases/latest` full-release endpoint does not yet resolve.

For issues or feature requests: https://github.com/serwansergo-sudo/sol-commander-releases/issues
