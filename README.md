# Análise de Performance

Gestão de Desempenho das Equipes de Campo — dashboard de produtividade para técnicos de campo da Alloha Fibra.

## Funcionalidades

- **Dashboard** — KPIs (SLA, Meta, Média, Total OS, Total Pontos, Ticket Médio, Dias Úteis, Dias Produtivos, Em Alerta), cards individuais por técnico com média, quartil, SLA e sparkline, gráficos (evolução diária, tendência semanal, radar do perfil da equipe, distribuição por quartil) e projeção de fechamento do mês com gap analysis
- **Acompanhamento** — tabela diária de pontuação por técnico com suporte a justificativas (BH, DSR, FE, FR, AT, TR, LI, MV), bloqueio automático após importação de relatório, e tabela de meta diária da equipe
- **Parâmetros** — configuração de metas por dia da semana, limites de quartil, alertas, modo de ranking e janela de tendência

## Como usar

1. Abra o arquivo `Acompanhamento_Produtividade_v2 (10).html` no navegador
2. Cadastre técnicos na aba Acompanhamento
3. Lance a pontuação manualmente ou importe um relatório `.xlsx` via botão "Importar relatório"
4. Acompanhe os indicadores no Dashboard

### Importação de relatório

O arquivo deve conter as colunas: `funcid`, `tecnico`, `data_fechamento`, `baremo`, `avalia_prazo`, `realizado_no_prazo`, `atividade`, `expurgo_dupla`

## Tecnologias

- HTML/CSS/JS puro (single‑file)
- [Chart.js](https://www.chartjs.org/) — gráficos
- [SheetJS](https://sheetjs.com/) — leitura de arquivos .xlsx
- Firebase (opcional) — sincronização em nuvem
