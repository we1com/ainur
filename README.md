# Cloud Infrastructure Project (Project 02)

## 1. Жобаны жоспарлау
* **Құралдар:** JIRA
* **Әдістеме:** Kanban

## 2. Технологиялық стек
* **Frontend:** React
* **Backend:** Python (Flask)
* **Cloud:** AWS (EC2, S3)
* **Monitoring:** Prometheus & Grafana

## 3. Архитектуралық диаграмма
```mermaid
graph LR
    User((Пайдаланушы)) --> CloudFront[AWS CloudFront]
    CloudFront --> S3[S3 Bucket: Static Files]
    CloudFront --> EC2[EC2 Instance: Flask App]
    EC2 --> DB[(PostgreSQL)]
    EC2 -.-> Mon[Monitoring: Prometheus]# ainur
