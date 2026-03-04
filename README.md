# 🚀 Local Server Monitoring Stack (Docker + Prometheus + Grafana)

## 📌 Overview

This project implements a containerized monitoring stack using Docker Compose to simulate a lightweight data centre monitoring environment.

The stack monitors:
- Host system metrics (CPU, Memory, Disk)
- Containerized services (Nginx)
- Real-time performance data visualized via Grafana dashboards

This project demonstrates foundational DevOps, infrastructure automation, and observability skills aligned with enterprise data centre operations.

---

## 🏗 Architecture


Docker Compose
├── Prometheus (Metrics Collection)
├── Grafana (Metrics Visualization)
├── Node Exporter (Host Metrics)
└── Nginx (Sample Application Service)


### Components

- **Prometheus** – Scrapes and stores time-series metrics  
- **Grafana** – Visualizes metrics through dashboards  
- **Node Exporter** – Exposes system-level metrics  
- **Nginx** – Sample containerized service being monitored  

---

## 🛠 Technologies Used

- Docker
- Docker Compose
- Prometheus
- Grafana
- Node Exporter
- Nginx
- YAML configuration
- Linux CLI

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/monitoring-stack.git
cd monitoring-stack
2️⃣ Start Services
docker compose up -d
3️⃣ Verify Running Containers
docker ps

Expected services:

prometheus

grafana

node-exporter

nginx

```
🌐 Access Services
Service	URL
Prometheus	http://localhost:9090

Grafana	http://localhost:3000

Nginx	http://localhost:8080
Grafana Default Login
Username: admin
Password: admin
📊 Monitoring Capabilities
Host Metrics (via Node Exporter)

- CPU usage

- Memory usage

- Disk utilization

- Network activity

- Container Metrics

- Nginx service health

```bash
HTTP traffic monitoring

📁 Project Structure
monitoring-stack/
├── docker-compose.yml
├── prometheus/
│   └── prometheus.yml
└── grafana/
    └── provisioning/
        └── datasources/
            └── datasource.yml
```

🔍 : Key Learning Outcomes

- Container orchestration using Docker Compose

- Prometheus scrape configuration

- Infrastructure monitoring concepts

- Metrics visualization using Grafana dashboards

- Troubleshooting Docker networking & DNS issues

- Writing production-style documentation

🚧 Challenges Faced

- Encountered Docker image resolution failure due to DNS misconfiguration

- Diagnosed network connectivity issue

- Reconfigured system DNS

- Successfully restored Docker registry access

This reflects real-world infrastructure troubleshooting experience.

📌 Future Improvements

- Add alerting rules (Prometheus Alertmanager)

- Integrate ELK Stack for log monitoring

- Deploy on remote VPS for production simulation

- Add CI pipeline for automated deployment

👨‍💻 Author

Emmanuel Kipngeno
Full-Stack Developer | DevOps Enthusiast

GitHub: https://github.com/kkmanuu
