# 📊 Dashboard de Salários na Área de Dados

Dashboard interativo desenvolvido em Python para explorar e analisar informações sobre salários no mercado de trabalho da área de Dados. O projeto permite visualizar indicadores, comparar remunerações e identificar tendências de acordo com diferentes características profissionais.

🔗 **Acesse o dashboard:** [Relatório de Dados Python](https://relatorio-de-dados-python.streamlit.app/)

## 🎯 Objetivo

O objetivo deste projeto é facilitar a visualização e a análise do mercado de trabalho na área de Dados, utilizando gráficos interativos e indicadores que ajudam a compreender a distribuição salarial e as características das oportunidades profissionais.

## 🚀 Funcionalidades

O dashboard oferece filtros interativos e diferentes visualizações para explorar os dados:

- **Filtros dinâmicos:** seleção por ano, senioridade, tipo de contrato e tamanho da empresa.
- **Salário médio:** visualização da média salarial anual em dólares.
- **Maior salário:** identificação do maior salário presente nos dados filtrados.
- **Total de registros:** quantidade de registros disponíveis após a aplicação dos filtros.
- **Cargo mais frequente:** identificação do cargo com maior ocorrência.
- **Top 10 cargos:** comparação dos cargos com as maiores médias salariais.
- **Distribuição salarial:** histograma para visualizar a distribuição dos salários.
- **Tipos de trabalho:** comparação entre modalidades remotas e presenciais.
- **Análise geográfica:** visualização da média salarial de Cientistas de Dados por país.
- **Tabela detalhada:** consulta aos registros após a aplicação dos filtros.

## 🛠️ Tecnologias utilizadas

| Tecnologia | Finalidade |
|---|---|
| Python | Linguagem de programação |
| Streamlit | Desenvolvimento da interface interativa |
| Pandas | Manipulação e análise dos dados |
| Plotly Express | Criação de gráficos interativos |

## 📂 Estrutura do projeto

```text
dados-python-main/
│
├── .devcontainer/
│   └── devcontainer.json
│
├── app.py
├── dados-final.csv
├── requirements.txt
└── README.md
```

## ⚙️ Como executar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/SEU-USUARIO/dados-python.git
```

### 2. Acesse a pasta do projeto

```bash
cd dados-python
```

### 3. Crie um ambiente virtual

```bash
python -m venv venv
```

### 4. Ative o ambiente virtual

**Windows:**

```bash
venv\Scripts\activate
```

**Linux / macOS:**

```bash
source venv/bin/activate
```

### 5. Instale as dependências

```bash
pip install -r requirements.txt
```

### 6. Execute o dashboard

```bash
streamlit run app.py
```

Após executar o comando, acesse o endereço disponibilizado pelo Streamlit no navegador, normalmente:

```text
http://localhost:8501
```

## 📈 Fonte dos dados

O dashboard utiliza uma base de dados sobre salários de profissionais da área de Dados, disponibilizada em formato CSV.

Os dados incluem informações como:

- Ano de referência;
- Nível de senioridade;
- Tipo de contrato;
- Cargo;
- Salário;
- Moeda;
- Salário convertido para USD;
- País de residência;
- Modalidade de trabalho;
- Localização da empresa;
- Tamanho da empresa.

A aplicação atualmente carrega os dados diretamente de um arquivo CSV hospedado no GitHub.

## 📌 Observações

Os valores salariais apresentados no dashboard estão expressos em dólares americanos (USD).

Os resultados e indicadores são atualizados conforme os filtros selecionados pelo usuário.

---

**Desenvolvido com Python, Pandas, Streamlit e Plotly.**
