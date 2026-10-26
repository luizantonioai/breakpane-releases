# Breakpane

**Real phone, tablet and laptop frames floating over your code, with an MCP server your coding agent can drive.**

Breakpane is a desktop app for Mac and Windows that shows your site or web app on iPhones, Androids, iPads, laptops and a desktop monitor, each with its real viewport, pixel ratio, user agent, touch and safe areas, always on top of your editor while you code. It finds your local dev servers and reloads with them.

**Website, pricing and download:** [breakpane.com](https://breakpane.com/en) · [Breakpane for coding agents](https://breakpane.com/en/agents)

This repository only holds the installers and release notes. The app checks it for updates.

## Install

- **Mac (Apple silicon):** download the `.dmg` from the [latest release](https://github.com/luizantonioai/breakpane-releases/releases/latest), open it and drag Breakpane to Applications. On first launch macOS may ask for confirmation: steps at [breakpane.com/en/#download](https://breakpane.com/en/#download).
- **Windows 10 and 11:** get it from the [Microsoft Store](https://apps.microsoft.com/detail/9MZSGPJM8Z1N?mode=direct), or download `Breakpane-Setup-….exe` from the latest release.

The first 14 days are free, no card. Then a monthly or yearly subscription: [breakpane.com/en/pricing](https://breakpane.com/en/pricing).

## MCP server for coding agents (Beta)

Breakpane has a built-in MCP server (Streamable HTTP, local only at `http://127.0.0.1:47821/mcp`, one key per client). Claude Code, Codex, Cursor, VS Code, Windsurf and Claude Desktop can open your page on real device frames, tap, type, scroll and audit it while you watch.

| Tool | What it does |
|---|---|
| `list_devices` | Device catalog, open devices and local dev servers |
| `open` | Open a URL on several devices side by side |
| `close` | Close the agent's devices |
| `configure` | Change model, orientation, dark mode or installed-app mode |
| `arrange` | Arrange devices side by side at one scale |
| `navigate` | Go to a URL, back, forward or reload |
| `snapshot` | Accessibility outline with element refs |
| `tap` | Tap with real touch events on phones, clicks on laptops |
| `type` | Type text or press a key |
| `scroll` | Touch scroll on phones, wheel on laptops |
| `wait_for` | Wait for text, a selector, a URL or idle |
| `screenshot` | Viewport screenshots or one combined sheet |
| `get_logs` | Console errors and failed network requests |
| `audit` | Responsive audit: overflow, notch and home indicator, small or covered tap targets, clipped text, broken images, errors, PWA. Numbered findings, an annotated image and an HTML report |

Prompts: `test_site`, `fix_until_clean`, `test_flow`.

The agent only acts on the devices it opened, in a separate browser profile, and you can take over any of them with one click. Every session leaves a diary with numbered screenshots.

**Setup:** turn on Coding agents (the plug button on the device rail), click **Connect** next to your agent, then ask in a new chat: *"Use the breakpane MCP server to open http://localhost:5173 on an iPhone and an Android and audit it."*

## Verify the download

Each release includes `SHA256SUMS.txt` with the checksum of every installer. Compare with:

- Mac: `shasum -a 256 Breakpane-<version>-arm64.dmg`
- Windows: `certutil -hashfile Breakpane-Setup-<version>.exe SHA256`

## Support

[support@breakpane.com](mailto:support@breakpane.com)

---

## Em português

O **Breakpane** é um app para Mac e Windows que mostra o seu site ou app web em iPhones, Androids, iPads, notebooks e monitores, com as medidas reais de cada tela, flutuando na frente do editor enquanto você programa. Tem um servidor MCP embutido para agentes de código testarem a página nesses aparelhos.

- **Site, preços e download:** [breakpane.com](https://breakpane.com) · [Agentes de código](https://breakpane.com/agentes)
- **Mac:** baixe o `.dmg` da [versão mais recente](https://github.com/luizantonioai/breakpane-releases/releases/latest). Passo a passo da primeira abertura em [breakpane.com/#download](https://breakpane.com/#download).
- **Windows:** pela [Microsoft Store](https://apps.microsoft.com/detail/9MZSGPJM8Z1N?mode=direct) ou pelo `.exe` da versão mais recente.
- 14 dias grátis, sem cartão. Depois, assinatura mensal ou anual em [breakpane.com/precos](https://breakpane.com/precos).

© SFAL Solutions Ltda. All rights reserved.
