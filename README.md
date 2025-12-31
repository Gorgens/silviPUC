# 🌲 Potencial Silvicultural

Este projeto contém uma análise de **Potencial Silvicultural** utilizando **Google Earth Engine (GEE)** e **Geemap** para processamento e visualização de dados espaciais. O objetivo é identificar áreas com aptidão para silvicultura, categorizando-as em diferentes níveis de potencial (Alto, Médio, Baixo, etc.).

## 📋 Conteúdo

O notebook principal `potencial_silvicultural.ipynb` realiza as seguintes etapas:
- Autenticação e inicialização do Google Earth Engine.
- Carregamento de dados espaciais (incluindo possíveis integrações com SiSCar ou bases locais).
- Definição de classes de uso e cobertura do solo.
- Identificação de áreas de interesse e zonas de exclusão.
- Visualização das camadas de potencial (Alto Potencial, Sem Potencial, etc.) em um mapa interativo.

## 🚀 Como Executar

### Pré-requisitos

Você precisará de uma conta no Google Earth Engine e um ambiente Python configurado. As principais bibliotecas utilizadas são:

- `earthengine-api`
- `geemap`
- `geopandas`

### Instalação

Instale as dependências necessárias (caso ainda não as tenha):

```bash
pip install geemap earthengine-api geopandas
```

### Execução

1. Abra o notebook `potencial_silvicultural.ipynb` em seu ambiente Jupyter ou VS Code.
2. Na primeira execução, será necessário autenticar sua conta do Google Earth Engine:
   ```python
   import ee
   ee.Authenticate()
   ```
3. Execute as células sequencialmente para gerar as análises e visualizar os mapas interativos.

## 📊 Visualização

O notebook gera mapas interativos onde você pode:
- Inspecionar camadas de **Alto Potencial** para silvicultura.
- Visualizar áreas de **Restrição** ou **Sem Potencial**.
- Consultar dados de pontos de interesse específicos.

## 📁 Estrutura do Projeto

- `potencial_silvicultural.ipynb`: Notebook principal com a lógica de análise.
- `shp/`: Diretório contendo arquivos shapefile de apoio (como `LASSANCE_gcs.cpg`, etc.).

---
*Gerado com base na análise do notebook `potencial_silvicultural.ipynb`.*
