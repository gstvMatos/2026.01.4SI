# FireWatch AI
## Inteligência Espacial para Análise e Monitoramento de Queimadas no Brasil

## Sobre o Projeto

O FireWatch AI é um projeto de Ciência de Dados desenvolvido com o objetivo de analisar padrões geográficos e temporais relacionados à ocorrência de queimadas no Brasil.

Utilizando dados oficiais do Programa Queimadas do INPE, foram aplicadas técnicas de Análise Exploratória de Dados (EDA), Clusterização (K-Means) e Machine Learning para identificar regiões críticas, padrões sazonais e características espaciais associadas aos focos de calor registrados por satélites ambientais.

---

## Problema

As queimadas representam um dos principais desafios ambientais do Brasil, causando impactos significativos na biodiversidade, qualidade do ar, saúde pública, agricultura e economia.

Segundo o INPE, o Brasil registrou mais de 278 mil focos de queimadas em 2024, representando um crescimento de aproximadamente 46,5% em relação a 2023.

Diante desse cenário, este projeto busca responder:

> Existem padrões geográficos e temporais capazes de auxiliar na identificação de regiões mais vulneráveis às queimadas?

---

## Base de Dados

Os dados utilizados foram obtidos através do Programa Queimadas do Instituto Nacional de Pesquisas Espaciais (INPE).

Fonte Oficial:

https://data.inpe.br/queimadas/dados-abertos/

Arquivos utilizados:

- focos_br_ref_2023.zip
- focos_br_ref_2024.zip
- focos_br_ref_2025.zip

---

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab
- GitHub

---

## Hipóteses Investigadas

### Hipótese 1
Determinados estados concentram maior número de queimadas.

### Hipótese 2
Existem biomas mais vulneráveis às queimadas.

### Hipótese 3
Existe sazonalidade na ocorrência das queimadas.

### Hipótese 4
Existem padrões geográficos de concentração de focos.

### Hipótese 5
Técnicas de clusterização podem auxiliar na identificação de regiões críticas.

---

## Modelagem de Machine Learning

Foi desenvolvido um modelo supervisionado utilizando:

- Random Forest Classifier

Objetivo:

Prever o bioma de ocorrência de um foco de calor a partir das coordenadas geográficas (latitude e longitude).

### Métricas Obtidas

- Accuracy: ~99%
- Precision média: ~99%
- Recall médio: ~99%
- F1-Score médio: ~99%

Também foi realizada avaliação através de:

- Matriz de Confusão
- Relatório de Classificação

---

## Principais Resultados

### Distribuição por Estado

Os estados com maior número de focos registrados foram:

1. Pará
2. Mato Grosso
3. Maranhão
4. Amazonas
5. Tocantins

---

### Distribuição por Bioma

Os biomas mais impactados foram:

1. Amazônia
2. Cerrado
3. Caatinga

---

### Sazonalidade

Os focos de queimadas apresentam forte concentração entre os meses de agosto e outubro, indicando comportamento sazonal bem definido.

---

### Clusterização

A aplicação do algoritmo K-Means identificou cinco agrupamentos geográficos distintos.

Os resultados demonstraram que os focos de queimadas não estão distribuídos de forma homogênea pelo território brasileiro, concentrando-se principalmente em regiões associadas aos biomas Amazônia e Cerrado.

---

## Estrutura do Repositório

```text
.
├── README.md
├── FireWatch_AI.ipynb
├── focos_br_ref_2023.zip
├── focos_br_ref_2024.zip
└── focos_br_ref_2025.zip
```

---

## Como Executar

### 1. Baixar os arquivos

Faça o download dos arquivos ZIP disponibilizados neste repositório.

### 2. Extrair os arquivos

Extraia os arquivos para uma pasta local de sua preferência.

### 3. Configurar os caminhos

No notebook, informe o caminho dos arquivos:

```python
# Informe abaixo os caminhos dos datasets

url_2023 = ''
url_2024 = ''
url_2025 = ''

df_2023 = pd.read_csv(url_2023)
df_2024 = pd.read_csv(url_2024)
df_2025 = pd.read_csv(url_2025)
```

### 4. Executar o notebook

Execute as células sequencialmente para reproduzir toda a análise, visualizações e resultados do projeto.

---

Projeto desenvolvido para a disciplina de Visão Computacional e Machine Learning — FIAP.

---
