# Claude Instructions

## Repository structure

This repo has a `main` branch and 6 exercise branches, each a solution snapshot of one exercise: `01-setup-infra-metrics`, `02-setup-obi`, `03-instrumenting-applications`, `04-customizing-instrumentations`, `05-processing` and `06-manual-instrumentation`. Each exercise branch is stacked on top of the previous one (i.e., `02-setup-obi` is based on `01-setup-infra-metrics`, etc.).

The exercise branches carry the history of the original `grafana-cold-storage/grafanacon2026-opentelemetry-instrumentation` repository plus a commit that points links at this repo. Don't squash or force-push them without asking the user first.

Links in the docs must point to this repo (`immavalls/opentelemetry-instrumentation-workshop`) or be relative, never to `grafana/grafanacon2026-opentelemetry-instrumentation`.

## Validating changes

Always run tests after making changes to go or js files:

```bash
make test
```

This runs both backend and frontend tests.

After making any changes, run formatting and spell check:

```bash
make format
make spell
```
