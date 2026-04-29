# TECH CHALLENGE 1 - PÓS TECH FIAP 📊

> **TECH CHALLENGE 1 - Data Analytics** > Universidade FIAP - 2026

![PowerBI](https://img.shields.io/badge/Python%20-blue)
![Status](https://img.shields.io/badge/Status-Em%20andamento-yellow)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📌 Sobre o Projeto

**Case E-commerce Olist**
Este desafio propõe a construção de um relatório executivo voltado a investidores e acionistas do setor de e-commerce, baseado no Brazilian E-Commerce Public Dataset by Olist. O objetivo é transformar dados transacionais em uma narrativa clara sobre desempenho comercial, eficiência logística e/ou satisfação do cliente, culminando em recomendações acionáveis e, quando possível, previsões fundamentadas.

---

## 📈 Sobre o Dataset

O dataset reúne aproximadamente 100 mil pedidos entre 2016 e 2018, cobrindo múltiplos marketplaces no Brasil. Inclui tabelas interconectadas de clientes, pedidos, itens, produtos, vendedores, pagamentos, avaliações e geolocalização por CEP. Os dados são reais e foram anonimizados. Há possibilidade de análises multidimensionais, como status do pedido, preço, meios de pagamento, desempenho de frete, localização, atributos de produto e reviews. 

O dataset pode ser acessado aqui (https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

## Estrutura dos Dados e Dicionário (visão executiva)

- **customers**: customer_id, customer_unique_id, zip_code_prefix, cidade, estado  
- **orders**: order_id, customer_id, status, timestamps de compra/aprovação/entrega  
- **order_items**: order_id, item_id, product_id, seller_id, shipping_limit_date, price, freight_value  
- **payments**: order_id, payment_type, installments, payment_value  
- **order_reviews**: order_id, review_score, timestamps, review_comment_title/text  
- **products**: product_id, category_name, pesos/medidas, descrição  
- **sellers**: seller_id, zip_code_prefix, cidade, estado  
- **geolocation**: zip_code_prefix, latitude, longitude, cidade, estado  
- **category_translation**: tradução de nomes de categorias para inglês

---

## 📥 Como reproduzir a análise

### 1. Baixe o dataset
Download diretamente do Kaggle:

🔗 [Brazilian E-Commerce Public Dataset by Olist — Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

Após baixar, extraia os arquivos CSV na pasta `data/`. Os arquivos esperados são:

```
data/
├── olist_orders_dataset.csv
├── olist_customers_dataset.csv
├── olist_order_items_dataset.csv
├── olist_order_payments_dataset.csv
├── olist_order_reviews_dataset.csv
├── olist_products_dataset.csv
└── olist_sellers_dataset.csv
```

### 2. Execute o notebook
Abra `notebook/tech_challenge.ipynb` no Google Colab ou Jupyter e execute as células sequencialmente.

```bash
# Ou via terminal com Jupyter
jupyter notebook notebook/tech_challenge.ipynb
```

### 3. Consulte os entregáveis
- **Relatório executivo** em `relatorio/`
- **Painel em PowerBI** em `apresentacao/`

---

## 👥 Integrantes do Grupo

| Nome | RM |
|------|----|
| **Emerson Henrique de Lima e Sousa** | 373751 |
| **Moacyr Souza Barros** | 373412 |

---
