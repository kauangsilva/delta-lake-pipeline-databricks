# 🚀 Pipeline ELT com Delta Lake no Databricks

Projeto profissional de engenharia de dados implementando um pipeline ELT completo utilizando Delta Lake no Databricks com Arquitetura Medallion.

## 🎥 Vídeo Demonstrativo  
Para ver todo o processo do projeto em ação, assista ao vídeo explicativo:  
👉 [Clique aqui para assistir ao vídeo no youtube](https://www.youtube.com/watch?v=Ryu0ri_XC_M) 

## 📊 Dashboard Analítico no Power BI  
Os dados processados neste pipeline foram utilizados para criar um **dashboard interativo de vendas no Power BI**, com foco em **análises de faturamento, ticket médio, canais de venda e desempenho por vendedor**.  
👉 [Acesse o Dashboard Power BI aqui](https://github.com/kauangsilva/delta-lake-powerbi-dashboard)  

O dashboard foi desenvolvido a partir dos **dados da camada Gold (Business)** deste projeto, exportados em formato **Parquet particionado**, garantindo alta performance nas consultas e visualizações.

---


## 🏗️ Arquitetura Medallion

### 🥉 Camada BRONZE (Raw)
- **Dados brutos** ingeridos das fontes originais
- Formato Delta Lake com versionamento nativo
- Preserva dados exatamente como foram extraídos

### 🥈 Camada Silver (Cleaned)  
- **Dados tratados** e enriquecidos
- Qualidade aplicada: remoção de duplicatas, tratamento de nulos
- Junção de tabelas e enriquecimento dimensional

### 🥇 Camada Gold (Business)
- **Dados prontos para análise**
- Agregações e métricas de negócio
- Formato Parquet otimizado para consultas
- Particionamento para performance


### 📊 Descrição dos Arquivos:

- **`data/raw/`**: Dados brutos com problemas reais de qualidade
- **`notebooks/`**: Código modular e executável passo a passo  
- **`README.md`**: Guia completo de implementação

## 📁 Estrutura do Projeto
sales_project/
* 01_ingestao_dados.py          # Extração e carga (Bronze)
* 02_transformacao_delta.py     # Transformação (Silver → Gold)  
* 03_manutencao_otimizacao.py   # Otimização e manutenção


## 🔧 Tecnologias Utilizadas

- **Databricks** - Plataforma de execução
- **Delta Lake** - Armazenamento e governança de dados
- **PySpark** - Processamento distribuído
- **Python** - Linguagem de programação
- **SQL** - Consultas e transformações

## ⚡ Funcionalidades Implementadas

### 🔄 Pipeline ELT Completo
- Extração de dados de múltiplas fontes
- Carga incremental com Delta Lake
- Transformações com PySpark e SQL

### 🛠️ Transformações de Dados
- **Limpeza**: tratamento de nulos e duplicatas
- **Enriquecimento**: joins entre tabelas
- **Agregação**: métricas de negócio
- **Desnormalização**: dados prontos para análise

### ⚡ Otimizações (Conceituais)
*Demonstração de conceitos enterprise aplicáveis em ambientes production:*
- **VACUUM**: Limpeza de versões antigas
- **OPTIMIZE**: Compactação de arquivos
- **Z-ORDER**: Clusterização para performance
- **CACHE**: Armazenamento em memória

## 🚀 Como Executar

### Ordem de Execução
1. **Notebook 1**: `01_ingestao_dados.py` (Ingestão)
2. **Notebook 2**: `02_transformacao_delta.py` (Transformação)
3. **Notebook 3**: `03_manutencao_otimizacao.py` (Otimizações conceituais)

## 📈 Resultados

### Dados de Saída
- **Bronze**: Dados brutos com versionamento
- **Silver**: Dados tratados e enriquecidos
- **Gold**: Dados agregados para análise

### Métricas Business
- Performance por vendedor
- Vendas por região e categoria
- Ticket médio e volume de vendas

## 💡 Diferenciais

- **Arquitetura Medallion** aplicada na prática
- **Delta Lake** com time travel e versionamento
- **Otimizações** profissionais demonstradas
- **Código production-ready** e modular

---

## 📬 Contato

- [LinkedIn](https://www.linkedin.com/in/kauansilva96/)
- [Biolink](https://biolink.website/socialKauanSilva)
- Email: kauangsilva1996@gmail.com
