# Loja Veloz – Plataforma de Pedidos

## Arquitetura

Plataforma de microserviços composta por:
- **api-gateway** - Gateway de entrada (porta 8080)
- **pedidos** - Serviço de pedidos
- **pagamentos** - Serviço de pagamentos
- **estoque** - Serviço de estoque
- **postgres** - Banco de dados PostgreSQL

## Execução Local

Pré-requisitos: Docker e Docker Compose

```bash
docker compose up -d
```

## Endpoints

- Health check: http://localhost:8080/health
- Métricas Prometheus: http://localhost:8080/metrics

## Tecnologias

- Python 3.11 + Flask
- PostgreSQL 15
- Docker & Kubernetes
- Terraform
- Prometheus (observabilidade)
