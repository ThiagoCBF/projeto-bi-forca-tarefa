# Estrutura do Projeto

## Visão Geral

Esta documentação descreve a estrutura da solução de dados desenvolvida para análise comercial no varejo.

A arquitetura foi projetada com base em boas práticas de engenharia e análise de dados, separando claramente as camadas de ingestão, processamento, análise e visualização.

## Estrutura de Pastas

```
solucao-bi-varejo/

├── app_streamlit/
│   └── app.py
│
├── python/
│   ├── tratamento_dados.py
│   ├── analise_exploratoria.py
│   └── validacao_dados.py
│
├── sql/
│   └── queries.sql
│
├── images/
│   ├── dashboard_executiva.png
│   ├── dashboard_produtos.png
│   ├── dashboard_vendedores.png
│   ├── dashboard_operacao.png
│   ├── modelagem_tabelas.png
│   └── streamlit_interface.png
│
├── docs/
│   ├── arquitetura_solucao.md
│   ├── estrutura_projeto.md
│   └── dicionario_dados.md
│
└── README.md
```

## Descrição das Camadas

### app_streamlit
Aplicação responsável pelo registro de vendas de forma operacional, permitindo a inserção de múltiplos produtos por transação e geração da base de dados.

---

### python
Camada responsável pelo processamento dos dados, incluindo:

- Tratamento e padronização da base
- Análise exploratória de dados (KPIs e métricas)
- Validação de qualidade dos dados

---

### sql
Camada de modelagem analítica, contendo consultas utilizadas para:

- Cálculo de KPIs
- Agregações de vendas
- Análises por produto, vendedor e período

---

### images
Contém as evidências visuais da solução:

- Dashboards do Power BI
- Modelagem de dados
- Interface do Streamlit

> ⚠️ Todas as imagens utilizam dados fictícios para fins de demonstração.

---

### docs
Documentação técnica da solução:

- Arquitetura do sistema
- Estrutura do projeto
- Dicionário de dados

---

## Boas Práticas Aplicadas

- Separação por camadas de dados
- Organização modular do código
- Pipeline estruturado de dados (ETL + BI)
- Isolamento de dados sensíveis
- Estrutura compatível com projetos reais de dados

---

## Conclusão

Esta solução simula um fluxo completo de dados para análise comercial, desde a captura operacional até a visualização estratégica em dashboards.

O objetivo é demonstrar competências em análise de dados, engenharia de dados e business intelligence aplicados a um cenário realista de varejo.

---

**Autor:** Thiago Ferreira
