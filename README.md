# Eric Martinez — Portafolio de Data Engineer

> **Data Engineer** con experiencia práctica construyendo pipelines end-to-end, automatizando flujos de trabajo y desplegando soluciones de ML en **GCP**, **Azure** y entornos locales con **Kubernetes**. Me muevo con comodidad a lo largo de todo el ciclo de vida del dato — desde la ingesta cruda hasta el servicio de modelos.

---

## 🛠️ Habilidades principales

| Área | Tecnologías |
|---|---|
| **Plataformas Cloud** | Google Cloud Platform · Azure |
| **Orquestación** | Apache Airflow · Cloud Composer · Databricks Lakeflow |
| **Procesamiento Batch** | Apache Beam · Dataflow · Azure Data Factory · dbt |
| **Almacenamiento & Analítica** | BigQuery · Snowflake · ADLS Gen2 · Azure Blob · GCS |
| **ML / IA** | MLflow · Vertex AI (Gemini) · LangChain · KServe |
| **Infraestructura** | Kubernetes · Helm · Docker · Cloud Build (CI/CD) |
| **Lenguajes** | Python · SQL · JavaScript / TypeScript |

---

## ☁️ Google Cloud Platform

### 📚 [Recomendador de Libros — Dataform + Vertex AI](https://github.com/ericmartinezr/etl_books_ml)
Pipeline ETL de extremo a extremo que ingesta datos de libros, genera **embeddings semánticos con Vertex AI** y alimenta un recomendador visualizado en **Looker Studio**.

`Dataform` `BigQuery` `Vertex AI` `Cloud Build` `Looker Studio`

---

### 🗂️ [ETL Censo 2024 — Dataflow](https://github.com/ericmartinezr/etl_censo_gcp)
Pipeline batch escalable que procesa los datos del Censo 2024 de Chile usando **Apache Beam sobre Dataflow**. Maneja archivos Parquet de gran tamaño, está contenedorizado con Docker y se despliega via CI/CD con Cloud Build.

`Apache Beam` `Dataflow` `BigQuery` `GCS` `Docker` `Cloud Build` `Parquet`

---

### 📈 [ETL Indicadores Económicos de Chile — Cloud Composer](https://github.com/ericmartinezr/etl_indicadores_gcp)
Pipeline orquestado que extrae indicadores económicos diarios e históricos desde la API pública chilena (`mindicador.cl`), los procesa y los carga en BigQuery para su análisis en Looker Studio.

`Cloud Composer 3` `Apache Airflow` `BigQuery` `REST API` `Cloud Build`

---

## 🔵 Azure

### 🏛️ [ETL Censo 2024 — Arquitectura Medallion en Databricks](https://github.com/ericmartinezr/etl_censo_databricks)
Implementación completa de la arquitectura **Bronze → Silver → Gold** en **Azure Databricks**. Usa PySpark para transformaciones distribuidas y **Unity Catalog** para gobernanza y linaje de datos.

`Azure Databricks` `PySpark` `Unity Catalog` `ADLS Gen2` `Arquitectura Medallion`

---

### 🏭 [ETL Censo 2024 — Azure Data Factory](https://github.com/ericmartinezr/adf-censo)
Pipeline ETL visual y low-code construido con **Azure Data Factory** para procesar datos del censo de extremo a extremo, desde Azure Blob Storage hasta salidas en formato Parquet usando Data Flows.

`Azure Data Factory` `Data Flows` `Azure Blob Storage` `Parquet`

---

### 🔬 [Pipeline de Entrenamiento ML — Databricks Lakeflow](https://github.com/ericmartinezr/databricks-lakeflow)
Exploración de **Databricks Lakeflow Jobs** y **Asset Bundles (DABs)** para la automatización declarativa de flujos de ML. Entrena y rastrea un modelo de clasificación Iris con gestión completa de experimentos en **MLflow**.

`Databricks Lakeflow` `Asset Bundles (DABs)` `MLflow` `Python` `uv`

---

## 🖥️ Local / Self-Hosted

### 🕷️ [Scraper de Noticias y Licitaciones — Airflow Standalone](https://github.com/ericmartinezr/airflow-scrapper)
Pipeline de scraping automatizado orquestado con **Apache Airflow** (modo standalone en WSL2) que extrae noticias de Emol y licitaciones de MercadoPublico. Los resultados se persisten en PostgreSQL.

`Apache Airflow 3` `BeautifulSoup` `PostgreSQL` `Docker` `WSL2`

---

### ☸️ [Airflow en Kubernetes — Despliegue con Helm](https://github.com/ericmartinezr/airflow-helm)
Configuración local completa de Apache Airflow en Kubernetes usando **Helm**, incluyendo un stack de observabilidad con **Prometheus + Grafana** y un stack MLOps con **MLflow** y **KServe** para servir modelos.

`Helm` `Kubernetes` `Apache Airflow` `Prometheus` `Grafana` `MLflow` `KServe`

---

### 🛒 [Pipeline Batch de E-commerce — Apache Beam](https://github.com/ericmartinezr/ecommerce_beam)
Demuestra patrones fundamentales de ingeniería de datos usando **Apache Beam**: filtrado de datos, enmascaramiento de PII, detección de fraude y normalización de formatos sobre datos sintéticos de e-commerce, con **Side Outputs** para manejo de errores.

`Apache Beam` `Python` `Parquet` `PyArrow` `Faker`

---

## 📦 Otras Plataformas

### ❄️ [Modelado de Datos — dbt + Snowflake](https://github.com/ericmartinezr/dbt-snowflake)
Aplica las mejores prácticas de **analítica moderna** usando dbt para limpiar, enriquecer y modelar datos dentro de Snowflake. Incluye modelado dimensional con tablas de Hechos y Dimensiones.

`dbt` `Snowflake` `SQL` `Modelado Dimensional`

---

## 🤖 Proyectos IA / ML

### 💬 [Plataforma de IA para Documentos — GCP + LangChain](https://github.com/ericmartinezr/document_ai_gcp)
Aplicación GenAI full-stack que permite **conversar con documentos PDF** mediante búsqueda vectorial (pgvector) para generación aumentada por recuperación (RAG) y los modelos Gemini de Google vía Vertex AI.

- **Frontend:** Angular 21 + FastAPI (patrón BFF)
- **Backend:** FastAPI + LangChain
- **GCP:** Cloud Run · Cloud SQL (pgvector) · Vertex AI · API Gateway · Artifact Registry · Cloud Build

`FastAPI` `LangChain` `Angular` `Vertex AI (Gemini)` `Cloud Run` `pgvector` `RAG`

---

## 🔧 Utilidades & Librerías

### 🔒 [LangChain RUT Middleware](https://github.com/ericmartinezr/langchain_rut_middleware)
Un **middleware para LangChain** que detecta y redacta automáticamente RUTs chilenos de las respuestas de los modelos de lenguaje, habilitando aplicaciones de IA con protección de datos sensibles (PII) en el contexto normativo chileno.

`LangChain` `Python` `Regex` `Redacción de PII` `Privacidad de Datos`

---

*Cada proyecto incluye un README detallado con diagramas de arquitectura, instrucciones de instalación y ejemplos de uso.*
