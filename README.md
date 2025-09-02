# Análise e Predição de Dados Cinematográficos

## Proposta de Valor (PDV)

Este projeto entrega valor ao transformar dados brutos de filmes em insights acionáveis para a tomada de decisão estratégica de estúdios cinematográficos. Através de análises detalhadas e modelagem preditiva, é possível:

-   Identificar os fatores que mais influenciam o sucesso de um filme (faturamento, nota, público-alvo, gênero, elenco, etc.)
-   Recomendar características ideais para o próximo lançamento, aumentando as chances de sucesso comercial e de crítica
-   Prever a nota do IMDB de novos filmes antes do lançamento, reduzindo riscos e otimizando investimentos
-   Apoiar decisões baseadas em dados, tornando o processo de escolha do próximo filme mais objetivo e eficiente

Assim, o projeto contribui diretamente para maximizar o retorno sobre o investimento e o impacto dos lançamentos do estúdio.

## Estrutura do Projeto

```
.
├── analise_cinema.ipynb         # Notebook principal com toda a análise e modelagem
├── README.md                    # Este arquivo
├── requirements.txt             # Dependências do projeto
├── data/
│   └── desafio_indicium_imdb.csv  # Base de dados utilizada
└── modelos/
	 └── modelo_imdb.pkl            # Modelo treinado salvo
```

## Pré-requisitos

-   Python 3.8 ou superior
-   pip (gerenciador de pacotes Python)
-   Recomenda-se o uso de um ambiente virtual (venv, conda, etc.)

## Instalação

1. **Clone o repositório ou baixe os arquivos do projeto.**

2. **Crie e ative um ambiente virtual (opcional, mas recomendado):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/Mac
    venv\Scripts\activate     # Windows
    ```

3. **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

## Execução

1. **Abra o Jupyter Notebook:**

    ```bash
    jupyter notebook
    ```

    Ou, se preferir, utilize o Jupyter Lab:

    ```bash
    jupyter lab
    ```

2. **Navegue até o arquivo `analise_cinema.ipynb` e execute as células em ordem.**

    - O notebook realiza:
        - Carregamento e limpeza dos dados
        - Análise exploratória e visualizações
        - Geração de insights para o negócio
        - Construção e avaliação de um modelo de regressão (Random Forest) para prever a nota do IMDB
        - Salvamento do modelo treinado em `modelos/modelo_imdb.pkl`

3. **Personalize e teste o modelo:**
    - Você pode alterar as características do filme de exemplo no final do notebook para prever a nota do IMDB de outros filmes.

## Sobre os Dados

O arquivo `data/desafio_indicium_imdb.csv` contém informações sobre filmes, como título, ano de lançamento, classificação etária, duração, gênero, nota do IMDB, meta score, diretor, elenco, número de votos e faturamento.

## Resultados

-   O notebook apresenta insights sobre os fatores que influenciam o sucesso de um filme.
-   O modelo preditivo atinge um RMSE baixo, indicando boa precisão para prever a nota do IMDB.

## Observações

-   O projeto pode ser expandido com novas fontes de dados, melhorias no modelo e análises de NLP na coluna de sinopse dos filmes.
-   Sinta-se à vontade para contribuir ou sugerir melhorias!
