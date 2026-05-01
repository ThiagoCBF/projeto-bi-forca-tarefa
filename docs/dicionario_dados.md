# Data Dictionary

## Visão Geral
Esta documentação apresenta a estrutura de dados implementada na solução de Business Intelligence desenvolvida para otimização de gestão comercial.

O objetivo desta estrutura é organizar dados operacionais em camadas analíticas, permitindo padronização, modelagem relacional, consultas estratégicas e suporte à construção de dashboards gerenciais.

---

# Fonte Operacional Primária

# dados_brutos
Base inicial originada da coleta operacional via Google Forms e centralizada em Google Sheets.

## Finalidade:
Captura padronizada de registros comerciais para posterior tratamento, validação e estruturação analítica.

| Campo | Tipo | Descrição |
|------|------|------------|
| data_hora | datetime | Data e hora do registro operacional |
| id_venda | varchar | Identificador único da venda |
| vendedor | varchar | Nome do responsável pela venda |
| forma_pagamento | varchar | Método de pagamento utilizado |
| produto | varchar | Produto registrado |
| quantidade_produto | int | Quantidade vendida |
| valor_total | decimal | Valor total informado |

---

# Camada de Dados Tratados

# dados_tratados
Base processada após aplicação de limpeza, padronização e validação via Python.

## Finalidade:
Garantir qualidade e consistência antes da modelagem relacional.

## Processos aplicados:
- Padronização de colunas
- Conversão de tipos
- Tratamento de nulos
- Remoção de duplicidades
- Normalização textual

---

# Camada Analítica

# tb_vendas
Tabela fato consolidada por venda.

## Finalidade:
Concentrar informações principais de cada transação comercial.

| Campo | Tipo | Descrição |
|------|------|------------|
| id_venda | varchar | Identificador único da venda |
| data_venda | datetime | Data consolidada da venda |
| nome_vendedor | varchar | Vendedor responsável |
| forma_pagamento | varchar | Método de pagamento |
| valor_total_venda | decimal | Valor consolidado da venda |

---

# tb_itens_venda
Tabela transacional detalhada por item vendido.

## Finalidade:
Registrar granularidade por produto dentro de cada venda.

| Campo | Tipo | Descrição |
|------|------|------------|
| id_item | int | Identificador único do item |
| id_venda | varchar | Relacionamento com tb_vendas |
| nome_produto | varchar | Produto comercializado |
| quantidade | int | Quantidade vendida |
| valor_unitario | decimal | Valor unitário calculado |

---

# tb_produtos
Tabela dimensão de produtos.

## Finalidade:
Estruturar informações estratégicas de portfólio e operação.

| Campo | Tipo | Descrição |
|------|------|------------|
| id_produto | varchar | Identificador único do produto |
| nome_produto | varchar | Nome do produto |
| categoria | varchar | Categoria comercial |
| custo | decimal | Custo unitário |
| preco_venda | decimal | Preço de venda |
| estoque | int | Quantidade disponível |

---

# tb_vendedores
Tabela dimensão de vendedores.

## Finalidade:
Organizar estrutura comercial para análises de performance.

| Campo | Tipo | Descrição |
|------|------|------------|
| id_vendedor | varchar | Identificador único |
| nome_vendedor | varchar | Nome do vendedor |

---

# Relacionamentos Analíticos

## tb_vendas
- id_venda → tb_itens_venda.id_venda
- nome_vendedor → tb_vendedores.nome_vendedor

---

## tb_itens_venda
- nome_produto → tb_produtos.nome_produto

---

# Regras de Negócio Estruturais

## Venda:
Uma venda pode conter múltiplos produtos vinculados ao mesmo `id_venda`.

---

## Itens:
Cada item representa uma unidade transacional vinculada à venda principal.

---

## Estoque Crítico:
Produtos com estoque inferior ao limite operacional definido para monitoramento estratégico.

---

## Ticket Médio:
Faturamento total dividido pelo total de vendas consolidadas.

---

# Indicadores Estratégicos Derivados

## Comerciais:
- Faturamento Total
- Ticket Médio
- Total de Vendas
- Ranking de Vendedores
- Performance por Forma de Pagamento

---

## Produtos:
- Quantidade Vendida
- Faturamento por Produto
- Lucro por Produto
- Performance por Categoria

---

## Operacionais:
- Estoque Atual
- Estoque Crítico
- Capital em Estoque
- Potencial de Receita

---

# Governança e Qualidade de Dados
A estrutura foi desenvolvida considerando princípios de organização analítica e consistência operacional:

- Padronização de entradas
- Validação de registros
- Tratamento de inconsistências
- Separação entre camada bruta, tratada e analítica
- Escalabilidade para futuras integrações

---

# Segurança e Confidencialidade
Todos os elementos desta documentação foram estruturados para preservar informações estratégicas e comerciais. Dados reais, nomes, valores e elementos sensíveis foram anonimizados ou adaptados para fins exclusivos de portfólio técnico e documentação profissional.

---

# Conclusão
O modelo de dados implementado organiza uma operação comercial em estrutura relacional analítica, permitindo suporte robusto à gestão, monitoramento estratégico e expansão para análises mais avançadas em Business Intelligence, SQL e automação.