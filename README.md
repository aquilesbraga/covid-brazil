![Python](https://img.shields.io/badge/Python-3.10%2B-blue)

# Perfil Clínico de Mortalidade por COVID-19 no Brasil

Análise exploratória de dados simulados com perfil clínico de pacientes hospitalizados por COVID-19 no Brasil, investigando os fatores associados ao risco de óbito.

## Pergunta de negócio

**Quais fatores clínicos e demográficos mais influenciam a mortalidade por COVID-19?**

## Tecnologias utilizadas

- Python 3.10+
- Pandas
- NumPy
- Plotly (visualização interativa)
- SciPy (teste estatístico qui-quadrado)
- Jupyter Notebook

## Como executar

1. Clone o repositório e acesse a pasta do projeto:
   ```bash
   git clone https://github.com/seu-usuario/covid-clinical-profile-brazil.git
   cd covid-clinical-profile-brazil
   ```

2. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/macOS
   # ou
   venv\Scripts\activate      # Windows
   pip install -r requirements.txt
   ```

3. Execute o notebook:
   ```bash
   jupyter notebook notebooks/analysis.ipynb
   ```

## Principais insights

> *Análise pendente — os resultados serão gerados após a execução do notebook.*

Os insights esperados incluem:

1. Relação entre faixa etária e taxa de mortalidade
2. Impacto de comorbidades no risco de óbito
3. Diferença de mortalidade entre sexos
4. Associação entre internação em UTI e desfecho
5. Significância estatística das diferenças observadas

## Sobre o autor

Analista de dados em transição de carreira, com formação e experiência prévia na área da saúde. Esta análise combina o conhecimento clínico com ferramentas de ciência de dados para gerar insights relevantes para a saúde pública.
