
# 📊 Análise RFM em Python

Este repositório contém uma implementação prática de **Análise RFM (Recency, Frequency, Monetary)** utilizando **Python e Pandas**, com foco em segmentação de clientes e geração de insights para estratégias de CRM, marketing e retenção.

O projeto foi desenvolvido com fins **educacionais e analíticos**, simulando um cenário real de base transacional.

---

## 🧠 O que é Análise RFM?

A Análise RFM é uma técnica de segmentação de clientes baseada em três dimensões comportamentais:

* **Recency (R)** – há quanto tempo o cliente realizou a última compra
* **Frequency (F)** – com que frequência o cliente compra
* **Monetary (M)** – quanto dinheiro o cliente gastou no período analisado

A combinação dessas métricas permite identificar clientes mais valiosos, clientes em risco, clientes perdidos e oportunidades de reativação.

---

## 🎯 Objetivo do Projeto

* Aplicar a metodologia RFM em um conjunto de dados transacionais
* Criar **scores R, F e M** utilizando quintis
* Classificar clientes em **segmentos acionáveis**
* Demonstrar uma abordagem clara, reproduzível e alinhada a boas práticas de análise de dados

---

## 🗂️ Estrutura do Projeto

```
📁 AnaliseRFM
 ├── AnaliseRFM.ipynb   # Notebook principal com a análise completa
 └── README.md         # Documentação do projeto
```

---

## 🛠️ Tecnologias Utilizadas

* Python 3
* Pandas
* NumPy
* Jupyter Notebook

---

## 🔎 Etapas da Análise

### 1. Preparação dos Dados

* Leitura do dataset
* Conversão de datas
* Verificação de valores nulos e tipos de dados

### 2. Cálculo das Métricas RFM

As métricas são calculadas por cliente:

* Recency: diferença em dias entre a última compra do cliente e a data de referência
* Frequency: número total de compras
* Monetary: soma do valor gasto

### 3. Criação dos Scores

Cada métrica é transformada em um score de **1 a 5**, utilizando quintis:

* Recency: quanto menor o valor, maior o score
* Frequency e Monetary: quanto maior o valor, maior o score

### 4. Score RFM Consolidado

Os scores são concatenados para formar um identificador único:

```
RFM_Score = R_Score + F_Score + M_Score
```

Exemplo: `545`

### 5. Segmentação de Clientes

Os clientes são classificados em segmentos estratégicos, como:

* **Campeões**
* **Clientes Fiéis**
* **Novos Clientes**
* **Em Risco**
* **Perdidos**

A segmentação considera simultaneamente R, F e M, garantindo uma visão mais fiel do valor do cliente.

---

## 📈 Possíveis Insights de Negócio

* Identificação dos clientes mais valiosos da base
* Ações de retenção para clientes em risco
* Campanhas de reativação para clientes perdidos
* Estratégias de upsell para clientes frequentes com baixo ticket médio

---

## 🚀 Próximos Passos (Evoluções Possíveis)

* Integração com Power BI ou Tableau
* Automatização da análise para dados recorrentes
* Inclusão de métricas como margem ou ticket médio
* Comparação RFM por períodos (cohort analysis)

---

## 👤 Autor

Diego Rodrigues
Profissional com foco em Dados, BI e Analytics

---

## 📌 Observação

Este projeto tem caráter demonstrativo e pode ser adaptado para diferentes contextos de negócio, como e-commerce, SaaS, varejo ou serviços financeiros.

