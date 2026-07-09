# 📊 Marketing Analytics — Performance de Campanhas (Power BI)

Análise de performance de campanhas de marketing digital construída em **Power BI**, respondendo a três perguntas de negócio: **descontos aumentam o volume vendido? Quais canais convertem melhor? As estimativas de crescimento das campanhas são confiáveis?**

## Visão Geral do Dashboard


<img width="1299" height="735" alt="images01_visao_geral" src="https://github.com/user-attachments/assets/083a40e3-bed8-4897-a710-2df777d579cf" />


---

## 🎯 Problema de negócio

Times de marketing investem em descontos e múltiplos canais sem saber, com dados, o que de fato move receita e conversão. Este projeto cruza transações, campanhas, clientes e eventos de navegação para orientar três decisões: política de descontos, alocação de verba por canal e confiança no planejamento de campanhas.

## 🔍 Principais insights

| # | Insight | Implicação para o negócio |
|---|---------|---------------------------|
| 1 | A quantidade média por transação **com e sem desconto varia entre 0% e 3%** em todas as categorias | O desconto não gera volume adicional — revisar a política de descontos, que reduz margem sem elevar vendas |
| 2 | **E-mail é a fonte de tráfego com maior taxa de conversão (8,9%)**, à frente de paid search | Priorizar CRM/e-mail na alocação de verba antes de expandir mídia paga |
| 3 | O crescimento esperado das campanhas (*expected uplift*) apresenta **correlação forte com a receita realizada** | O método de estimativa da empresa é consistente e pode ser usado no planejamento |

> ⚠️ Nota metodológica: a correlação do insight 3 é influenciada pelo porte das campanhas (campanhas maiores geram mais receita e maior uplift esperado). Uma evolução natural é normalizar por investimento ou nº de clientes impactados.

## 🗂️ Modelo de dados

Modelo em esquema estrela com 5 tabelas:

| Tabela | Papel | Conteúdo |
|--------|-------|----------|
| `transactions` | Fato | Transações com valor, quantidade e flag de desconto |
| `campaigns` | Dimensão | Campanhas, canal e uplift esperado |
| `customers` | Dimensão | Clientes e nível de fidelidade (loyalty tier) |
| `products` | Dimensão | Produtos e categorias |
| `events` | Fato | Eventos de navegação e fonte de tráfego |

## Modelo de Dados


<img width="985" height="686" alt="images02_modelo" src="https://github.com/user-attachments/assets/4d26333c-3afe-42de-958c-ab927aababff" />


## 📄 Estrutura do relatório

- **Página 1 — Visão Geral:** KPIs de receita e clientes, comparativo com/sem desconto por categoria, conversão por fonte de tráfego, funil por nível de fidelidade e dispersão uplift × receita.
- **Página 2 — Insights e Recomendações:** leitura analítica de cada visual, com conclusões e recomendações para o negócio.

## Página de Insights e Recomendações


<img width="1299" height="736" alt="images03_insights" src="https://github.com/user-attachments/assets/b989168e-0f26-4d0c-b6f9-9651b5b2868c" />


## 🛠️ Como usar

1. Baixe o arquivo [`report/marketing_analytics.pbix`](report/)
2. Abra no Power BI Desktop (versão mais recente)
3. Os dados estão embutidos no modelo — não é necessária configuração de fonte

## 📁 Estrutura do repositório

```
marketing-analytics-powerbi/
├── README.md
├── LICENSE
├── .gitignore
├── report/
│   └── marketing_analytics.pbix
├── images/
│   ├── 01_visao_geral.png
│   ├── 02_modelo.png
│   └── 03_insights.png
└── data/
    └── fonte_dos_dados.md
```

## 🧰 Stack

Power BI Desktop · DAX · Power Query · Modelagem dimensional (esquema estrela)

## 👩‍💻 Autora

**Priscilla de Jesus Paz** — profissional com 11 anos em tecnologia e qualidade de dados em sistemas de saúde pública, em transição para Análise de Dados.

[LinkedIn](https://www.linkedin.com/in/priscilla-j-paz) · [GitHub](https://github.com/priscilladejesuspaz)
