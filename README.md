# 📊 Real-Time YouTube Analytics Pipeline (Data Engineering Zoomcamp 2025 Project)
 [Data Engineering Zoomcamp 2025](https://www.youtube.com/watch?v=X8cEEwi8DTM&list=PL3MmuxUbc_hJZdpLpRHp7dg6EOx828q6y)

This project is built as part of the **Data Engineering Zoomcamp 2025**. It implements an end-to-end real-time data pipeline that monitors YouTube activity (views, likes, comments) on a selected video list and streams it through Kafka for processing and analysis.

> ⚠️ **Note**: Telegram bot integration is currently not functional and will be addressed in future work.

---

## 🚀 Project Overview

This pipeline fetches video analytics from the YouTube API, streams it into Kafka topics, processes it with ksqlDB, and enables extensible integrations with external systems. The goal is to demonstrate real-time analytics capability using industry-grade tools and infrastructure.

---

## 🛠 Technologies & Tools Used

| Tool/Tech | Purpose |
|-----------|---------|
| **Python** | Fetch data from YouTube API and push to Kafka |
| **YouTube Data API v3** | Access video statistics and metadata |
| **Docker + Docker Compose** | Containerize the full Kafka ecosystem |
| **Apache Kafka** | Real-time messaging and data streaming |
| **Kafka Connect** | External system integration (e.g., Telegram, future DB) |
| **ksqlDB** | Real-time stream processing using SQL-like syntax |
| **Google Cloud Platform** | Set up API keys and manage quotas for YouTube API |
| **Confluent Platform** | Kafka management, Control Center, Connectors |

---

## 📌 Features

- ✅ Real-time ingestion of YouTube video stats using Python
- ✅ Kafka ecosystem setup via Docker Compose (Zookeeper, Kafka, Schema Registry, ksqlDB, Control Center)
- ✅ Stream processing using ksqlDB (custom queries and filtering)
- ✅ Modular and extensible design to connect with external systems

---

## 📈 Use Case

I applied this pipeline to **analyze the video list from the [Data Engineering Zoomcamp 2025]**, enabling near real-time insights into audience interaction.

---

## 📂 Folder Structure
```bash
├── docker-compose.yml        # Setup Kafka ecosystem
├── YoutubeAnalytics.py       # Fetch YouTube video data
├── config/                   # API keys and secrets
└── README.md                 # Project documentation
```

## 🔮 Future Work
❌ Telegram Integration: Although initial steps were implemented (Telegram Bot setup), real-time alerts for significant YouTube events are not functional yet due to integration issues. This remains a priority for future development.

🔌 Integration with databases such as PostgreSQL or BigQuery

📊 Visualization dashboards using tools like Grafana or Looker Studio
