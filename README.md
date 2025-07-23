<!-- Tab simulation using details -->
<details open>
<summary>🇧🇷 Português</summary>

# Artigo Científico – Análise Preditiva da Produtividade do Trigo com Dados Sintéticos

Este repositório contém o conjunto de dados sintéticos e o código-fonte (notebooks Jupyter/Colab) utilizados nas análises apresentadas no artigo científico: "Análise Preditiva da Produtividade do Trigo em Múltiplos Ambientes Utilizando Modelos de Regressão e uma Base de Dados Sintética Fundamentada".

O objetivo deste projeto é demonstrar a viabilidade da aplicação de técnicas de Machine Learning para prever a produtividade de cultivares de trigo, utilizando uma base de dados agronômica sintética e robusta, fundamentada em um estudo de campo de referência.

## 🎯 Objetivo do Repositório

Este repositório visa garantir a reprodutibilidade completa dos experimentos e análises descritos no artigo científico associado. Ele permite a exploração, validação ou adaptação dos modelos preditivos para a produtividade do trigo (PROD_kg_ha) e o índice de produção corrigido (IPPH), e serve como um recurso para pesquisadores interessados na aplicação de aprendizado de máquina à agronomia e ao melhoramento genético de plantas, particularmente utilizando conjuntos de dados sintéticos.

## 📁 Estrutura do Repositório

-   **`/data/`**: Contém a base de dados sintética.
    -   📄 `dados_trigo_sinteticos.xlsx`: Dataset com 10.080 registros, simulando 16 cultivares de trigo em 9 ambientes (local x ano), com suas respectivas características fenotípicas e de produtividade.
-   **`/notebooks/`**: Contém os notebooks Jupyter com todo o fluxo de análise.
📄 01_geracao_dados_sinteticos.ipynb: Código para a geração da base de dados sintética com base nos parâmetros do estudo de referência.

📄 02_analise_exploratoria_correlacao.ipynb: Análise exploratória de dados (EDA), incluindo a geração de matrizes de correlação de Pearson e Spearman e visualizações 3D interativas.

📄 03_avaliacao_modelos_regressao.ipynb: Pré-processamento, treinamento e avaliação de mais de 20 modelos de regressão para prever PROD_kg_ha e IPPH utilizando validação cruzada.

📄 04_interpretabilidade_modelo_shap.ipynb: Análise de interpretabilidade (XAI) do melhor modelo preditivo utilizando a biblioteca SHAP.

📄 05_previsao_cenarios_futuros.ipynb: Aplicação do modelo final para realizar previsões em cenários agronômicos hipotéticos, incluindo anos futuros.

/figures/: Contém as visualizações geradas pelos notebooks.

📄 heatmap_pearson_correlation.png: Heatmap da matriz de correlação de Pearson.

📄 heatmap_spearman_correlation.png: Heatmap da matriz de correlação de Spearman.

📄 interactive_3d_plot.html: Arquivo HTML do gráfico 3D interativo (Plotly).

📄 r2_performance_prod.png: Gráfico de barras comparando o R² dos modelos para predição de produtividade.

📄 r2_performance_ipph.png: Gráfico de barras comparando o R² dos modelos para predição de IPPH.

📄 shap_summary_plot.png: Gráfico de resumo SHAP mostrando a importância das features.

📄 shap_dependence_plot.png: Gráfico de dependência SHAP para a variável de altura.

/results/: Armazena as métricas de desempenho dos modelos em formato CSV.

📄 performance_metrics_prod.csv: Métricas (R², MAE, RMSE) para os modelos de predição de PROD_kg_ha.

📄 performance_metrics_ipph.csv: Métricas para os modelos de predição de IPPH.

/article/: Contém os arquivos-fonte do manuscrito.

📄 manuscrito.tex: Código-fonte LaTeX do artigo científico.

📄 referencias.bib: Arquivo de bibliografia BibTeX.

## 📝 Observações Metodológicas

-   Todos os dados são sintéticos, gerados com base nos parâmetros estatísticos e relações agronômicas reportadas no estudo de referência de Cardozo (2024), Adaptabilidade e estabilidade de cultivares de trigo nas mesorregiões do Campo das Vertentes e sul/sudoeste de Minas Gerais.

-   A lógica de geração dos dados buscou refletir as interações Genótipo por Ambiente (GxE) plausíveis (e.g., efeito do local e ano na produtividade, resposta diferencial das cultivares), mas é, por natureza, uma simulação controlada.

As dependências Python necessárias para executar os notebooks estão listadas no arquivo requirements.txt.

## 🚀 Como Utilizar

1.  **Clone o repositório:**
    ```bash
    git clone [URL_DO_SEU_REPOSITORIO_GIT]
    cd [NOME_DA_PASTA_DO_REPOSITORIO]
    ```
2.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Execute os notebooks:** Abra os notebooks na pasta `/notebooks/` utilizando Jupyter Lab ou Google Colab para replicar as análises.

## 📄 Como Citar

Se você utilizar este repositório, a base de dados ou os conceitos apresentados no artigo, por favor cite o trabalho original (a citação completa será atualizada após a publicação):

> Brandão Junior, L.C. & Magalhães, R.R. (Ano). Análise Preditiva da Produtividade do Trigo em Múltiplos Ambientes Utilizando Modelos de Regressão e uma Base de Dados Sintética Fundamentada. Nome do Periódico, Volume(Edição), Páginas. DOI (se disponível)

## ⚖️ Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE.md).

</details>

<details>
<summary>🇺🇸 English</summary>

# Scientific Article – Predictive Analysis of Wheat Yield with Synthetic Data

This repository contains the synthetic dataset and source code (Jupyter/Colab notebooks) used in the analyses presented in the scientific article: "Predictive Analysis of Wheat Yield in Multiple Environments Using Regression Models and a Grounded Synthetic Dataset".

The goal of this project is to demonstrate the feasibility of applying Machine Learning techniques to predict the yield of wheat cultivars, using a robust, synthetic agronomic database grounded in a reference field study.

## 🎯 Repository Objective

This repository aims to ensure full reproducibility of the experiments and analyses described in the associated scientific article. It allows for the exploration, validation, or adaptation of predictive models for wheat yield (PROD_kg_ha) and the corrected production index (IPPH), and serves as a resource for researchers interested in applying machine learning to agronomy and plant breeding, particularly using synthetic datasets.


## 📁 Repository Structure

-   **`/data/`**: Contains the synthetic dataset.
    -   📄 `dados_trigo_sinteticos.xlsx`: Dataset with 10,080 records, simulating 16 wheat cultivars across 9 environments (location x year), with their respective phenotypic and yield traits.
    -   📄 01_synthetic_data_generation.ipynb: Code for generating the synthetic dataset based on parameters from the reference study.

    -   📄 02_exploratory_data_analysis_correlation.ipynb: Exploratory data analysis (EDA), including Pearson and Spearman correlation matrices and interactive 3D visualizations.

    -   📄 03_regression_model_evaluation.ipynb: Preprocessing, training, and evaluation of over 20 regression models to predict PROD_kg_ha and IPPH using cross-validation.

    -   📄 04_model_interpretation_with_shap.ipynb: Interpretable AI (XAI) analysis of the best predictive model using the SHAP library.

    -   📄 05_future_scenario_prediction.ipynb: Application of the final model to make predictions on hypothetical agronomic scenarios, including future years.

/figures/: Contains visualizations generated by the notebooks.

    -   📄 heatmap_pearson_correlation.png: Pearson correlation matrix heatmap.

    -   📄 heatmap_spearman_correlation.png: Spearman correlation matrix heatmap.

    -   📄 interactive_3d_plot.html: HTML file of the interactive 3D plot (Plotly).

    -   📄 r2_performance_prod.png: Bar chart comparing the R² scores of models for yield prediction.

    -   📄 r2_performance_ipph.png: Bar chart comparing the R² scores of models for IPPH prediction.

    -   📄 shap_summary_plot.png: SHAP summary plot showing feature importance.

    -   📄 shap_dependence_plot.png: SHAP dependence plot for the plant height variable.

/results/: Stores model performance metrics in CSV format.

    -   📄 performance_metrics_prod.csv: Metrics (R², MAE, RMSE) for PROD_kg_ha prediction models.

    -   📄 performance_metrics_ipph.csv: Metrics for IPPH prediction models.

/article/: Contains the source files for the manuscript.

    -   📄 manuscript.tex: LaTeX source code for the scientific article.

    -   📄 references.bib: BibTeX bibliography file.

    -   📝 Methodological Notes

All data are synthetic, generated based on the statistical parameters and agronomic relationships reported in the reference study by Cardozo (2024), Adaptabilidade e estabilidade de cultivares de trigo nas mesorregiões do Campo das Vertentes e sul/sudoeste de Minas Gerais.

The data generation logic aimed to reflect plausible Genotype-by-Environment (GxE) interactions (e.g., the effect of location and year on yield, differential cultivar responses) but is, by nature, a controlled simulation.

The Python dependencies required to run the notebooks are listed in the requirements.txt file.
## 🚀 How to Use

1.  **Clone the repository:**
    ```bash
    git clone [YOUR_GIT_REPOSITORY_URL]
    cd [REPOSITORY_FOLDER_NAME]
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the notebooks:** Open the notebooks in the `/notebooks/` folder using Jupyter Lab or Google Colab to replicate the analyses.

## 📄 How to Cite

If you use this repository, the dataset, or the concepts presented in the article, please cite the original work (full citation will be updated upon publication):

> Brandão Junior, L.C. & Magalhães, R.R. (Year). Predictive Analysis of Wheat Yield in Multiple Environments Using Regression Models and a Grounded Synthetic Dataset. Journal Name, Volume(Issue), Pages. DOI (if available)

## ⚖️ License

This project is licensed under the [MIT License](LICENSE.md).

</details>
