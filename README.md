# Enterprise Mobile & Cloud Solution 2025

## 1. Project Management
* **Framework:** Lean Software Development
* **Management Tool:** GitHub Projects (Kanban Board)
* **Status:** In Production

## 2. Technology Infrastructure
* **Mobile Frontend:** React Native
* **Backend Services:** Java (Spring Boot)
* **Database:** Redis & MySQL
* **Cloud Platform:** Google Cloud Platform (GCP)
* **Deployment:** Helm & Kubernetes

## 3. System Architecture Diagram
```mermaid
graph LR
    App((Mobile App)) --> API[Cloud Endpoints]
    API --> Logic[Spring Boot Microservices]
    Logic --> Cache[(Redis Cache)]
    Logic --> DB[(MySQL Cluster)]
    
    subgraph "DevOps Pipeline"
        Git[GitHub] --> Action[GitHub Actions]
        Action --> GCR[Google Container Registry]
        GCR --> GKE[Google Kubernetes Engine]
    end
