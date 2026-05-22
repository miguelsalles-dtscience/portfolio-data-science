# 📊 Análise do Mercado de Trabalho Brasileiro
> Exploração da PNAD Contínua (IBGE) com foco em desocupação, desigualdades regionais e retorno educacional — usando Python.

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-blue)
![Fonte](https://img.shields.io/badge/Fonte-IBGE%20PNAD%20Contínua-green)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

---

## 🎯 Objetivo

Analisar a evolução do desemprego no Brasil entre 2022 e 2024, identificando padrões regionais, gaps de gênero/raça e o impacto da escolaridade na empregabilidade e renda, além de trazer perspectivas com gráficos que normalmente passam despercebidas pela população — com dados reais da PNAD Contínua via API SIDRA/IBGE.

---

## 📌 Principais Insights

| Taxa de desocupação (4ºT2024) | **6,1%** — menor desde 2012 |
| Queda no período analisado | **−5,0 p.p.** entre 1ºT2022 e 4ºT2024 |
| Maior desemprego regional | Nordeste: **10,2%** |
| Menor desemprego regional | Sul: **3,8%** |
| Gap mulheres vs homens | **+3,6 p.p.** de desocupação |
| Premium salarial do ensino superior | **3,7× maior** que sem instrução |

### Destaques da análise
- A queda de 5 pontos percentuais no desemprego em 2 anos é expressiva, mas **esconde desigualdades regionais gritantes** — o Nordeste tem taxa 2,7× maior que o Sul.
- Mulheres negras concentram o pior cenário: **11,8% de desocupação** e rendimento médio de R$1.720 — versus R$3.650 para homens brancos.
- O **retorno educacional é não-linear**: ensino médio incompleto tem desemprego *maior* que fundamental completo, sugerindo que abandono escolar no médio é um ponto crítico.

---

## 📁 Estrutura do Projeto

```
projeto1_mercado_trabalho/
│
├── src/
│   └── analise.py          # Script principal de análise
│
├── outputs/
│   ├── analise_mercado_trabalho.png     # Painel: série temporal + regional + escolaridade
│   └── desigualdades_genero_raca.png    # Painel: desocupação e renda por grupo
│
└── README.md
```

---

## 📊 Visualizações

### Painel Principal
- Evolução trimestral da taxa de desocupação (2022–2024) -- Gráfico 1
- Desocupação por grande região com destaque para máximo/mínimo -- Gráfico 2
- Relação entre escolaridade, desemprego e rendimento médio -- Gráfico 3

### Painel de Desigualdades
- Taxa de desocupação por gênero × raça/cor
- Rendimento médio por gênero × raça/cor

---

## 🛠️ Como Executar

```bash
# 1. Clone o repositório
git clone https://github.com/miguelsalles-dtscience/portfolio-data-science
cd portfolio-data-science/projeto1_mercado_trabalho

# 2. Instale as dependências
pip install pandas numpy matplotlib seaborn requests

# 3. Execute a análise
python src/analise.py
```

> **Nota:** O script tenta buscar dados diretamente da API SIDRA/IBGE. Caso a API esteja indisponível, utiliza automaticamente a série histórica embutida com os valores reais publicados pelo IBGE.

---

## 🔧 Tecnologias

- **pandas** — manipulação e agregação de dados
- **matplotlib / seaborn** — visualizações estáticas personalizadas
- **requests** — coleta via API REST (SIDRA/IBGE)
- **numpy** — operações numéricas com funções da biblioteca

---

## 📚 Fonte dos Dados

- [IBGE — PNAD Contínua](https://www.ibge.gov.br/estatisticas/sociais/trabalho/9173-pesquisa-nacional-por-amostra-de-domicilios-continua-trimestral.html)
- API SIDRA: `https://apisidra.ibge.gov.br` — Tabela 6381 (Taxa de desocupação)

---

## 👤 Autor

**Miguel Salles Reis**
Estudante de Estatística — UFMG | Desenvolvedor Python
[github.com/MSallesR](https://github.com/miguelsalles-dtscience) · miguelsalles.dtscience@gmail.com
