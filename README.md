# Dashboard Cripto

**Versão atual: v1.4.0** · Criado por **Wonder BOAT | WonderHUB.AI**

Dashboard estático (HTML/CSS/JS, sem backend) para acompanhar o dossiê cripto diário: preço do BTC, KPIs (funding, Fear & Greed, fluxo de ETF), viés do dia (long/short/neutro) e o dossiê completo em Markdown, navegável por data.

## Demo

https://wonderboat-ai.github.io/dashboard-cripto/

## Como funciona

- Página única (`index.html`), sem dependência de build ou servidor.
- Os dados ficam salvos no `localStorage` do próprio navegador — nada é enviado para fora.
- **Salvar dossiê do dia** registra preço, viés, funding, Fear & Greed, fluxo de ETF e o texto completo do dossiê (Markdown simplificado: `##` para seções, tabelas `|...|`, `> ` para citação, `**negrito**`, links `[texto](url)`).
- **Exportar/Importar** fazem backup e restauração do histórico em JSON.
- O tema visual muda automaticamente conforme o viés do dia selecionado: verde (long), amarelo (neutro), vermelho (short). A cor de destaque e as silhuetas decorativas do fundo (símbolo do Bitcoin, diamante do Ethereum, moedas, candlesticks e hexágonos) acompanham o mesmo viés.
- O gráfico é o widget [Advanced Chart do TradingView](https://www.tradingview.com/widget/advanced-chart/) ao vivo (BYBIT:BTCUSDT por padrão, com troca de símbolo habilitada). Sem internet, o dashboard segue funcional — apenas o gráfico deixa de carregar.

## Stack

HTML + CSS + JavaScript vanilla. Gráfico ao vivo via widget embed do [TradingView](https://www.tradingview.com/).

## Uso local

Baixe o repositório e abra `index.html` diretamente no navegador.

## Histórico de versões

| Versão | Data | Mudanças |
|---|---|---|
| v1.4.0 | 2026-08-24 | Gráfico Chart.js substituído pelo widget Advanced Chart do TradingView ao vivo (BYBIT:BTCUSDT, tema dark integrado). |
| v1.3.0 | 2026-08-24 | Rodapé institucional (Wonder BOAT \| WonderHUB.AI) e versionamento visível no app (`APP_VERSION`). |
| v1.2.1 | 2026-07-23 | Silhuetas de criptomoedas no fundo (₿, Ξ, moeda), candles mais sutis e tolerância a falha do CDN do Chart.js. |
| v1.2.0 | 2026-07-23 | Tema reativo ao viés do dia (long/short/neutro): cor de destaque, decoração de fundo e gráfico colorido por viés. |
| v1.1.0 | 2026-07-23 | Tema dark verde-neon (textura de grão, glow, cards escuros). |
| v1.0.0 | 2026-06 | Dashboard original (tema claro), dossiê por data com KPIs, gráfico e import/export JSON. |

---

**Wonder BOAT | WonderHUB.AI**
