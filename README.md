# Perfil Clínico de Mortalidade por COVID-19 no Brasil

Análise exploratória de dados simulados com perfil clínico de pacientes hospitalizados por COVID-19, investigando os fatores associados ao risco de óbito.

## 1. Objetivo do Projeto

Responder à pergunta: **"Quais fatores clínicos e demográficos mais influenciam a mortalidade por COVID-19?"** A partir de dados realistas simulados de 5.000 pacientes, o projeto investiga como idade, sexo, comorbidades (diabetes, cardiopatia, obesidade, doença respiratória) e internação em UTI se associam ao risco de óbito. A análise busca gerar evidências que possam orientar políticas públicas e alocação de recursos hospitalares.

## 2. Resultado Obtido

Um notebook Jupyter completo com:
- **Geração de dados sintéticos** calibrados para refletir padrões epidemiológicos reais (mortalidade crescente com idade, maior risco em homens e portadores de comorbidades)
- **Quatro visualizações interativas** com Plotly: taxa de mortalidade por faixa etária, impacto de cada comorbidade, análise por sexo e faixa etária, e associação com internação em UTI
- **Teste estatístico qui-quadrado** (SciPy) confirmando associação significativa entre presença de comorbidades e maior mortalidade (p < 0,05)
- **Cinco conclusões principais** sintetizadas em linguagem clara para tomadores de decisão

## 3. Ferramentas Utilizadas

- **Python 3.10+** — linguagem principal
- **Pandas** — manipulação, agregação e tabulação cruzada dos dados
- **NumPy** — geração dos dados sintéticos (distribuições binomial, choice, randint) e modelagem logística
- **Plotly** (Express + Graph Objects) — visualizações interativas com barras e gradientes de cor
- **SciPy** — teste qui-quadrado de independência (`chi2_contingency`)
- **Jupyter Notebook** — ambiente de desenvolvimento e documentação

## 4. O que Aprendi

- Simular conjuntos de dados realistas usando numpy com calibração baseada em conhecimento do domínio (modelo logístico para probabilidade de óbito)
- Construir uma narrativa analítica completa: da pergunta de negócio → geração dos dados → exploração visual → teste estatístico → conclusões acionáveis
- Aplicar e interpretar o teste qui-quadrado de independência, incluindo a comunicação do significado do p-valor em linguagem acessível
- Criar visualizações comparativas eficazes com Plotly (barras agrupadas, gradientes de cor, hover interactions)
- Documentar o raciocínio analítico em cada etapa do notebook, conectando os achados à literatura científica sobre COVID-19

## 5. Melhorias Futuras

- Substituir dados simulados por dados reais do SIVEP-Gripe (SRAG) para validar os achados
- Incorporar análise temporal (séries históricas por onda da pandemia)
- Desenvolver um modelo preditivo de risco individual (regressão logística ou random forest)
- Incluir análise por região geográfica e disponibilidade de leitos de UTI
- Criar um dashboard interativo com Streamlit para explorar os dados dinamicamente
- Expandir para outras variáveis: raça/cor, escolaridade, vacinação
