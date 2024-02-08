# Grafana Prometheus and Alertmanager Setup with Docker Compose

This repository contains a Docker Compose setup for a monitoring stack with Grafana, Prometheus, Alertmanager, and multiple agents with node_exporter.

## Prerequisites

Make sure you have Docker and Docker Compose installed on your machine.

- [Docker Installation](https://docs.docker.com/get-docker/)
- [Docker Compose Installation](https://docs.docker.com/compose/install/)

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-monitoring-repo.git
cd your-monitoring-repo
```
### 2. Set Up Docker Compose
# Start the monitoring stack
```bash
docker-compose -f docker-compose.yml up -d
```

# Start the agents
```bash
docker-compose -f agent-compose.yml up -d
```

### Access Services

- **Grafana:** [http://localhost:3000](http://localhost:3000) 
  - Default credentials: admin/admin

- **Prometheus:** [http://localhost:9090](http://localhost:9090)

- **Alertmanager:** [http://localhost:9093](http://localhost:9093)



### 4. Stop the Services
```bash
docker-compose -f docker-compose.yml down
docker-compose -f agent-compose.yml down
```
## Configuration
- **prometheus.yml:** Defines agents ip/hostname Ex. agent1:9100.
- **alertmanager.yml:** Defines your SMTP credentials for Email alert.

- **docker-compose.yml:** Defines services for Grafana, Prometheus, and Alertmanager along with volume configurations.

- **agent-compose.yml:** Defines services for multiple agents with node_exporter.

## Volumes(bind mount)

- **grafana:** Grafana data directory.

- **prometheus:** Prometheus data directory.

- **alertmanager:** Alertmanager data directory.
