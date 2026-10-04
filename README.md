# Pipeline de Dados com Python e Programação Orientada a Objetos

Projeto de Engenharia de Dados que combina informações de fontes heterogêneas e organiza o fluxo em camadas de dados brutos, processamento e dados refinados.

## Objetivo

O projeto demonstra como um pipeline em Python pode ingerir dados em diferentes formatos, realizar transformações e produzir um conjunto consolidado pronto para análise.

## Arquitetura

```text
Fonte JSON ---------\
                     > Dados brutos -> Processamento em Python -> Dados refinados
Fonte CSV ----------/
```

## Estrutura do repositório

```text
pipeline_dados/
├── notebooks/
│   └── exploracao.ipynb
├── raw/
│   ├── dados_empresaA.json
│   └── dados_empresaB.csv
├── refined/
│   └── dados_combinados.csv
└── scripts/
    ├── dados_processados.py
    └── fusao_mercado_fv.py
```

## Competências demonstradas

- ingestão de dados em CSV e JSON;
- separação entre dados brutos e refinados;
- transformação de dados com Python;
- consolidação de datasets;
- análise exploratória com Jupyter;
- organização da lógica de processamento fora do notebook;
- aplicação de conceitos de programação orientada a objetos em fluxos de dados.

## Tecnologias utilizadas

- Python
- Pandas
- Jupyter Notebook
- CSV
- JSON

## Fluxo sugerido de execução

1. inspecionar os arquivos de origem em `pipeline_dados/raw`;
2. executar os scripts em `pipeline_dados/scripts`;
3. analisar o resultado consolidado em `pipeline_dados/refined`;
4. utilizar `pipeline_dados/notebooks/exploracao.ipynb` para análise exploratória.

## Conceitos de Engenharia de Dados

O repositório segue um padrão simples de camadas:

- **Raw** — dados de origem como foram recebidos;
- **Processing** — transformações e regras de consolidação em Python;
- **Refined** — dados tratados e prontos para análise.

Essa separação facilita a compreensão do fluxo, depuração e evolução do pipeline.

## Próximas melhorias

- adicionar arquivo de dependências e ambiente reproduzível;
- criar ponto de entrada por linha de comando;
- adicionar testes automatizados;
- validação de esquema;
- logging estruturado;
- orquestração;
- integração com armazenamento em nuvem;
- pipeline de CI.
