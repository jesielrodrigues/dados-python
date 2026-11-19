<h1 align="center">📊 Dashboard de Carreira, Mercado e Análise de Dados</h1>

<p align="center">
  Explore mais de <b>133 mil registros</b> de salários da área de dados com filtros interativos e gráficos dinâmicos.
</p>

<p align="center">
  <a href="https://relatorio-de-dados-python.streamlit.app/"><img src="https://img.shields.io/badge/🚀_Ver_dashboard_ao_vivo-FF4B4B?style=for-the-badge" alt="Ver dashboard ao vivo"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Streamlit-1.44.1-FF4B4B?logo=streamlit&logoColor=white" alt="Streamlit">
  <img src="https://img.shields.io/badge/Plotly-5.24.1-3F4F75?logo=plotly&logoColor=white" alt="Plotly">
  <img src="https://img.shields.io/badge/Pandas-2.2.3-150458?logo=pandas&logoColor=white" alt="Pandas">
</p>

<p align="center">
  <a href="https://relatorio-de-dados-python.streamlit.app/">
    <img src="assets/dashboard.png" alt="Prévia do dashboard de salários na área de dados" width="100%">
  </a>
</p>

---

## 🎯 Sobre o projeto

Este projeto é um **dashboard interativo** construído com **Streamlit** e **Plotly** para analisar salários na área de dados ao longo dos últimos anos (2020 a 2025).

Com ele é possível responder perguntas como:

- Quais cargos pagam melhor, em média?
- Como os salários se distribuem entre faixas?
- Qual a proporção entre trabalho presencial, híbrido e remoto?
- Quanto ganha, em média, um(a) Cientista de Dados em cada país?

Tudo isso podendo recortar os dados por **ano**, **senioridade**, **tipo de contrato** e **tamanho da empresa**.

## ✨ Funcionalidades

- 🔍 **Filtros na barra lateral:** ano, senioridade, tipo de contrato e tamanho da empresa.
- 📈 **Métricas gerais (KPIs):** salário médio, salário máximo, total de registros e cargo mais frequente.
- 📊 **Top 10 cargos por salário médio:** gráfico de barras horizontais.
- 📉 **Distribuição de salários anuais:** histograma com as faixas salariais em USD.
- 🍩 **Proporção dos tipos de trabalho:** gráfico de rosca (presencial, híbrido e remoto).
- 🗺️ **Mapa mundial:** salário médio de Cientista de Dados por país.
- 🗂️ **Tabela detalhada:** todos os registros filtrados, para consulta e exploração.

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| [Python](https://www.python.org/) | Linguagem principal |
| [Streamlit](https://streamlit.io/) | Interface web e filtros |
| [Plotly Express](https://plotly.com/python/plotly-express/) | Gráficos interativos |
| [Pandas](https://pandas.pydata.org/) | Leitura e manipulação dos dados |

## 📁 Estrutura do repositório

```
dados-python/
├── app.py              # Aplicação Streamlit (filtros, KPIs e gráficos)
├── dados-final.csv     # Base de dados de salários
├── requirements.txt    # Dependências do projeto
├── assets/
│   └── dashboard.png   # Print usado neste README
└── .devcontainer/      # Configuração para GitHub Codespaces / Dev Containers
```

## 🗃️ Sobre os dados

A base contém **133.339 registros** com as seguintes colunas:

| Coluna | Descrição |
|---|---|
| `ano` | Ano de referência do salário |
| `senioridade` | Nível de experiência (júnior, pleno, sênior, executivo) |
| `contrato` | Tipo de contrato (integral, parcial, contrato, freelancer) |
| `cargo` | Nome do cargo |
| `salario` / `moeda` | Salário na moeda original |
| `usd` | Salário anual convertido para dólar (USD) |
| `residencia` / `residencia_iso3` | País de residência da pessoa (código ISO-2 e ISO-3) |
| `remoto` | Modelo de trabalho (presencial, híbrido, remoto) |
| `empresa` | País da empresa |
| `tamanho_empresa` | Porte da empresa (pequena, média, grande) |

> **Nota:** o `app.py` carrega o CSV a partir de uma URL pública do GitHub. Para usar o arquivo local `dados-final.csv`, basta trocar o caminho na chamada `pd.read_csv(...)`.

## 🚀 Como executar localmente

**1. Clone o repositório**

```bash
git clone https://github.com/<seu-usuario>/<nome-do-repositorio>.git
cd <nome-do-repositorio>
```

**2. (Opcional) Crie um ambiente virtual**

```bash
python -m venv .venv
source .venv/bin/activate      # Linux/macOS
.venv\Scripts\activate         # Windows
```

**3. Instale as dependências**

```bash
pip install -r requirements.txt
```

**4. Rode o app**

```bash
streamlit run app.py
```

O dashboard abrirá em `http://localhost:8501`.

### ☁️ Alternativa: GitHub Codespaces

O repositório já inclui um `.devcontainer`. Basta abrir no Codespaces e o app é iniciado automaticamente na porta `8501`.

## 🔗 Link do projeto

👉 **[relatorio-de-dados-python.streamlit.app](https://relatorio-de-dados-python.streamlit.app/)**

## 🤝 Contribuindo

Sugestões e melhorias são bem-vindas! Abra uma *issue* ou envie um *pull request*.

---

<p align="center">Feito com 💙 e Python</p>
