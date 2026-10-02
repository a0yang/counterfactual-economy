# [INFRA] Create a minimal experiment configuration loader

**Labels:** `good first issue`, `python`, `area:infra`, `priority:starter`

## Goal

Define how a simulation experiment declares its period, country, model modules, data sources, parameters, seed, and output location.

Use the existing `examples/experiment.yaml` as the starting point.

## Acceptance criteria

- Load the YAML configuration into a typed Python object or equivalent structure.
- Validate required fields.
- Reject unknown or malformed values with useful messages.
- Add one test fixture for a valid experiment and one invalid fixture.
