# Dashboard Cripto

Dashboard estático (HTML/CSS/JS, sem backend) para acompanhar o dossiê cripto diário: preço do BTC, KPIs (funding, Fear & Greed, fluxo de ETF), viés do dia (long/short/neutro) e o dossiê completo em Markdown, navegável por data.

## Demo

https://wonderboat-ai.github.io/dashboard-cripto/

## Como funciona

- Página única (`index.html`), sem dependência de build ou servidor.
- Os dados ficam salvos no `localStorage` do próprio navegador — nada é enviado para fora.
- **Salvar dossiê do dia** registra preço, viés, funding, Fear & Greed, fluxo de ETF e o texto completo do dossiê (Markdown simplificado: `##` para seções, tabelas `|...|`, `> ` para citação, `**negrito**`, links `[texto](url)`).
- **Exportar/Importar** fazem backup e restauração do histórico em JSON.
- O tema visual muda automaticamente conforme o viés do dia selecionado: verde (long), amarelo (neutro), vermelho (short). A cor de destaque, as silhuetas decorativas do fundo (símbolo do Bitcoin, diamante do Ethereum, moedas, candlesticks e hexágonos) e as cores do gráfico de preço acompanham o mesmo viés — no gráfico, cada ponto do histórico é colorido pelo viés do próprio dia.
- Se o CDN do Chart.js estiver inacessível, o dashboard segue funcional — apenas o gráfico deixa de ser exibido.

## Stack

HTML + CSS + JavaScript vanilla. Gráfico via [Chart.js](https://www.chartjs.org/) (CDN).

## Uso local

Baixe o repositório e abra `index.html` diretamente no navegador.

---

WonderHUB.AI
