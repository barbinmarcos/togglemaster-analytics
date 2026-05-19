# ToggleMaster Analytics Service

Microsserviço responsável pela coleta e análise de métricas da plataforma.

## Responsabilidades

- Coleta de eventos
- Métricas de uso
- Auditoria
- Processamento analítico

## Stack

- Golang
- Docker
- Kubernetes
- GitHub Actions
- Amazon ECR
- Amazon EKS

## Execução local

```bash
go run cmd/main.go
Endpoint de Health Check
GET /health
Docker

Build:

docker build -t togglemaster-analytics .

Run:

docker run -p 8084:8084 togglemaster-analytics
CI/CD

Pipeline DevSecOps com:

Build
Unit Tests
GolangCI-Lint
Gosec
Trivy
Docker Build
Push para Amazon ECR
Deploy

Deploy automatizado via GitOps utilizando ArgoCD.



