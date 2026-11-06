# SOL Commander

One product for ChatGPT and an authorized Windows PC. You install **one Windows Setup EXE** per PC; the ChatGPT plugin is a separate connected software component, not another Windows installer.

## Быстрый старт SOL Commander (русский)

**Статус:** публичная тестовая версия Windows `0.1.8 Beta`. Плагин ещё не опубликован в каталоге ChatGPT. Сайт пока предлагает выпуск `0.1.6` с 32 инструментами PUBLIC_CORE. Автоматическое обновление неподписанных версий отключено.

1. Откройте [SOL Commander v0.1.8 Beta](https://github.com/serwansergo-sudo/sol-commander-releases/releases/tag/v0.1.8) и скачайте только `SOL-Commander-Setup-v0.1.8.exe`. ZIP и JSON не нужно устанавливать.
2. Проверяйте, что файл получен из данного GitHub-релиза. SHA-256 установщика: `93cd3ed77b03c7370b346e031d8cb187690544b5c876bdc54de94d70b6b22a6e`. Это неподписанная Beta: если Windows блокирует запуск, не отключайте защиту ради установки.
3. Если установка прошла без предупреждений, откройте SOL Commander и следуйте экранным инструкциям для подключения своей учётной записи и разрешённых папок. Плагин из общего каталога ChatGPT пока недоступен.
4. Для тестирования используйте только свои несекретные файлы. Не подключайте медицинские карты, платёжные данные, пароли, документы детей и иные чувствительные материалы. Защита чувствительного содержимого неполная.
5. Об ошибках сообщайте через [GitHub Issues](https://github.com/serwansergo-sudo/sol-commander-releases/issues), без персональных данных, логинов, паролей и токенов.

[Независимый тест установки, обновления и удаления v0.1.8 — PASS](https://github.com/serwansergo-sudo/sol-commander-releases/actions/runs/42130912126). Это не сертификат цифровой подписи и не подтверждение публикации плагина OpenAI.

## Current public Windows download

**Current default public Windows download: v0.1.6** (Cloudflare stable channel; GitHub currently labels this release a Beta/prerelease).

[Download SOL Commander for Windows (Setup EXE)](https://github.com/serwansergo-sudo/sol-commander-releases/releases/download/v0.1.6/SOL-Commander-Setup-v0.1.6.exe)

- File: `SOL-Commander-Setup-v0.1.6.exe`
- Size: `49,567,744` bytes
- SHA-256: `4852f8eacb847e2ab756cf882a6c95ee74b2596059579e20ae434dd4aedb92d4`
- Official product website: https://sol-commander-public-core.serwanboba.workers.dev/

For the stable experience, download from the verified link above. Follow the Windows installer prompts and review Windows security warnings. SOL requires explicit local permissions and an authorized pairing before it can work with your computer.

## Public beta v0.1.8 — independently tested, still unsigned

[View v0.1.8 Beta release and Windows Setup](https://github.com/serwansergo-sudo/sol-commander-releases/releases/tag/v0.1.8)

- Setup: `SOL-Commander-Setup-v0.1.8.exe` — 49,584,128 bytes, SHA-256 `93cd3ed77b03c7370b346e031d8cb187690544b5c876bdc54de94d70b6b22a6e`.
- Optional ZIP SHA-256: `6005ba47f53bddbb5cdfad566f1460ebce442e7f53cbc04f76e7e237c601674c`.
- [Independent Windows installation, v0.1.6 upgrade and data preservation — PASS](https://github.com/serwansergo-sudo/sol-commander-releases/actions/runs/42130912126). Exact SHA pinned; production owner PC unchanged.
- **Unsigned prerelease; do not disable Windows security to install it.** Automatic updates remain disabled. Not the default stable download.
- The public ChatGPT plugin is not in the directory; Cloudflare still exposes 32 tools despite 57 being prepared in source.

## Third-party license information for v0.1.8

[Independent immutable ZIP integrity and third-party inventory audit — PASS](https://github.com/serwansergo-sudo/sol-commander-releases/actions/runs/42195517638). The published v0.1.8 ZIP contains 33 npm runtime packages with declared license metadata. Two npm tarballs omitted an individual license-text file, so we provide the original upstream licenses here for review:

- [isarray 1.0.0 — MIT license, copyright Julian Gruber](https://github.com/juliangruber/isarray/blob/master/LICENSE)
- [@bazel/runfiles 6.5.0 — Apache License 2.0](https://github.com/bazel-contrib/rules_nodejs/blob/main/LICENSE)

The next version of the installer is being prepared to include standalone copies of these notices. Existing published v0.1.8 EXE/ZIP files remain immutable. This inventory is not a complete legal audit; bundled Node.js, geckodriver and other notices must remain available under their applicable licenses.

## Previous beta v0.1.7 — independently tested, still unsigned

[View v0.1.7 Beta release and setup download](https://github.com/serwansergo-sudo/sol-commander-releases/releases/tag/v0.1.7)

- Windows beta Setup: `SOL-Commander-Setup-v0.1.7.exe` — 49,583,616 bytes, SHA-256 `16c3f87a09a6d7f39dbe717e648f76fc275a4f62856d61e9b02ef844a9364bba`.
- GitHub Actions independently verified exact Setup SHA-256, clean installation/uninstallation, upgrade from v0.1.6, and preservation of synthetic user data on disposable Windows Server 2022: [PASS report](https://github.com/serwansergo-sudo/sol-commander-releases/actions/runs/42020532912).
- **Beta only, unsigned.** Windows security warnings may appear. Do not disable security protections. Automatic updates are NOT enabled for this beta. It is not the recommended stable download.
- Publishing the Windows beta does not publish the OpenAI ChatGPT directory plugin or switch Cloudflare's existing public site.

## Release channels and version numbers

| Component | Version/status | Meaning |
| --- | --- | --- |
| Default public Windows Setup | `0.1.6` | Configured via Cloudflare stable channel; GitHub release itself is marked Beta |
| Windows beta installer | `0.1.8` — unsigned prerelease | Published beta; isolated installation/upgrade PASS; not stable auto-update |
| Private ChatGPT development plugin | `1.0.9` | Plugin package version, not the Windows Agent version |
| Public ChatGPT plugin | Not submitted or published | A separate review and approval process |

The different version numbers are intentional: ChatGPT plugin package, Windows Agent and hosted MCP tools evolve independently. They remain **one SOL Commander product**. Installing a separate ZIP or developer plugin is not necessary for a normal Windows user.

## Updates

The Windows updater checks the public stable release metadata and independently verifies installer size, SHA-256, trusted Authenticode signature and a pinned publisher certificate before installing an update. Until trusted signing is configured, unsigned beta installers **cannot be installed automatically** by that updater.

After a ChatGPT plugin is published, its hosted MCP tools can be rescanned and made available to users following OpenAI's validation. Package metadata and bundled skill updates still require a plugin package update.

The GitHub `v0.1.8` release is the **newest public Windows prerelease**; earlier `v0.1.7` remains available. Both are independently tested but unsigned. The default public download remains v0.1.6. Both existing GitHub release records are currently marked prerelease, so GitHub's `/releases/latest` full-release endpoint does not yet resolve.

For issues or feature requests: https://github.com/serwansergo-sudo/sol-commander-releases/issues
