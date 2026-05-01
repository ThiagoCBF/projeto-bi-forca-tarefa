# Projeto de Business Intelligence para Gestão Comercial de Varejo

## Visão Geral
Este projeto foi desenvolvido como uma solução de Business Intelligence aplicada a uma operação comercial varejista real, com foco em estruturar dados operacionais, transformar informações transacionais em indicadores estratégicos e fornecer suporte visual à tomada de decisão por meio de dashboards gerenciais.

Por questões de confidencialidade, dados operacionais, nomes e informações sensíveis foram anonimizados. Este repositório apresenta a arquitetura, metodologia, modelagem e resultados analíticos do projeto.

---

# Objetivo do Projeto
Desenvolver uma estrutura completa de análise de dados para gestão comercial, abrangendo:

- Coleta padronizada de vendas
- Estruturação e transformação de dados
- Modelagem relacional
- Construção de KPIs estratégicos
- Dashboards executivos e operacionais
- Análise de vendas, produtos, vendedores e estoque

---

# Problema de Negócio
A operação comercial possuía coleta de dados descentralizada e ausência de visão consolidada sobre:

- Faturamento
- Lucro
- Ticket médio
- Performance de vendedores
- Produtos mais vendidos
- Produtos mais lucrativos
- Estoque crítico
- Capital parado em estoque

---

# Solução Desenvolvida
Foi implementado um pipeline de Business Intelligence utilizando ferramentas acessíveis e foco em automação e gestão:

## Coleta:
- Google Forms

## Armazenamento:
- Google Sheets

## Transformação / ETL:
- Power Query

## Modelagem:
- Estrutura relacional com tabelas fato e dimensão

## Visualização:
- Power BI

## Métricas:
- DAX (Data Analysis Expressions)

---

# Modelagem de Dados
A estrutura foi organizada com base em modelagem relacional para garantir escalabilidade analítica.

## Tabelas principais:
- `tb_vendas`
- `tb_itens_venda`
- `tb_produtos`
- `tb_vendedores`

## Fonte operacional:
- `dados_brutos`

---

# Modelo Relacional
![Modelagem das Tabelas](./images/modelagem_tabelas.png)

---

# Dashboards Desenvolvidos

# Página 1 — Visão Executiva
## Indicadores:
- Faturamento Total
- Lucro Total
- Ticket Médio
- Total de Vendas

## Análises:
- Evolução temporal de vendas
- Formas de pagamento
- Ranking comercial

![Dashboard Executivo](./images/dashboard_executiva.png)

---

# Página 2 — Produtos & Categorias
## Indicadores:
- Produtos mais vendidos
- Produtos mais lucrativos
- Performance por categoria
- Estoque crítico

## Análises:
- Top 10 vendas
- Top 10 lucro
- Gestão de portfólio
- Reposição

![Dashboard Produtos](./images/dashboard_produtos.png)

---

# Página 3 — Performance de Vendedores
## Indicadores:
- Faturamento por vendedor
- Lucro por vendedor
- Ticket médio
- Volume de vendas

## Análises:
- Ranking comercial
- Performance temporal
- Eficiência de vendas

![Dashboard Vendedores](./images/dashboard_vendedores.png)

---

# Página 4 — Estoque & Operação
## Indicadores:
- Estoque total
- Valor em estoque
- Produtos críticos
- Potencial de venda

## Análises:
- Capital parado
- Risco de ruptura
- Saúde operacional

![Dashboard Operação](./images/dashboard_operacao.png)

---

# Principais KPIs Construídos
- Faturamento Total
- Lucro Total
- Ticket Médio
- Total de Vendas
- Quantidade Vendida
- Margem por Produto
- Performance por Categoria
- Performance por Vendedor
- Estoque Crítico
- Potencial de Receita

---

# Principais Insights Gerados
- Identificação de produtos de maior giro vs maior margem
- Análise de vendedores por volume e qualidade de vendas
- Visão de categorias estratégicas
- Mapeamento de estoque crítico
- Identificação de capital parado
- Estruturação de gestão comercial orientada por dados

---

# Tecnologias Utilizadas
- Google Forms
- Google Sheets
- Power Query
- Power BI
- DAX
- dbdiagram.io

---

# Diferenciais do Projeto
- Aplicação em contexto comercial real
- Estruturação ponta a ponta (coleta → transformação → BI)
- Modelagem relacional
- Dashboard multiárea
- Foco em tomada de decisão
- Visão executiva + operacional

---

# Aprendizados Técnicos
Durante o desenvolvimento deste projeto, foram aplicados conceitos de:

- ETL
- Data Modeling
- Business Intelligence
- KPI Design
- Data Visualization
- Power Query
- DAX
- Gestão orientada por dados

---

# Observação de Confidencialidade
Este projeto foi publicado exclusivamente para fins de portfólio profissional. Todos os dados, nomes, valores e elementos sensíveis foram anonimizados ou adaptados para preservar confidencialidade operacional.

---

# Próximos Passos
- Evolução para SQL como camada analítica
- Automação expandida
- Forecast de vendas
- Análise preditiva
- Expansão para engenharia de dados

---

# Autor
## Thiago Ferreira

Projeto independente com foco em desenvolvimento profissional em Dados, BI e Analytics.
