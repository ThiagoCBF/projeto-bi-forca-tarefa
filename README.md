# Solução de Business Intelligence para Gestão Comercial no Varejo

## Visão Geral

Esta solução foi desenvolvida para estruturar e automatizar o processo de gestão comercial de uma operação de varejo, substituindo processos manuais por uma aplicação centralizada em Streamlit e uma arquitetura de dados voltada à análise.

A evolução do sistema permitiu a implementação de um fluxo de dados mais confiável, com suporte a transações multi-itens, padronização na origem e geração de uma base analítica estruturada para consumo em ferramentas de Business Intelligence.

---

## ⚠️ Confidencialidade

Todas as imagens, valores e indicadores apresentados neste documento utilizam **dados fictícios**, com o objetivo de preservar informações sensíveis da operação real.

---

## Contexto do Problema

O processo anterior baseado em formulários apresentava limitações como:
- baixa estruturação dos dados
- dificuldade no registro de múltiplos produtos por venda
- inconsistências na consolidação para análise

Para resolver esse cenário, foi desenvolvida uma aplicação em Streamlit que centraliza o registro de vendas e estrutura os dados já na origem.

---

## Stack Técnica

- Interface de Ingestão: Streamlit (Python)  
- Armazenamento: CSV (camada transacional)  
- Processamento de Dados: Python (Pandas)  
- Modelagem de Dados: SQL (modelo dimensional)  
- Visualização: Power BI  

---

## Arquitetura da Solução

### 1. Camada de Ingestão (Streamlit)

Aplicação responsável pelo registro operacional das vendas, contendo:

- suporte a múltiplos produtos por transação (carrinho de compras)  
- cálculo automático de subtotais e total da venda  
- geração de identificador único (id_venda)  
- padronização dos dados no momento da entrada  

📌 Interface do sistema de registro (dados fictícios):

![Streamlit Interface](images/streamlit_interface.png)

---

### 2. Camada de Processamento e Padronização (Python - ETL)

Nesta etapa são aplicados scripts em Python responsáveis pela preparação dos dados para análise, incluindo:

- padronização de nomes de colunas  
- tratamento de tipos de dados (datas, valores numéricos e categorias)  
- validação de integridade das transações  
- consolidação de vendas multi-itens  
- organização do dataset para consumo analítico  

---

### 3. Camada de Dados (CSV)

Os dados são armazenados em formato transacional estruturado, permitindo rastreabilidade completa das vendas e histórico operacional.

---

### 4. Camada de Modelagem (SQL)

Os dados são estruturados em modelo analítico com abordagem dimensional (Star Schema), permitindo:

- consultas otimizadas por produto, vendedor e período  
- análise de performance comercial  
- suporte direto à construção de dashboards  

📌 Modelagem de dados (dados fictícios):

![Modelagem de Tabelas](images/modelagem_tabelas.png)

---

### 5. Camada de Visualização (Power BI)

Os dados são transformados em dashboards estratégicos para suporte à tomada de decisão.

---

## Visualização Estratégica e KPIs

A camada de BI foi estruturada com foco em indicadores operacionais e estratégicos:

### Visão Executiva
Acompanhamento dos principais KPIs do negócio:
- Receita total  
- Ticket médio  
- Volume de vendas  
- Evolução temporal da performance  

📌 Dashboard Executivo (dados fictícios):

![Dashboard Executivo](images/dashboard_executiva.png)

---

### Análise de Produtos
Foco na inteligência de portfólio:
- produtos mais vendidos  
- análise de giro  
- contribuição por item na receita total  
- identificação de produtos estratégicos  

📌 Dashboard Produtos (dados fictícios):

![Dashboard Produtos](images/dashboard_produtos.png)

---

### Performance Comercial
Avaliação do desempenho individual da equipe:
- ranking de vendedores  
- volume de vendas por colaborador  
- contribuição por faturamento  
- comparação de performance  

📌 Dashboard Vendedores (dados fictícios):

![Dashboard Vendedores](images/dashboard_vendedores.png)

---

### Visão Operacional
Monitoramento do fluxo de vendas e operação:
- volume de transações  
- comportamento de compra  
- análise operacional do dia a dia  

📌 Dashboard Operação (dados fictícios):

![Dashboard Operação](images/dashboard_operacao.png)

---

## Competências Técnicas Aplicadas

- Desenvolvimento de aplicações com Streamlit  
- Engenharia de dados com Python (Pandas)  
- Processos de ETL e padronização de dados  
- Modelagem de dados relacional e dimensional (SQL)  
- Construção de dashboards com Power BI  
- Definição e análise de KPIs de negócio  

---

## Conclusão

Este projeto demonstra a capacidade de transformar uma operação comercial real por meio de tecnologia. A evolução da ferramenta de coleta destaca o foco na qualidade do dado e na escalabilidade da solução analítica, consolidando competências essenciais para um profissional de Dados e BI.

**Autor:** Thiago Ferreira
