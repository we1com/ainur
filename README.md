# Қауіпсіз желілік инфрақұрылым жобасы 2025

## 1. Жобаны басқару (Management)
* **Әдістеме:** Extreme Programming (XP)
* **Бақылау құралы:** GitHub Projects тақтасы
* **Орындалу деңгейі:** 100% аяқталды

## 2. Технологиялық құрам
* **Backend:** Ruby on Rails
* **Деректер қоры:** Redis & MariaDB
* **Инфрақұрылым:** DigitalOcean Droplets
* **Қауіпсіздік:** SSL/TLS & Cloudflare WAF
* **Контейнерлеу:** Docker Compose

## 3. Желілік архитектура схемасы
```mermaid
graph TD
    User((Пайдаланушы)) --> WAF[Cloudflare Firewall]
    WAF --> LB[Load Balancer]
    LB --> App1[Ruby Server 1]
    LB --> App2[Ruby Server 2]
    App1 & App2 --> Cache[(Redis Cache)]
    App1 & App2 --> DB[(MariaDB Cluster)]
    
    subgraph "Security Layer"
        WAF
        LB
    end
