# Solução de Business Intelligence para Otimização de Gestão Comercial no Varejo

## Visão Geral
Esta solução foi desenvolvida para otimizar processos de gestão comercial por meio da estruturação de dados operacionais, transformação analítica e geração de inteligência gerencial aplicada a um contexto varejista real.

O trabalho foi conduzido com foco em organização operacional, padronização de informações, criação de pipeline analítico e desenvolvimento de dashboards estratégicos para suporte à tomada de decisão.

Por questões de confidencialidade, informações comerciais, operacionais e estratégicas foram preservadas por meio de anonimização e adaptação estrutural. Esta documentação apresenta exclusivamente metodologia, arquitetura, stack técnica e capacidades analíticas implementadas.

---

# Contexto de Atuação
Desenvolvimento de uma solução prática de dados voltada à otimização de processos comerciais, análise de performance e organização estratégica de informações.

## Principais responsabilidades:
- Estruturação da coleta operacional de dados
- Organização e centralização de informações comerciais
- Tratamento e padronização de bases
- Validação e controle de qualidade de dados
- Modelagem relacional para análise
- Desenvolvimento de consultas analíticas com SQL
- Construção de dashboards estratégicos
- Definição de indicadores executivos, comerciais e operacionais

---

# Objetivo Estratégico
Desenvolvido para transformar registros operacionais em uma estrutura analítica robusta, permitindo visão consolidada sobre:

- Faturamento
- Lucro
- Ticket médio
- Performance comercial
- Performance por vendedor
- Performance por produto
- Gestão de estoque
- Eficiência operacional

---

# Stack Técnica Aplicada

## Coleta Operacional:
Google Forms

## Armazenamento Inicial:
Google Sheets

## Tratamento / ETL:
Python (Pandas)

## Modelagem Analítica:
SQL

## Business Intelligence:
Power BI

## Documentação Técnica:
dbdiagram.io + GitHub

---

# Arquitetura da Solução

## 1. Coleta Operacional
Implementada para padronizar o registro de vendas e operações comerciais.

---

## 2. Centralização de Dados
Estruturada em Google Sheets como camada inicial de armazenamento bruto.

---

## 3. Tratamento e Padronização com Python
Desenvolvido para garantir consistência e qualidade analítica por meio de:

- Limpeza de dados
- Padronização estrutural
- Conversão de tipos
- Remoção de duplicidades
- Validação
- Análise exploratória inicial

---

## 4. Modelagem e Estruturação com SQL
Aplicado para transformar dados operacionais em base analítica escalável:

- Consolidação de vendas
- Criação de tabelas fato e dimensão
- Ranking de produtos
- Ranking de vendedores
- Performance por forma de pagamento
- Análise de estoque crítico

---

## 5. Visualização Estratégica
Desenvolvida em Power BI para consolidar inteligência gerencial em dashboards multiárea.

---

# Estrutura Analítica Implementada
## Principais tabelas:
- tb_vendas
- tb_itens_venda
- tb_produtos
- tb_vendedores

## Fonte operacional:
- dados_brutos

---

# Modelagem Relacional
![Modelagem das Tabelas](./images/modelagem_tabelas.png)

---

# Dashboards Estratégicos Desenvolvidos

# Página 1 — Visão Executiva
### Desenvolvida para análise de:
- Receita
- Lucro
- Ticket Médio
- Formas de pagamento
- Evolução temporal de vendas

![Dashboard Executivo](./images/dashboard_executiva.png)

---

# Página 2 — Produtos & Categorias
### Desenvolvida para análise de:
- Produtos mais vendidos
- Produtos mais lucrativos
- Categorias estratégicas
- Estoque crítico

![Dashboard Produtos](./images/dashboard_produtos.png)

---

# Página 3 — Performance Comercial
### Desenvolvida para análise de:
- Faturamento por vendedor
- Ticket médio
- Volume de vendas
- Ranking de performance

![Dashboard Vendedores](./images/dashboard_vendedores.png)

---

# Página 4 — Operação & Estoque
### Desenvolvida para análise de:
- Gestão de estoque
- Produtos críticos
- Capital imobilizado
- Potencial operacional

![Dashboard Operação](./images/dashboard_operacao.png)

---

# Entregas Técnicas

## Python:
- tratamento_dados.py
- validacao_dados.py
- analise_exploratoria.py

## SQL:
- Consolidação de dados transacionais
- Estruturação relacional
- Consultas gerenciais
- Performance comercial
- Análise operacional

---

# Indicadores Estratégicos Desenvolvidos
- Faturamento Total
- Lucro Total
- Ticket Médio
- Total de Vendas
- Performance por Produto
- Performance por Categoria
- Performance por Vendedor
- Estoque Crítico
- Potencial de Receita

---

# Competências Técnicas Aplicadas
- Data Collection
- ETL
- Data Cleaning
- Data Validation
- Python (Pandas)
- SQL
- Data Modeling
- Power BI
- DAX
- KPI Design
- Business Intelligence
- Data Documentation

---

# Diferenciais da Solução
- Aplicação prática em operação comercial real
- Estrutura ponta a ponta
- Integração entre operação, análise e gestão
- Visão executiva, comercial e operacional
- Arquitetura documentada
- Proteção de informações estratégicas
- Organização compatível com portfólio profissional

---

# Confidencialidade
Toda a documentação foi estruturada para preservar integralmente informações estratégicas, operacionais e comerciais. Dados, nomes e elementos sensíveis foram anonimizados ou adaptados exclusivamente para demonstração técnica e portfólio profissional.

---

# Resultados e Impacto
A implementação desta solução permitiu estruturar uma base comercial descentralizada em uma arquitetura analítica organizada, ampliando capacidade de acompanhamento gerencial, análise de performance e suporte estratégico à tomada de decisão.

## Impactos principais:
- Padronização operacional
- Melhoria na organização de dados
- Visão consolidada de performance
- Estruturação de KPIs estratégicos
- Fortalecimento da gestão comercial orientada por dados
- Base preparada para evolução analítica

---

# Conclusão
Em conclusão, esta solução demonstra aplicação prática de análise de dados, Business Intelligence, tratamento analítico e organização estratégica de informações em contexto comercial, consolidando competências técnicas em Python, SQL, Power BI e documentação estruturada.

---

# Autor
## Thiago Ferreira

Desenvolvido como experiência prática aplicada em Dados, BI e Analytics, com foco em estruturação profissional, capacidade analítica e desenvolvimento técnico orientado a negócios.
