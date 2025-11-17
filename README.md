# 🏗️ Arquitetura Medallion — Pipeline Analítico com Microsoft Fabric

![Arquitetura Medallion](IMAGEM_ARQUITETURA_AQUI)

Este repositório implementa uma solução completa utilizando a **Arquitetura Medallion** para ingestão, tratamento e disponibilização de dados usando **Microsoft Fabric (Lakehouse)**, **Spark**, **SQL**, e consumo final via **Power BI**.

A arquitetura é composta por três camadas — **Bronze**, **Silver** e **Gold** — organizadas para garantir qualidade, rastreabilidade e valor analítico crescente.

---

## 📌 Sumário

- [Visão Geral da Arquitetura](#-visão-geral-da-arquitetura)
- [Camada Bronze](#-bronze--dados-brutos)
- [Camada Silver](#-silver--dados-tratados)
- [Camada Gold](#-gold--dados-refinados)
- [Modelo Semântico](#-modelo-semântico)
- [Regras de Negócio](#-📊-regra-de-negócio)
- [Pipeline (a preencher)](#-pipeline-completo)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)

---

# 🔭 Visão Geral da Arquitetura

![Fluxo Medallion](IMAGEM_FLUXO_AQUI)

A Arquitetura Medallion organiza os dados em camadas com propósitos bem definidos:

- **Bronze** → Ingestão pura  
- **Silver** → Tratamento e padronização  
- **Gold** → Preparação analítica  

Essa abordagem garante:

✔ alta rastreabilidade  
✔ consistência entre camadas  
✔ facilidade para reprocessamento  
✔ governança e qualidade dos dados  
✔ material final otimizado para BI  

---

# 🔹 Bronze — Dados Brutos

![Camada Bronze](IMAGEM_BRONZE_AQUI)

A camada **Bronze** recebe os dados exatamente como chegam da origem.

### ✔ O que é feito nesta camada

- Ingestão direta de:
  - Arquivos **CSV**
  - Dados extraídos via **API**
- Nenhuma transformação aplicada  
- Somente padronização mínima de colunas para permitir leitura  
- Armazenamento no Lakehouse para rastreabilidade

### 🎯 Objetivo

> Preservar a integridade do dado original para auditorias e reprocessamento.

---

# 🔸 Silver — Dados Tratados

![Camada Silver](IMAGEM_SILVER_AQUI)

A camada **Silver** realiza o tratamento e estruturação dos dados usando Spark Notebooks e SQL.

### ✔ O que é feito nesta camada

- Limpeza de nulos  
- Padronização de tipos  
- Padronização de nomes de colunas  
- Correção de formatos inconsistentes  
- Filtragem de registros inválidos  
- União/Junção de tabelas relacionadas  
- Criação de tabelas estruturadas  
- Aplicação de regras de qualidade

### 🎯 Objetivo

> Garantir que os dados estejam consistentes, limpos e prontos para análises exploratórias e cálculos avançados.

---

# 🟡 Gold — Dados Refinados

![Camada Gold](IMAGEM_GOLD_AQUI)

A camada **Gold** é a etapa final de dados preparados para consumo analítico e dashboards.

### ✔ O que é feito nesta camada

- Agregações  
- Cálculos de KPIs finais  
- Métricas econômicas e sociais  
- Tabelas de fatos e dimensões  
- Estruturas otimizadas para Power BI  
- Aplicação das regras de negócio finais

### 🎯 Objetivo

> Entregar dados confiáveis, refinados e de alto valor analítico para o Modelo Semântico e dashboards.

---

# 📐 Modelo Semântico

![Modelo Semântico](IMAGEM_MODELO_AQUI)

A partir da camada **Gold**, foi criado um modelo semântico no Fabric com:

- Entidades organizadas (Dimensões e Fatos)  
- Relacionamentos bem definidos  
- Medidas DAX otimizadas  
- Estrutura adequada para performance em Power BI  

---

# 📊 Regra de Negócio

A solução foi desenvolvida com foco nos **países da União Europeia**, aplicando as seguintes regras:

- Extração de dados via **API X** e **CSV Y**
- Filtragem exclusiva para países da **UE**
- Cálculo de **indicadores sociais e econômicos**
- Padronização e estruturação para análises comparativas
- Criação de KPIs estratégicos para o dashboard final

---

# ⚙️ Pipeline Completo

> 🔧 **(Reserve aqui o espaço para descrever seu pipeline: Bronze → Silver → Gold → Semantic → Power BI.  
> Caso queira, posso preencher automaticamente lendo seus notebooks.)**

---

# 🛠 Tecnologias Utilizadas

- **Microsoft Fabric Lakehouse**
- **PySpark**
- **Spark SQL**
- **Notebooks Fabric**
- **Power BI**
- **Arquitetura Medallion**
- **Git / GitHub**

---

Se quiser que eu gere as **imagens** ou um **diagrama profissional** para substituir os blocos `IMAGEM_..._AQUI`, posso produzir automaticamente!  
Só pedir. 🚀
# 🏗️ Arquitetura Medallion — Pipeline Analítico com Microsoft Fabric

![Arquitetura Medallion](IMAGEM_ARQUITETURA_AQUI)

Este repositório implementa uma solução completa utilizando a **Arquitetura Medallion** para ingestão, tratamento e disponibilização de dados usando **Microsoft Fabric (Lakehouse)**, **Spark**, **SQL**, e consumo final via **Power BI**.

A arquitetura é composta por três camadas — **Bronze**, **Silver** e **Gold** — organizadas para garantir qualidade, rastreabilidade e valor analítico crescente.

---

## 📌 Sumário

- [Visão Geral da Arquitetura](#-visão-geral-da-arquitetura)
- [Camada Bronze](#-bronze--dados-brutos)
- [Camada Silver](#-silver--dados-tratados)
- [Camada Gold](#-gold--dados-refinados)
- [Modelo Semântico](#-modelo-semântico)
- [Regras de Negócio](#-📊-regra-de-negócio)
- [Pipeline (a preencher)](#-pipeline-completo)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)

---

# 🔭 Visão Geral da Arquitetura

![Fluxo Medallion](IMAGEM_FLUXO_AQUI)

A Arquitetura Medallion organiza os dados em camadas com propósitos bem definidos:

- **Bronze** → Ingestão pura  
- **Silver** → Tratamento e padronização  
- **Gold** → Preparação analítica  

Essa abordagem garante:

✔ alta rastreabilidade  
✔ consistência entre camadas  
✔ facilidade para reprocessamento  
✔ governança e qualidade dos dados  
✔ material final otimizado para BI  

---

# 🔹 Bronze — Dados Brutos

![Camada Bronze](IMAGEM_BRONZE_AQUI)

A camada **Bronze** recebe os dados exatamente como chegam da origem.

### ✔ O que é feito nesta camada

- Ingestão direta de:
  - Arquivos **CSV**
  - Dados extraídos via **API**
- Nenhuma transformação aplicada  
- Somente padronização mínima de colunas para permitir leitura  
- Armazenamento no Lakehouse para rastreabilidade

### 🎯 Objetivo

> Preservar a integridade do dado original para auditorias e reprocessamento.

---

# 🔸 Silver — Dados Tratados

![Camada Silver](IMAGEM_SILVER_AQUI)

A camada **Silver** realiza o tratamento e estruturação dos dados usando Spark Notebooks e SQL.

### ✔ O que é feito nesta camada

- Limpeza de nulos  
- Padronização de tipos  
- Padronização de nomes de colunas  
- Correção de formatos inconsistentes  
- Filtragem de registros inválidos  
- União/Junção de tabelas relacionadas  
- Criação de tabelas estruturadas  
- Aplicação de regras de qualidade

### 🎯 Objetivo

> Garantir que os dados estejam consistentes, limpos e prontos para análises exploratórias e cálculos avançados.

---

# 🟡 Gold — Dados Refinados

![Camada Gold](IMAGEM_GOLD_AQUI)

A camada **Gold** é a etapa final de dados preparados para consumo analítico e dashboards.

### ✔ O que é feito nesta camada

- Agregações  
- Cálculos de KPIs finais  
- Métricas econômicas e sociais  
- Tabelas de fatos e dimensões  
- Estruturas otimizadas para Power BI  
- Aplicação das regras de negócio finais

### 🎯 Objetivo

> Entregar dados confiáveis, refinados e de alto valor analítico para o Modelo Semântico e dashboards.

---

# 📐 Modelo Semântico

![Modelo Semântico](IMAGEM_MODELO_AQUI)

A partir da camada **Gold**, foi criado um modelo semântico no Fabric com:

- Entidades organizadas (Dimensões e Fatos)  
- Relacionamentos bem definidos  
- Medidas DAX otimizadas  
- Estrutura adequada para performance em Power BI  

---

# 📊 Regra de Negócio

A solução foi desenvolvida com foco nos **países da União Europeia**, aplicando as seguintes regras:

- Extração de dados via **API X** e **CSV Y**
- Filtragem exclusiva para países da **UE**
- Cálculo de **indicadores sociais e econômicos**
- Padronização e estruturação para análises comparativas
- Criação de KPIs estratégicos para o dashboard final

---

# ⚙️ Pipeline Completo

> 🔧 **(Reserve aqui o espaço para descrever seu pipeline: Bronze → Silver → Gold → Semantic → Power BI.  
> Caso queira, posso preencher automaticamente lendo seus notebooks.)**

---

# 🛠 Tecnologias Utilizadas

- **Microsoft Fabric Lakehouse**
- **PySpark**
- **Spark SQL**
- **Notebooks Fabric**
- **Power BI**
- **Arquitetura Medallion**
- **Git / GitHub**

---

Se quiser que eu gere as **imagens** ou um **diagrama profissional** para substituir os blocos `IMAGEM_..._AQUI`, posso produzir automaticamente!  
Só pedir. 🚀
