# 📊 Dashboard de Vendas — Power BI

Este projeto apresenta uma **análise de vendas e lucratividade**, desenvolvida no **Power BI**, utilizando a base de dados **SuperStore**, bastante conhecida para estudos e projetos de análise de dados.

O foco do dashboard é transformar dados brutos em **informações visuais claras**, facilitando a leitura de indicadores financeiros e o entendimento do desempenho do negócio ao longo do tempo.

---

## 🖼️ Visão Geral do Dashboard

![Dashboard de Vendas](dash.png)

---

## 🎯 Objetivo do Projeto

- Analisar o **desempenho de vendas** da empresa
- Avaliar **lucro, margem de lucro e ticket médio**
- Identificar **categorias, produtos e regiões** mais relevantes
- Praticar **modelagem de dados**, **medidas DAX** e **visualização no Power BI**
- Criar um dashboard com **padrão profissional para portfólio**

---

## 📂 Estrutura do Projeto

MEU-DASH/
│
├── data/
│ └── base de dados SuperStore_data.csv
│
├── Dash - SuperStore.pbix
├── dash.png
└── README.md

---

## 📊 Indicadores (KPIs)

O dashboard apresenta os seguintes indicadores principais:

- **Total de Vendas**
- **Lucro**
- **Margem de Lucro**
- **Ticket Médio**

Esses KPIs permitem uma visão rápida da saúde financeira do negócio.

---

## 📐 Medidas Criadas (DAX)

As principais medidas criadas no projeto foram:

```DAX
TotalVendas = SUM(SuperStore[Sales])

Lucro = SUM(SuperStore[Profit])

MargemLucro = DIVIDE([Lucro], [TotalVendas])

TicketMedio = DIVIDE([TotalVendas], DISTINCTCOUNT(SuperStore[Order ID]))
```

## 🔎 Análises Realizadas

Comparação do total de vendas por categoria

Evolução das vendas ao longo do tempo (Ano e Mês)

Identificação dos produtos com maiores valores de venda e lucro

Análise geográfica de vendas por região

Identificação de tendências de crescimento no faturamento


## ⚠️ Observação Importante sobre a Margem de Lucro

A margem de lucro apresenta um valor elevado (acima de 100%), o que pode chamar atenção à primeira vista.

Isso ocorre devido às características da própria base de dados SuperStore, que contém:

Registros com lucros muito altos

Valores negativos em alguns produtos

Estrutura voltada para aprendizado e simulação, não para um cenário financeiro real

O objetivo do projeto não foi ajustar ou alterar os dados, mas sim:

Trabalhar com a base original

Entender o impacto dos dados nos cálculos

Focar em modelagem, DAX e visualização

Esse ponto foi tratado como aprendizado técnico, e não como erro.


## 🛠️ Ferramentas Utilizadas

Power BI Desktop

DAX para criação de medidas

Power Query para tratamento e transformação de dados

Visualizações nativas do Power BI (gráficos, tabela e mapa)


## 📌 Considerações Finais

Este projeto faz parte do meu portfólio de Análise de Dados e representa uma evolução em relação a dashboards iniciais, com maior volume de dados, mais indicadores e análises mais completas.

O foco foi criar um dashboard:

Organizado

Visualmente limpo

Com leitura clara

Próximo de um cenário real de negócio

Feedbacks e sugestões são sempre bem-vindos!