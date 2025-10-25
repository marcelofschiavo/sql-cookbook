# Portfólio de Análise SQL: People Analytics

**Autor:** Marcelo Ferreira Schiavo
[LinkedIn](link-para-seu-linkedin) | [GitHub](link-para-seu-github)

---

## 1. Resumo do Projeto

Este repositório contém um projeto de análise de dados "ponta-a-ponta" focado na área de **People Analytics (Recursos Humanos)**. O objetivo é demonstrar a aplicação prática de SQL para transformar dados brutos de RH em *insights* acionáveis que possam guiar a tomada de decisão estratégica.

A análise é apresentada em um notebook Jupyter (`.ipynb`) e é estruturada em **22 níveis de complexidade crescente**, partindo de consultas básicas de filtragem e culminando em análises estatísticas, hierárquicas e de qualidade de dados de nível sênior.

Os dados que compõem o banco de dados foram criados apenas para este projeto.

Uma versão PDF da apresentação está incluída no repositório. Uma versão online interativa (via Canva) também está disponível [aqui](link-para-seu-linkedin)."

## 2. O Problema de Negócio

Atuando como Analista de Dados para o time de RH, o desafio é responder a perguntas críticas sobre a força de trabalho da empresa, incluindo:
* **Compensação e Custo:** Como nossa folha de pagamento está distribuída? Estamos pagando de forma justa e competitiva?
* **Performance e Talentos:** Quem são nossos melhores funcionários? Quem está em risco de *burnout* ou desengajamento?
* **Retenção e Cultura:** Nós recompensamos performance ou apenas tempo de casa?
* **Qualidade dos Dados:** Nossos dados de RH são confiáveis para tomar essas decisões?

## 3. Stack de Ferramentas (Tool Stack)

| Ferramenta | Propósito |
| :--- | :--- |
| **Python** | Linguagem base para orquestração e setup do ambiente. |
| **Pandas** | Utilizado para criar os arquivos `.csv` e exibir os resultados das consultas. |
| **DuckDB** | Motor SQL analítico (OLAP) de alta performance, usado para consultar os `.csv` diretamente. |
| **Jupyter/Colab** | Ambiente interativo de análise para documentação e *storytelling*. |

## 4. Como Executar Este Projeto

Este notebook é 100% autocontido e não requer arquivos externos.

1.  Clone este repositório.
2.  Instale as bibliotecas necessárias:
    ```bash
    pip install pandas duckdb jupyterlab
    ```
3.  Abra o arquivo `.ipynb` (seja no Google Colab, VS Code ou Jupyter).
4.  Execute as células na ordem:
    * A **Célula 4** irá criar os arquivos `.csv` simulados no ambiente.
    * As células seguintes irão consultar esses arquivos.

## 5. Estrutura da Análise (Níveis 1-22)

A análise é dividida em níveis para demonstrar uma progressão lógica de investigação:

* **Níveis 1-5 (Fundamentos):**
    * Filtragem (`WHERE`), Agregação (`GROUP BY`), Junções (`JOIN`), Funções de Data (`CAST`, `CURRENT_DATE`) e CTEs (`WITH`).
* **Níveis 6-10 (Análise de BI):**
    * Funções de Janela (`RANK()`, `LAG()`, `NTILE()`) e Agregações Móveis (`SUM() OVER(...)`).
* **Níveis 11-15 (Análise Sênior):**
    * Operações de Conjunto (`EXCEPT`), Análise de Coorte (`LIKE`), CTEs Recursivas (para hierarquia) e Lógica Condicional Agregada (para Dashboards de BI).
* **Níveis 16-22 (Estatística e Data Quality):**
    * Análise de Correlação (`CORR()`), Percentis (`MEDIAN`), Desvio Padrão (`STDDEV_POP`), Pivotagem Nativa (`PIVOT`), Regex (`REGEXP_MATCHES`) e Detecção de Duplicatas (`ROW_NUMBER()`).

## 6. Principais Insights e Recomendações

A análise gerou quatro principais *insights* acionáveis para o negócio:

1.  **Risco de Equidade em Engenharia** 
2.  **Risco de Receita em Vendas** 
3.  **Desalinhamento Cultural Crítico** 
4.  **Risco de Processo e Compliance

## 7. Glossário de Conceitos Estatísticos

O projeto é finalizado com um glossário detalhado (em Markdown) que explica os conceitos estatísticos por trás das consultas, incluindo:
* Média vs. Mediana (P50)
* Análise de Percentis e Quartis (P90, NTILE)
* Medidas de Dispersão (Desvio Padrão)
* Análise de Correlação (Coeficiente de Pearson)
