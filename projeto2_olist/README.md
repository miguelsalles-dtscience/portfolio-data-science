# 🛒 Análise de E-Commerce Brasileiro — Olist Dataset
> Análise exploratória e segmentação de clientes (RFM) sobre 98 mil pedidos do maior marketplace brasileiro — usando Python.

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-blue)
![Dataset](https://img.shields.io/badge/Dataset-Olist%20Brazilian%20E--Commerce-orange)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen)

---

## 🎯 Objetivo

Extrair insights de negócio acionáveis a partir de um dataset real de e-commerce: entender sazonalidade de receita, desempenho por categoria, satisfação de clientes e segmentar a base usando a metodologia RFM (Recência, Frequência, Valor).

---

## 📌 Principais Insights

| Indicador | Resultado |
|-----------|-----------|
| Pedidos analisados | **98.207** (out/2016 – ago/2018) |
| Receita total | **R$ 14,6 milhões** |
| Ticket médio | **R$ 149,01** |
| Avaliação média | **3,75 / 5,0** ★ |
| Tempo médio de entrega | **11,1 dias** |
| Clientes satisfeitos (nota ≥ 4) | **65,1%** |
| Melhor mês | **Novembro/2017** — R$ 1,0M (Black Friday) |

### Destaques da análise

**Sazonalidade:**
A receita cresceu de forma consistente ao longo de 2017, com pico expressivo em novembro (Black Friday + antecipação de Natal). Estratégias de estoque e logística devem prever esse pico com 45–60 dias de antecedência.

**Categorias:**
Cama/mesa/banho, móveis/decoração e informática concentram ~31% da receita total. São categorias com alto ticket médio e alta frequência — prioritárias para campanhas de retenção.

**Satisfação:**
24,9% de clientes insatisfeitos (nota ≤ 2) é um número crítico. Correlaciona diretamente com tempo de entrega acima de 15 dias — especialmente na região Norte.

**Logística:**
A região Norte tem tempo médio de entrega 2,5× maior que o Sudeste. Isso impacta diretamente a satisfação e o LTV dos clientes nessa região.

---

## 🧠 Segmentação RFM

A análise RFM classifica clientes em 4 segmentos baseados em comportamento de compra:

| Segmento | % da Base | Estratégia Recomendada |
|----------|-----------|------------------------|
| **Champions** | ~24% | Programa de fidelidade, acesso antecipado a promoções |
| **Leais** | ~23% | Up-sell e cross-sell com produtos complementares |
| **Potencial** | ~29% | Campanhas de reativação, cupons de segunda compra |
| **Em risco** | ~23% | Win-back com desconto agressivo antes do churn definitivo |

---

## 📁 Estrutura do Projeto

```
projeto2_olist/
│
├── src/
│   └── analise.py              # Script principal (EDA + RFM)
│
├── outputs/
│   ├── analise_ecommerce_painel.png   # Painel: receita, categorias, notas, entrega
│   └── rfm_segmentacao.png            # Segmentação RFM: distribuição e valor médio
│
└── README.md
```

---

## 📊 Visualizações

### Painel Principal (2×2)
1. **Receita mensal** com anotação do pico sazonal
2. **Top 10 categorias** por receita total
3. **Distribuição de avaliações** (1–5 estrelas)
4. **Tempo de entrega** por grande região

### Painel RFM
1. **Pizza** de distribuição dos segmentos
2. **Barras** de valor médio por segmento

---

## 🛠️ Como Executar

```bash
# 1. Clone o repositório
git clone https://github.com/MSallesR/portfolio-data-science
cd portfolio-data-science/projeto2_olist

# 2. Instale as dependências
pip install pandas numpy matplotlib seaborn

# 3. Execute a análise
python src/analise.py
```

> **Nota:** O dataset é gerado sinteticamente com distribuições baseadas nas estatísticas reais publicadas do Olist Brazilian E-Commerce (Kaggle). Para usar os microdados reais, baixe o dataset em [kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) e adapte a seção de leitura do script.

---

## 🔧 Tecnologias

- **pandas** — limpeza, agregação e análise exploratória
- **matplotlib / seaborn** — visualizações de negócio
- **numpy** — geração de dados e operações numéricas
- **RFM Analysis** — segmentação comportamental de clientes

---

## 📚 Referências

- [Olist Brazilian E-Commerce Dataset — Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)
- [RFM Analysis for Customer Segmentation](https://clevertap.com/blog/rfm-analysis/)

---

## 👤 Autor

**Miguel Salles Reis**
Estudante de Estatística — UFMG | Desenvolvedor Python
[github.com/MSallesR](https://github.com/MSallesR) · miguelsallesreis@gmail.com
