# src

> Deployable / production-grade code lives here. Separated from the reference scripts in `80_Code/scripts/`.

## Structure

```
src/
├── validation/     # Event schema validators, QA checks
├── pipelines/      # BigQuery ETL / reporting pipelines
├── utils/          # Shared utilities, helpers, config loaders
└── __init__.py
```

> [!NOTE]
> This directory will be populated once the team's deployment patterns, CI/CD, and linting standards are understood. Until then, use `80_Code/scripts/` for exploratory and utility scripts.
