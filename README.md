# Dashboard Cripto

Dashboard estático (HTML/CSS/JS, sem backend) para acompanhar o dossiê cripto diário: preço do BTC, KPIs (funding, Fear & Greed, fluxo de ETF), viés do dia (long/short/neutro) e o dossiê completo em Markdown, navegável por data.

## Demo

https://wonderboat-ai.github.io/dashboard-cripto/

## Como funciona

- Página única (`index.html`), sem dependência de build ou servidor.
- Os dados ficam salvos no `localStorage` do próprio navegador — nada é enviado para fora.
- **Salvar dossiê do dia** registra preço, viés, funding, Fear & Greed, fluxo de ETF e o texto completo do dossiê (Markdown simplificado: `##` para seções, tabelas `|...|`, `> ` para citação, `**negrito**`, links `[texto](url)`).
- **Exportar/Importar** fazem backup e restauração do histórico em JSON.
- O tema visual (cor de destaque, elementos decorativos de fundo e as cores do gráfico de preço) muda automaticamente conforme o viés do dia selecionado: verde (long), amarelo (neutro), vermelho (short).

## Stack

HTML + CSS + JavaScript vanilla. Gráfico via [Chart.js](https://www.chartjs.org/) (CDN).

## Uso local

Baixe o repositório e abra `index.html` diretamente no navegador.

---

WonderHUB.AI
