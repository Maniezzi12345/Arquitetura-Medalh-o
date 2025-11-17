🏗️ Arquitetura Medallion — Visão Geral
Este projeto implementa a arquitetura Medallion para organização e tratamento de dados em camadas progressivas de qualidade e valor. Utilizando Microsoft Fabric, Spark e SQL, os dados são processados em três camadas principais:

🔹 Bronze
Dados brutos extraídos de fontes como APIs e arquivos CSV.

Armazenamento sem transformações, preservando fidelidade ao dado original.

Objetivo: servir como base confiável para auditoria e reprocessamento.

🔸 Silver
Dados tratados e estruturados com notebooks Spark e SQL.

Aplicação de limpezas, joins, enriquecimentos e validações.

Objetivo: fornecer dados prontos para análises exploratórias e modelagens.

🟡 Gold
Dados refinados e otimizados para consumo analítico.

Aplicação de regras de negócio específicas, agregações e métricas.

Objetivo: alimentar dashboards, relatórios e modelos preditivos com dados confiáveis.

📐 Modelo Semântico
Construído a partir da camada Gold no Microsoft Fabric.

Representa entidades de negócio, medidas e relacionamentos.

Facilita o consumo dos dados por ferramentas como Power BI.

📊 Regra de Negócio
Este projeto tem como objetivo explorar a arquitetura Medallion por meio da extração de dados de uma API (X) e de um arquivo CSV (Y),
focando em informações sobre países da União Europeia. A proposta é realizar limpezas simples e manipulações básicas utilizando notebooks com Spark e SQL, 
permitindo o aprendizado prático dos conceitos fundamentais da arquitetura em camadas.A partir dos dados tratados, são gerados KPIs que ajudam a identificar e 
analisar possíveis indicadores econômicos e sociais dos países europeus, oferecendo insights relevantes para tomada de decisão e visualização estratégica via Power BI.
