<!-- ================= HEADER (animated 3D SVG, see assets/banner.svg) ================= -->
<p align="center">
  <img src="./assets/banner.svg" alt="Samuel Acosta · Data Engineer" width="100%" />
</p>

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1000&color=38BDF8&center=true&vCenter=true&width=620&lines=Turning+raw+data+into+reliable+insights;Bronze+%E2%86%92+Silver+%E2%86%92+Gold+pipelines+on+AWS;PySpark+%7C+AWS+Glue+%7C+S3+%7C+SQL+%7C+Python;Open+source+contributor+in+the+data+ecosystem" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Focus-Data%20Engineering-0ea5e9?style=for-the-badge&logo=databricks&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloud-AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
  <img src="https://img.shields.io/badge/Based%20in-Medell%C3%ADn%2C%20CO-16a34a?style=for-the-badge&logo=googlemaps&logoColor=white" />
  <img src="https://komarev.com/ghpvc/?username=sacostaa1&style=for-the-badge&color=0ea5e9&label=Profile+views" />
</p>

---

## 👋 About me

I'm **Samuel**, a **Systems Engineer from EAFIT University** focused on **Data Engineering**.
I design and build data pipelines that take messy, raw data and turn it into clean, trusted datasets ready for analytics and machine learning.

```python
class DataEngineer:
    name     = "Samuel Acosta"
    location = "Medellín, Colombia 🇨🇴"
    focus    = ["Batch pipelines", "Medallion architecture", "Data quality", "Cloud data platforms"]
    stack    = {
        "processing": ["PySpark", "Pandas", "SQL"],
        "cloud":      ["AWS Glue", "S3", "Lambda", "RDS"],
        "platforms":  ["Databricks", "GCP Dataproc"],
        "serving":    ["Streamlit", "FastAPI", "Plotly"],
    }
    mindset  = "If it isn't tested, monitored and documented, it isn't production-ready."
```

- 🏗️ Building **Bronze → Silver → Gold** pipelines with **AWS Glue + PySpark** on **S3**
- 🧪 Obsessed with **data quality**: nulls, duplicates, outliers and schema drift are measured, not guessed
- ⚡ Background in **serverless backends** (FastAPI + AWS Lambda + RDS), so I care about latency and cost
- 🌱 Contributing to **open source data tools**, and always happy to collaborate

---

## 🔄 How I build pipelines

```mermaid
flowchart LR
    A[(Raw sources<br/>APIs · CSV · Open Data)] -->|ingest| B[🥉 Bronze<br/>raw on S3]
    B -->|clean · dedupe · cast types| C[🥈 Silver<br/>validated Parquet]
    C -->|enrich · aggregate · features| D[🥇 Gold<br/>analytics-ready]
    D --> E[📊 Dashboards]
    D --> F[🤖 ML models]
    B -.->|health checks| Q{{Data quality<br/>metrics}}
    C -.->|health checks| Q
```

---

## 🚀 Featured data projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🗽 NYC 311 · Medallion Data Pipeline</h3>
      <p>End-to-end pipeline over the NYC 311 service-request dataset. <b>AWS Glue (PySpark)</b> jobs move data from <b>Bronze → Silver → Gold</b> on <b>S3</b>, with health-check jobs that track nulls, duplicates and outliers per layer, plus feature enrichment for an ML model and a live quality dashboard.</p>
      <p>
        <img src="https://img.shields.io/badge/AWS%20Glue-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" />
        <img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
        <img src="https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white" />
        <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" />
      </p>
      <a href="https://github.com/SaraCmque/ny311_ds_project">📁 Code</a> · <a href="https://ny311dsproject.streamlit.app/">🌐 Live dashboard</a>
    </td>
    <td width="50%" valign="top">
      <h3>🏭 Decision Support System · Data Integration</h3>
      <p>Integrates three deliberately inconsistent sources (<b>inventory, logistics and customer feedback</b>) into a single model. Cleans type errors, outlier costs ($0.01 → $850k) and negative stock, then answers 5 business questions, including quantifying <b>17.44% of revenue at risk</b> from untracked inventory.</p>
      <p>
        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
        <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
        <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat-square&logo=plotly&logoColor=white" />
      </p>
      <a href="https://github.com/sacostaa1/challenge02-data-science">📁 Code</a> · <a href="https://challenge02-data-science-tikjhs9mnzqrgvwb4amsno.streamlit.app">🌐 Live app</a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>📡 IoT & Infrastructure Analytics Audit</h3>
      <p>Audit of agricultural and energy sensor data in Eastern Antioquia: denoising IoT signals (FFT, Butterworth filters), graph analysis to find single points of failure, and time-series forecasting (ADF, Granger, SARIMAX).</p>
      <p>
        <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white" />
        <img src="https://img.shields.io/badge/NetworkX-2C3E50?style=flat-square" />
        <img src="https://img.shields.io/badge/Statsmodels-4B8BBE?style=flat-square" />
      </p>
      <a href="https://github.com/SaraCmque/DS-Challenge3">📁 Code</a>
    </td>
    <td width="50%" valign="top">
      <h3>☁️ Data Storage & Processing Labs</h3>
      <p>Hands-on labs across platforms: <b>S3</b> data lakes, <b>SQL</b>, <b>Spark medallion</b> pipelines, a <b>Glue Bronze → Silver</b> job, <b>Databricks ETL</b> and <b>GCP Dataproc</b>.</p>
      <p>
        <img src="https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white" />
        <img src="https://img.shields.io/badge/Dataproc-4285F4?style=flat-square&logo=googlecloud&logoColor=white" />
        <img src="https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white" />
      </p>
      <a href="https://github.com/sacostaa1/almacenamiento_procesamiento_03_2026">📁 Code</a>
    </td>
  </tr>
</table>

---

## 🧰 Data stack

<p align="center"><b>Languages & processing</b></p>
<p align="center">
  <img src="https://skillicons.dev/icons?i=py,r,postgres,mysql,mongodb,sqlite&perline=8" />
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
</p>

<p align="center"><b>Cloud & data platforms</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/AWS%20Glue-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white" />
  <img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white" />
  <img src="https://img.shields.io/badge/AWS%20Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white" />
  <img src="https://img.shields.io/badge/Amazon%20RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white" />
  <img src="https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white" />
  <img src="https://img.shields.io/badge/Google%20Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" />
</p>

<p align="center"><b>Serving, visualization & tooling</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" />
</p>

<p align="center"><b>🎯 Next on my roadmap</b></p>
<p align="center">
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white" />
  <img src="https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/Delta%20Lake-00ADD4?style=for-the-badge&logo=delta&logoColor=white" />
</p>

---

## 📊 My contributions in 3D

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-3d-contrib/profile-night-rainbow.svg" />
    <source media="(prefers-color-scheme: light)" srcset="./profile-3d-contrib/profile-gitblock.svg" />
    <img src="./profile-3d-contrib/profile-night-rainbow.svg" alt="3D contribution graph" width="100%" />
  </picture>
</p>

---

## 🤝 Let's build together

I'm actively looking to **collaborate on open source data projects** (pipelines, data quality, Spark, AWS tooling) and to connect with people in the data community.
Open an issue on any of my repos, or reach out:

<p align="center">
  <a href="mailto:samuelacostaaristizabal1@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/sacostaa1"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<p align="center">
  🌎 Spanish (native) · English · Portuguese (learning)
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=110&section=footer" alt="footer" />
</p>
