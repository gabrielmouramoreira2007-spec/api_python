# api_python

API REST mínima feita com FastAPI, pronta para rodar em contêiner Docker e com testes e CI configurados. Serve como base (boilerplate) para novos serviços em Python.

## Endpoints
- GET /health — health check; retorna {"status": "ok", "version": "1.0.0"}

## Tecnologias
- FastAPI + Uvicorn
- Docker e docker-compose
- pytest (testes em test_main.py)
- GitHub Actions (CI)

## Como rodar localmente
```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

Acesse http://localhost:8000/health (documentação interativa em /docs).

## Com Docker
```bash
docker compose up --build
```

## Testes
```bash
pytest
```
