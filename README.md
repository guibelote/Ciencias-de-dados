# Projeto: Portfólio de Ciência de Dados

**Resumo**
Projeto pronto para subir no GitHub com datasets realistas, notebooks de exemplo e instruções para rodar localmente.

## Estrutura do repositório
```
/data
  /modulo2_vendas
    - base_vendas_suja.csv
    - base_vendas_suja.xlsx
  /modulo5_estatistica
    - notas_alunos.csv
    - notas_alunos.xlsx
  /modulo6_regressao
    - casas.csv
    - casas.xlsx
  /modulo8_ml
    - clientes.csv
    - clientes.xlsx
  /modulo10_nlp
    - tweets.csv
    - tweets.xlsx
/notebooks
  - modulo2_vendas.ipynb
  - modulo5_estatistica.ipynb
  - modulo6_regressao.ipynb
  - modulo8_ml.ipynb
  - modulo10_nlp.ipynb
README.md
.gitignore
```

## Descrição dos módulos e datasets

### Módulo 2 - Vendas
Dataset `base_vendas_suja` com:
- pedidos (order_id, order_date)
- cliente, cidade (textos despadronizados)
- produto com variações textuais
- preço, quantidade (contém valores ausentes e outliers)
- duplicatas e anotações inconsistentes

Útil para tarefas de limpeza, manipulação de datas, deduplicação e análise exploratória.

### Módulo 5 - Estatística
Dataset `notas_alunos` com:
- identificador e nome do aluno (vários formatos)
- notas de duas provas e nota final (contém valores ausentes, valores inválidos e duplicatas)
- ideal para exercícios de estatística descritiva, tratamento de valores inválidos e imputação

### Módulo 6 - Regressão
Dataset `casas` com características de imóveis:
- área (m2), quartos, banheiros, ano de construção, endereço, preço
- contém outliers, valores ausentes e duplicatas
- ideal para modelos de regressão e engenharia de features

### Módulo 8 - Machine Learning
Dataset `clientes` com informações:
- client_id, nome, email (formatos inconsistentes), idade, assinatura, última atividade, churn
- contém valores ausentes, duplicatas e categorias despadronizadas
- ideal para classificação de churn, engenharia de features categóricas e validação

### Módulo 10 - NLP
Dataset `tweets` com:
- tweet_id, usuário, texto bruto, timestamp
- textos despadronizados, emojis, pontuação excessiva, duplicatas e valores nulos
- ideal para pré-processamento de texto, análise de sentimento e tokenização

## Como rodar o projeto localmente
1. Clone o repositório:
```bash
git clone <seu-repo>.git
cd <seu-repo>
```

2. Recomenda-se criar um ambiente virtual:
```bash
python -m venv .venv
source .venv/bin/activate   # macOS / Linux
.\.venv\Scripts\activate  # Windows
pip install -r requirements.txt
```

3. Abra os notebooks em Jupyter Lab / Notebook:
```bash
jupyter lab
```
Os notebooks usam caminhos relativos (`data/...`) e conseguem abrir automaticamente CSV ou XLSX.

## Notas
- Os datasets aqui são fictícios, mas realistas — adequados para portfólio.
- Modifique e complemente os notebooks com suas análises, gráficos e modelos antes de subir no GitHub.
