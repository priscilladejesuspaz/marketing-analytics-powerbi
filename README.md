# Marketing Analytics Dashboard | Power BI

## Sobre o projeto

Este projeto apresenta uma análise de desempenho de campanhas de marketing utilizando Power BI.

O objetivo é transformar dados de campanhas, clientes, eventos e transações em indicadores que auxiliem gestores na avaliação da efetividade das campanhas, canais de aquisição e impacto dos descontos sobre as vendas.

---

## Objetivos do projeto

- Avaliar o desempenho das campanhas de marketing.
- Identificar os canais com maior taxa de conversão.
- Analisar o impacto dos descontos na receita.
- Comparar campanhas com e sem desconto.
- Identificar categorias e produtos com melhor desempenho.
- Apoiar a tomada de decisão baseada em dados.

---

## Dataset

O projeto utiliza uma base de dados de marketing contendo informações sobre:

- Campanhas
- Clientes
- Eventos
- Produtos
- Transações

---

## Tecnologias utilizadas

- Power BI
- Power Query
- DAX
- Modelagem Dimensional

---

## Modelagem

Foi adotada uma modelagem dimensional do tipo Estrela (Star Schema), composta por duas tabelas fato (transactions e events) e três tabelas dimensão (customers, campaigns e products), permitindo análises eficientes sobre campanhas, clientes e transações.

### Tabelas Fato

- Transactions
- Events

### Tabelas Dimensão

- Campaigns
- Customers
- Products

---

## Principais KPIs

- Receita Total
- Taxa de Conversão
- Receita por Campanha
- Receita por Categoria
- Receita por Canal
- Comparativo entre campanhas com e sem desconto
- Ticket Médio

---

## Principais Insights

- O e-mail apresentou a maior taxa de conversão entre os canais analisados.
- Campanhas com desconto não apresentaram aumento significativo no volume de vendas quando comparadas às campanhas sem desconto.
- Algumas categorias concentraram grande parte da receita total, indicando oportunidades de otimização das campanhas.
- A análise permite identificar quais campanhas entregaram maior retorno para o negócio.

---

## Estrutura do Projeto

```
marketing-analytics-powerbi/

│
├── Marketing Analytics.pbix
├── README.md
├── images/
│   ├── dashboard.png
│   ├── modelo-dados.png
│   └── insights.png
│
└── docs/
    └── medidas-dax.md
```

---

## Imagens

### Dashboard Geral


<img width="1299" height="735" alt="isczKVLWcp" src="https://github.com/user-attachments/assets/081efcf7-f888-4774-ad5a-76281fcc4ba9" />


### Modelo de Dados


<img width="985" height="686" alt="lz7z94x6sc" src="https://github.com/user-attachments/assets/cfe9ed96-a08b-4efe-b0a2-cd4f576a90b6" />


### Página de Insights


<img width="1299" height="736" alt="fhGDw6DIB6" src="https://github.com/user-attachments/assets/7ad9d9c2-cf28-4de9-ac42-2c5eda647b85" />


## Possíveis melhorias

- Inclusão de tabela calendário.
- Organização das medidas em uma tabela dedicada.
- Criação de tooltips personalizados.
- Implementação de bookmarks.
- Otimização do tamanho do arquivo Power BI.

---

## Aprendizados

Durante o desenvolvimento deste projeto foram aplicados conceitos de:

- Modelagem Dimensional
- Power Query
- DAX
- Criação de KPIs
- Storytelling com Dados
- Visualização de Dados
- Análise de Marketing

---

## Autor

**Priscilla de Jesus Paz**

- LinkedIn: https://linkedin.com/in/priscilla-j-paz
- GitHub: https://github.com/priscilladejesuspaz
