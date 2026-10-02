# [RESEARCH] Add reproducibility metadata for experiments

**Labels:** `good first issue`, `research`, `area:research`, `priority:starter`

## Goal

Create a small machine-readable record that captures the state needed to reproduce a simulation.

## Include

- experiment ID;
- model version / commit;
- dataset identifiers;
- dataset vintage or retrieval date;
- parameter set;
- assumptions profile;
- random seed;
- execution timestamp;
- software environment summary.

## Acceptance criteria

- Document the record format.
- Add a sample file under `examples/`.
- Explain which fields should be immutable after an experiment is published.
