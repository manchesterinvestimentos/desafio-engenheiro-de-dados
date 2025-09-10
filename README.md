# Desafio para vaga de Engenheiro de Dados

Por favor leiam este documento do começo ao fim, com muita atenção, o intuito deste teste é avaliar seus conhecimentos técnicos.

Este desafio deve ser feito por você, gaste o tempo que você quiser, porém normalmente você não deve precisar de mais do que algumas horas para finalizá-lo.

# Instruções de entrega do desafio

1. Envie via email com a solução proposta para seu contato Manchester Investimentos com cópia para rh@manchesterinvest.com.br.

# Contexto

A Manchester Investimentos quer criar uma base consolidada de informações para analisar o desempenho de ativos da bolsa.
Hoje, os dados vêm de duas fontes:

Trades (execuções de ordens): CSV exportado da corretora, com colunas: trade_id, account, symbol, side, qty, price, trade_date.

Preços de Fechamento (EOD): CSV diário de mercado, com colunas: symbol, date, close_price.

O objetivo é estruturar um processo que integre essas fontes e gere informações de P&L realizado por conta e ativo.

## Parte 1 — Arquitetura

Desenhe (ou descreva em texto) uma arquitetura simples para resolver o problema:

Onde você armazenaria os dados brutos?
Como faria a ingestão e transformação?
Como garantiria qualidade mínima dos dados?
Como entregaria o resultado para o time de análise (ex.: arquivo, banco, dashboard)?
Como faria o monitoramento dos pipelines?

👉 A resposta pode ser em texto com bullets + (opcional) um diagrama simples.

## Parte 2 — Código (Python + Pandas)

Implemente um script em Python que:

Leia os dois arquivos CSV (trades.csv e prices.csv).

Limpe e normalize os dados (ex.: garantir que as datas estejam em formato datetime, que qty seja numérico positivo).

Calcule:
Preço médio de compra por ativo e conta.
P&L realizado nas vendas ((preço_venda - custo_médio) * quantidade_vendida).
Gere uma tabela final consolidada com colunas: account, symbol, position_final, avg_price, realized_pnl.

Salve a saída em um novo CSV (pnl_report.csv).

# Ferramentas:

1. O candidato deve usar seu próprio julgamento para selecionar as ferramentas e métodos mais adequados para o desafio.
2. O candidato deve fornecer documentação clara e concisa para a solução.
3. O candidato deve ser capaz de defender sua solução e as ferramentas propostas.

# Avaliação:

A solução do candidato será avaliada com base nos seguintes critérios:
1. Atende aos requisitos e especificações do desafio
2. É escalável e segura
3. É fácil de usar

# Boa sorte!
