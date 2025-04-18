# 🧹 Limpeza e Tratamento de Dados - Clientes de Telecom

Este repositório contém um notebook Jupyter com um pipeline de **limpeza, transformação e preparação de dados** de clientes de uma empresa de telecomunicações. O foco é preparar os dados para análises futuras , como modelagem preditiva de churn (cancelamento).

---

## 📦 Dataset

O dataset utilizado está no formato `.json` e contém dados aninhados com informações sobre:
- Dados do cliente (gênero, tempo de serviço, parceiro, dependentes)
- Serviços contratados (telefone, internet, streaming, suporte, etc.)
- Informações de cobrança (tipo de contrato, pagamento, valor mensal e total)
- Indicador de **Churn** (cancelamento)

---

## 🧪 Objetivo do notebook

O notebook `limpeza_tratamento.ipynb` realiza:

1. 📥 **Carregamento e normalização do JSON**
   - Conversão dos dados aninhados para um DataFrame plano (flat).
2. 🧼 **Tratamento de valores ausentes**
   - Identificação e imputação de valores `null`.
3. 📊 **Tratamento de tipos de dados**
   - Conversão de strings para numéricos (ex: valores de cobrança).
4. 📈 **Criação de variáveis**
   - Cálculo do tempo de serviço estimado com base em cobrança total / mensal.
5. 🧹 **Remoção de outliers**
   - Identificação via IQR e correção ou remoção seletiva.
6. 🧠 **Codificação de variáveis categóricas**
   - Aplicação de `pd.get_dummies()` para permitir modelagem posterior.
7. 📉 **Análise exploratória leve**
   - Inspeção visual e estatística básica dos dados.

---
