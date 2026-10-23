# Dados

| Arquivo | Descrição | Como é gerado |
|---|---|---|
| `precos_ajustados.csv` | Preços diários de fechamento ajustados (dividendos e desdobramentos) de PETR4, VALE3, ITUB4 e BOVA11, dos últimos 5 anos | Gerado automaticamente ao rodar o notebook pela primeira vez (fonte: Yahoo Finance via `yfinance`) |
| `resumo_metricas.csv` | Tabela final com retorno, volatilidade, Sharpe, drawdown, correlação e beta | Gerado na última célula do notebook |

Se `precos_ajustados.csv` já existir, o notebook usa o arquivo salvo em vez de baixar de novo.
Assim os resultados ficam reproduzíveis, mesmo que o Yahoo Finance mude os dados depois.
Para atualizar a análise, apague o CSV e rode o notebook novamente.
