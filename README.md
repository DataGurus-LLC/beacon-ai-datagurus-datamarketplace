# Beacon AI - DataGurus NextGeneration Datamarket Place

**Repo:** `beacon-ai-datagurus-datamarketplace`

A community-driven, next-generation data marketplace maintained by DataGurus LLC.

## Highlights
- Guardrailed contribution flow (Conventional Commits, protected branches, signed commits)
- Strong CI: tests, type checks, license & secret scans, data QA gates
- Data contracts + reproducible releases (`/data/releases/<dataset>/<version>`)

## Getting Started
1. Fork or clone the repo.
2. Install dev tools:
   ```bash
   python -m venv .venv && source .venv/bin/activate
   pip install -r requirements-dev.txt
   pre-commit install
   ```
3. Run CI locally:
   ```bash
   make ci
   ```

## Branching
- Short-lived feature branches: `feat/<scope>`, `fix/<scope>`, `data/<dataset>`
- Squash merge via PR; no direct pushes to `main`

## Data Contracts
See [`data/README.md`](data/README.md) and example under `data/contracts/example_dataset.yaml`.

## Governance
See [`docs/GOVERNANCE.md`](docs/GOVERNANCE.md) and RFC process in `docs/rfcs/`.
