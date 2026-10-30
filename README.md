# Analytics Econômico

Portfólio de análise de dados em Flask: estudos sobre a economia brasileira e mundial
com dados coletados de APIs oficiais (Banco Central, FMI, IBGE…).

## Como rodar

```bash
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
cp .env.example .env
.venv/bin/flask --app run run --debug --port 5050
```

Acesse http://localhost:5050. Testes: `.venv/bin/pytest`.

## Estrutura

- `app/` — Flask (`routes/paginas.py` páginas, `routes/api.py` JSON dos gráficos, `dados.py` preparação dos dados)
- `app/static/css/global.css` — estilos globais e tokens do tema dark
- `app/static/fonts/`, `app/static/img/` — fontes e imagens
- `coletores/` — um módulo por fonte de dados, com cache em `data/cache/`
- `docs/` — planejamento e catálogo de fontes (`data/fontes.yaml`)
# BRLTrendAnalytics
