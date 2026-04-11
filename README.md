# 📊 Análise de Vendas com Python

Este projeto tem como objetivo analisar dados de vendas para identificar padrões de comportamento e os principais fatores que influenciam o faturamento.

A análise foi desenvolvida utilizando Python no Google Colab, com foco em gerar insights de negócio a partir de dados reais.

---

## 🎯 Problema de Negócio

A empresa busca entender melhor o desempenho de suas vendas, com foco em responder às seguintes questões:

* O preço dos produtos influencia a quantidade vendida?
* Existem regiões que geram mais faturamento?
* A receita está concentrada em poucos produtos?

---

## 🧠 Hipóteses

1 - Produtos mais caros vendem menos?

2 - Regiões influenciam faturamento?

3 - Existe concentração de receita por produto?

---

## 📂 Dataset

O dataset contém informações de vendas, incluindo:

* Data da venda
* Produto
* Categoria
* Marca
* Preço unitário (`PrecoUnitario`)
* Custo unitário (`CustoUnitario`)
* Quantidade vendida (`Qtd_Vendida`)
* Cliente
* País e continente

---

## 🔧 Engenharia de Dados

Foi criada uma nova variável "Faturamento" para análise de receita:

``python``

df["Faturamento"] = df["PrecoUnitario"] * df["Qtd_Vendida"]

``python``

---

## 🛠️ Tecnologias Utilizadas

* Python
* Pandas
* Matplotlib
* Seaborn
* Google Colab

---

## 📊 Análises Realizadas

### 📉 1. Relação entre Preço e Quantidade

* Gráfico de dispersão (scatter plot)
* Cálculo de correlação

**Resultado:**

* Correlação ≈ **-0.0087**

**Interpretação:**
Não existe relação significativa entre preço e quantidade vendida.

---

### 🌍 2. Faturamento por Região

* Agrupamento por continente
* Visualização em gráfico de barras

**Interpretação:**
Algumas regiões concentram maior faturamento, indicando influência geográfica nas vendas.

---

### 🏆 3. Concentração de Receita (Pareto)

* Ranking de faturamento por produto
* Identificação dos principais produtos

**Interpretação:**
Poucos produtos concentram grande parte da receita total.

---

### 📈 4. Matriz de Correlação

Correlação entre variáveis principais:

| Relação                   | Correlação |
| ------------------------- | ---------- |
| Preço vs Quantidade       | -0.0087    |
| Preço vs Faturamento      | 0.75       |
| Quantidade vs Faturamento | 0.38       |

---

## 🧠 Principais Percepções

* O faturamento é fortemente influenciado pelo preço dos produtos
* A quantidade vendida tem impacto moderado na receita
* Não há evidência de sensibilidade ao preço
* Existe concentração de receita em poucos produtos
* O modelo de negócio é orientado a valor (ticket alto)

---

## 📌 Conclusão

A análise demonstra que o faturamento da empresa é impulsionado principalmente pelo valor dos produtos, e não pelo volume de vendas.

A baixa sensibilidade ao preço sugere oportunidades para estratégias de aumento de margem e posicionamento premium.

---

## 💡 Recomendações de Negócio

* Priorizar produtos de maior valor agregado
* Testar estratégias de aumento de preço
* Investir em produtos premium
* Direcionar esforços para regiões mais lucrativas
* Otimizar o portfólio com foco em produtos de maior retorno

---

## 🚀 Possíveis Evoluções

* Análise de lucro e margem
* Criação de dashboard interativo (Streamlit)
* Modelos preditivos de vendas
* Segmentação por cliente ou região

---

## 📎 Como Executar

1. Acesse o notebook no Google Colab
2. Faça upload do arquivo `Vendas.CSV`
3. Execute as células

---

## 💼 Sobre o Projeto

Este projeto foi desenvolvido com foco em prática de análise de dados, aplicando conceitos de:

* Análise exploratória de dados (EDA)
* Visualização de dados
* Estatística básica

---
