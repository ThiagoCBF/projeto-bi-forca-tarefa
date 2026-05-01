# Arquitetura da Solução

## Visão Estratégica
Esta solução foi estruturada para otimizar processos de gestão comercial por meio da transformação de dados operacionais em inteligência analítica, permitindo organização, padronização, monitoramento de performance e suporte à tomada de decisão.

A arquitetura implementada foi desenvolvida para consolidar múltiplas etapas de dados — da coleta operacional à visualização executiva — em uma estrutura lógica, escalável e orientada a Business Intelligence.

---

# Objetivo da Arquitetura
Desenvolvido para estruturar uma operação comercial em uma pipeline analítica organizada, permitindo:

- Padronização de registros operacionais
- Centralização de dados
- Tratamento e validação
- Modelagem relacional
- Análise estratégica
- Visualização gerencial
- Suporte à gestão comercial

---

# Camadas da Solução

# 1. Coleta Operacional
## Ferramenta:
Google Forms

## Finalidade:
Implementado para padronizar o registro de vendas e garantir consistência na captura inicial de dados comerciais.

## Dados coletados:
- Data e hora
- ID da venda
- Vendedor
- Forma de pagamento
- Produto
- Quantidade
- Valor total

---

# 2. Armazenamento Inicial
## Ferramenta:
Google Sheets

## Finalidade:
Estruturado como camada inicial de centralização de dados brutos, permitindo armazenamento automatizado e organização operacional.

## Base:
- dados_brutos

---

# 3. Tratamento, Padronização e Validação
## Ferramenta:
Python (Pandas)

## Finalidade:
Desenvolvido para garantir integridade, qualidade e consistência analítica antes da modelagem.

## Processos aplicados:
- Limpeza de dados
- Padronização estrutural
- Conversão de tipos
- Tratamento de valores nulos
- Remoção de duplicidades
- Validação de consistência
- Análise exploratória inicial

## Entregas:
- tratamento_dados.py
- validacao_dados.py
- analise_exploratoria.py

## Saída:
- dados_tratados

---

# 4. Modelagem Relacional e Estrutura Analítica
## Ferramenta:
SQL

## Finalidade:
Aplicado para transformar dados tratados em uma estrutura relacional orientada à análise e escalabilidade.

## Processos:
- Consolidação de vendas
- Separação entre fatos e dimensões
- Estruturação de tabelas analíticas
- Queries gerenciais
- Ranking comercial
- Performance de produtos
- Análise operacional

## Principais tabelas:
- tb_vendas
- tb_itens_venda
- tb_produtos
- tb_vendedores

---

# 5. Camada de Business Intelligence
## Ferramenta:
Power BI

## Finalidade:
Desenvolvida para transformar dados estruturados em dashboards gerenciais e indicadores estratégicos.

## Dashboards:
### Página 1:
Visão Executiva

### Página 2:
Produtos & Categorias

### Página 3:
Performance Comercial

### Página 4:
Operação & Estoque

---

# Fluxo da Solução

Google Forms  
→ Google Sheets  
→ Python (Tratamento / Validação / Análise)  
→ SQL (Modelagem / Consolidação / Queries)  
→ Power BI (Dashboards / KPIs / Gestão)

---

# Estrutura Técnica do Repositório

```txt
solucao-bi-gestao-comercial/
│── README.md
│
├── images/
│   ├── dashboard_executiva.png
│   ├── dashboard_produtos.png
│   ├── dashboard_vendedores.png
│   ├── dashboard_operacao.png
│   └── modelagem_tabelas.png
│
├── python/
│   ├── tratamento_dados.py
│   ├── validacao_dados.py
│   └── analise_exploratoria.py
│
├── sql/
│   ├── criacao_tb_vendas.sql
│   ├── criacao_tb_itens_venda.sql
│   ├── ranking_produtos.sql
│   ├── ranking_vendedores.sql
│   ├── estoque_critico.sql
│   ├── lucro_produtos.sql
│   └── vendas_por_pagamento.sql
│
└── docs/
    ├── arquitetura_solucao.md
    └── data_dictionary.md