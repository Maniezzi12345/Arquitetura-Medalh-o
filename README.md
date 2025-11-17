# 🏗️ Arquitetura Medallion — Visão Geral

Este projeto implementa a **Arquitetura Medallion** para organização e tratamento de dados em camadas progressivas de qualidade e valor.  
Utilizando **Microsoft Fabric**, **Spark** e **SQL**, os dados são processados em três camadas principais:

---

## 🔹 Bronze — Dados Brutos
- Dados extraídos diretamente de fontes como **APIs** e **arquivos CSV**.  
- Armazenados **sem transformações**, preservando 100% da fidelidade ao dado original.  
- **Objetivo:** servir como base confiável para auditoria e reprocessamentos futuros.

---

## 🔸 Silver — Dados Tratados
- Dados **limpos, estruturados e enriquecidos** utilizando notebooks Spark e SQL.  
- Inclui transformações como **remoção de nulos**, **padronizações**, **joins** e **validações**.  
- **Objetivo:** fornecer dados prontos para análises exploratórias e modelagem.

---

## 🟡 Gold — Dados Refinados
- Dados preparados de forma otimizada para **consumo analítico**.  
- Aplicação de **regras de negócio**, **agregações**, cálculos e métricas finais.  
- **Objetivo:** alimentar dashboards, relatórios e modelos preditivos com alta confiabilidade.

---

## 📐 Modelo Semântico
Criado a partir da camada **Gold** no Microsoft Fabric, contendo:
- Entidades de negócio  
- Relacionamentos  
- Medidas DAX  
- Estrutura optimizada para consumo por ferramentas como **Power BI**

---

## 📊 Regra de Negócio

Este projeto explora a Arquitetura Medallion por meio da:

- **Extração de dados** de uma API (X) e de um arquivo CSV (Y)
- **Foco nos países da União Europeia**
- Aplicação de **limpezas e manipulações básicas** com Spark e SQL  
- Geração de **KPIs** para identificar e analisar possíveis indicadores econômicos e sociais dos países europeus  
- Entrega final orientada para **visualização estratégica** e **tomada de decisão** via Power BI

---

✳️ *O objetivo principal é o aprendizado prático dos conceitos fundamentais da Arquitetura Medallion e sua aplicação em cenários reais de engenharia de dados.*
