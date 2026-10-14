# Breakpane

Instaladores do **Breakpane**, o app para Mac e Windows que mostra o seu site ou app web em iPhones, Androids, iPads, notebooks e monitores, com as medidas reais de cada tela, flutuando na frente do editor enquanto você programa.

**Site, preços e download:** [breakpane.com](https://breakpane.com)

Este repositório guarda só os instaladores e as notas de cada versão. O app procura atualizações aqui.

## Instalar

- **Mac (chip Apple):** baixe o `.dmg` da [versão mais recente](https://github.com/luizantonioai/breakpane-releases/releases/latest), abra e arraste o Breakpane para Aplicativos. Na primeira abertura, o macOS pode pedir confirmação: o passo a passo está em [breakpane.com/#download](https://breakpane.com/#download).
- **Windows 10 e 11 (64 bits):** baixe o `Breakpane-Setup-….exe` e execute.

Os 14 primeiros dias são grátis, sem cartão. Depois, assinatura mensal ou anual em [breakpane.com/precos](https://breakpane.com/precos).

## Conferir o arquivo

Cada versão traz o arquivo `SHA256SUMS.txt` com a soma de verificação de cada instalador. Compare com:

- Mac: `shasum -a 256 Breakpane-<versão>-arm64.dmg`
- Windows: `certutil -hashfile Breakpane-Setup-<versão>.exe SHA256`

## Suporte

[support@breakpane.com](mailto:support@breakpane.com)

© SFAL Solutions Ltda. Todos os direitos reservados.
