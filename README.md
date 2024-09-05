# Distribuição Renovavel

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

Projeção de demanda de energia elétrica e recomendação de distribuição de fontes renováveis por região e subsistema de energia brasileiro.

## Bases de dados
Fontes externas utilizadas para construção do projeto.

### Consumo mensal de energia elétrica
Dados de consumo mensal de energia elétrica agregados por região, subsistema, classe, disponibilizado pela [EPE – Empresa de Pesquisa Energética](https://www.epe.gov.br/pt/publicacoes-dados-abertos/dados-abertos/dados-do-consumo-mensal-de-energia-eletrica), no endereço web [consumo-mensal-de-energia-eletrica](https://www.epe.gov.br/pt/publicacoes-dados-abertos/dados-abertos/dados-do-consumo-mensal-de-energia-eletrica).

#### Objetivo de utilização
Construção de projeções de demanda elétrica em diferentes regiões e/ou subsistemas.

### Capacidade instalada de geração
Dados de potência nominal de Unidades Geradoras de Usinas despachadas pelo [Operador Nacional do Sistema Elétrico (ONS)](https://dados.ons.org.br/), entre estas eolielétrica (eólica), fotovoltaica (solar), hidrelétrica, nuclear e térmica, disponível no endereço web [capacidade-geracao](https://dados.ons.org.br/dataset/capacidade-geracao).

#### Obetivo de utilização
Avaliação de disponibilidade de geração de energia renovável em diferentes regiões e/ou subsistemas, a fim de identificar oportunidades de distribuição de energia renovável segundo demanda de mercado.

### Dados comerciais de distribuidoras de energia
Dados de todas as distribuidoras brasileiras de energia, relacionados a aspectos comerciais, tais como faturamento, danos elétricos e atendimento, agregados por mês e município, disponibilizados pela [Agência Nacional de Energia Elétrica (ANEEL)](https://dadosabertos.aneel.gov.br/), no endereço web [indger-indicadores-gerenciais-da-distribuicao](https://dadosabertos.aneel.gov.br/dataset/indger-indicadores-gerenciais-da-distribuicao).

#### Objetivo de utilização
Identificar áreas de atuação de distribuidoras de energia a fim de gerar recomendações de utilização de energias renováveis específicas, baseadas na demanda e disponibilidade de geração nas áreas de atuação.

## Organização do Projeto

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         distribuicao_renovavel and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── distribuicao_renovavel   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes distribuicao_renovavel a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

