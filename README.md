# SOL Commander

One product for ChatGPT and an authorized Windows PC. You install **one Windows Setup EXE** per PC; the ChatGPT plugin is a separate connected software component, not another Windows installer.

## Current public Windows download

**Stable public download: v0.1.6**

[Download SOL Commander for Windows (Setup EXE)](https://github.com/serwansergo-sudo/sol-commander-releases/releases/download/v0.1.6/SOL-Commander-Setup-v0.1.6.exe)

- File: `SOL-Commander-Setup-v0.1.6.exe`
- Size: `49,567,744` bytes
- SHA-256: `4852f8eacb847e2ab756cf882a6c95ee74b2596059579e20ae434dd4aedb92d4`
- Official product website: https://sol-commander-public-core.serwanboba.workers.dev/

Download only from the verified link above. Follow the Windows installer prompts and review Windows security warnings. SOL requires explicit local permissions and an authorized pairing before it can work with your computer.

## Release channels and version numbers

| Component | Version/status | Meaning |
| --- | --- | --- |
| Public Windows Setup | `0.1.6` | Current publicly available installer |
| New Windows Agent candidate | `0.1.7` — unsigned draft | Under verification; not a stable update |
| Private ChatGPT development plugin | `1.0.9` | Plugin package version, not the Windows Agent version |
| Public ChatGPT plugin | Not submitted or published | A separate review and approval process |

The different version numbers are intentional: ChatGPT plugin package, Windows Agent and hosted MCP tools evolve independently. They remain **one SOL Commander product**. Installing a separate ZIP or developer plugin is not necessary for a normal Windows user.

## Updates

The Windows updater checks the public stable release metadata and independently verifies installer size, SHA-256, trusted Authenticode signature and a pinned publisher certificate before installing an update. Until trusted signing is configured, unsigned beta installers **cannot be installed automatically** by that updater.

After a ChatGPT plugin is published, its hosted MCP tools can be rescanned and made available to users following OpenAI's validation. Package metadata and bundled skill updates still require a plugin package update.

The GitHub `v0.1.7` release is currently a **draft with older unsigned candidate files**. It must not be presented as the current public download.

For issues or feature requests: https://github.com/serwansergo-sudo/sol-commander-releases/issues
