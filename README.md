# 🎧 Spotify End-To-End Data Engineering Project

This project demonstrates a complete **ETL (Extract, Transform, Load)** pipeline using the **Spotify Web API** and various **AWS services**. It was designed to simulate a real-world, scalable data engineering workflow—from data ingestion to querying insights with Amazon Athena.

---

## 🚀 Project Overview

- Extract real-time music metadata from Spotify's public API  
- Store raw data in Amazon S3 using AWS Lambda  
- Transform and clean the data using serverless functions  
- Catalog structured data using AWS Glue  
- Query and analyze insights using Amazon Athena

---

## 🧠 Why This Project?

This project was created to:
- Practice building **automated data pipelines**
- Work hands-on with **cloud-based tools** like AWS Lambda, S3, Glue, and Athena
- Develop an understanding of real-time **API integration and orchestration**
- Showcase practical **data engineering and cloud skills** in a portfolio-ready format

---

## 🛠️ Tools & Technologies Used

| Tool               | Purpose                                |
|--------------------|----------------------------------------|
| **Python**         | Data extraction, transformation logic  |
| **Spotify API**    | Source of music/artist metadata        |
| **AWS S3**         | Raw data storage (object store)        |
| **AWS Lambda**     | Serverless ETL orchestration           |
| **AWS Glue Crawler**| Schema inference for S3 data         |
| **Glue Data Catalog** | Metadata repository                |
| **Amazon Athena**  | SQL-based querying on S3               |
| **CloudWatch**     | Monitoring & Lambda logs               |

---

## 📊 Project Architecture

![Architecture Diagram](https://github.com/Sai-teja-gajula/spotify-data-pipeline-project/blob/main/Project%20Architecture%20Diagram.png)

---

## 📦 Installation

Install required Python packages:
```bash
pip install pandas
pip install numpy
pip install spotipy


## 📦 Installation

Install required Python packages:
```bash
pip install pandas
pip install numpy
pip install spotipy

Spotify API (Track/Artist/Album Metadata)
        ⬇
AWS Lambda (Trigger every hour via CloudWatch)
        ⬇
Raw Data stored in Amazon S3
        ⬇
Transform Function triggered via Lambda
        ⬇
Cleaned Data stored in S3 (processed zone)
        ⬇
AWS Glue Crawler detects schema
        ⬇
Glue Data Catalog created/updated
        ⬇
Amazon Athena used to query and analyze data

Spotify-Data-Pipeline-Project/
│
├── spotify_api_data_extract.py              # Data extraction from Spotify API
├── spotify_transformation_load_function.py  # Data cleaning and loading
├── Spotify Data Pipeline (ETL).ipynb        # ETL walkthrough in notebook format
├── Project Architecture Diagram.png         # Architecture visualization
├── ETL Process.png                          # ETL visual overview
└── README.md
