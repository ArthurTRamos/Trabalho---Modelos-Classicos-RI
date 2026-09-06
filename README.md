# Modelos Clássicos - RI

**Grupo**:

- Arthur Trottmann Ramos (14681052)
- Maicon Chaves Marques (14593530)

Link de acesso ao relatório: https://docs.google.com/document/d/1QOf_D9bBp5ZXklJE6X1Ski-qcL_V9KzXNavkvrYmSew/edit?usp=sharing

## Descrição

Projeto da disciplina SCC0282 - Recuperação de Informação voltado ao desenvolvimento de métodos de pré-processamento (tokenização, remoção de stopwords e stemming), aplicação de modelos de recuperação de informação tradicionais (BM25 e vetorial) e avaliação a partir de métricas. O dataset utilizado foi o ir_datasets - Cranfield.

## Como rodar

1. Clone o repositório:

```
git clone https://github.com/ArthurTRamos/Trabalho---Modelos-Classicos-RI.git
```

2. Acesse o repositório:

```
cd Trabalho--Modelos-Classicos-RI
```

3. Crie um ambiente virtual Python:

```
python -m venv .venv
```

4. Selecione o ambiente criado como kernel do código ```Trabalho_RI.ipynb```
5. Rode todos os scripts ou apenas células específicas. Bibliotecas e dependências são instaladas na seção de 'Instalação de Dependências e Carregamento de Dataset' através do comando ``` pip install ```

## Linguagem e Bibliotecas

**Linguagem**: Python (3.x)

**Bibliotecas Principais**: NLTK (3.10.3), ir_datasets (0.6.3)

## Identificação e Obtenção da Base de Dados

O dataset Cranfield conta com um corpus textual de 1400 resumos de artigos científicos em inglês. Também conta com mais de 200 consultas e um conjunto-reposta com documentos relevantes a serem considerados para cada consulta. Para carregamento dos dados, foi utilizada a biblioteca ```ir_datasets``` e o método ```load("Cranfield")```. Informações adicionais e formas de manipulação do dataset podem ser encontrados em: https://ir-datasets.com/cranfield.html.
