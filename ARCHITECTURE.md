# Architecture

This document describes a candidate architecture. It is a design starting point, not a fixed implementation mandate.

## 1. Data layer

Responsibilities:

- ingest public data through adapters;
- normalize country, unit, frequency and time conventions;
- preserve source metadata;
- preserve historical vintages where available;
- distinguish observations known at a given simulation date from later revisions;
- record transformations and assumptions.

Suggested storage formats:

- Parquet for analytical data;
- DuckDB for local research queries;
- SQLite for portable scenarios and small installations.

## 2. Economic state

The state should expose explicit balance sheets and flows.

Example entities:

- Household sector
- Corporate sector
- Banking sector
- Government sector
- Central bank
- Rest of world

A Stock-Flow Consistent accounting layer can provide hard consistency constraints.

## 3. Agents

Agents need not be one-to-one representations of real people. Representative or weighted heterogeneous agents are acceptable where computationally necessary.

An agent may contain:

- assets;
- liabilities;
- income;
- expected income;
- risk preference;
- borrowing constraint;
- investment/consumption rules;
- policy exposure;
- information set.

## 4. Production and input-output layer

This layer represents sectors and intermediate demand. It should be possible to add sectors without rewriting the core.

## 5. Financial network

Represent exposures and funding relationships between institutions.

Candidate mechanisms:

- bank capital;
- leverage;
- collateral;
- maturity mismatch;
- short-term wholesale funding;
- asset valuation;
- margin calls;
- fire sales;
- liquidity freezes;
- default propagation.

## 6. Policy engine

Policies are mechanisms, not bonuses.

Each policy should define:

- target;
- timing;
- implementation rule;
- affected agents;
- direct accounting effect;
- behavioral effect;
- constraints;
- possible side effects.

## 7. Expectations

The engine should support multiple expectation mechanisms, potentially including:

- adaptive expectations;
- moving averages;
- bounded rationality;
- rational expectations as a research option;
- heterogeneous expectations.

## 8. Calibration

Calibration should be explicit and versioned.

Possible techniques:

- historical matching;
- optimization;
- Bayesian calibration;
- simulated method of moments;
- indirect inference;
- sensitivity analysis.

## 9. Validation

Validation is separate from calibration.

The project should prioritize out-of-sample tests and avoid using future observations to tune a model that is then evaluated on the same period.

## 10. Counterfactual engine

The engine should support:

- baseline scenario;
- one-variable intervention;
- multi-policy intervention;
- scenario tree;
- Monte Carlo runs;
- parameter sweeps;
- policy search / optimization experiments.

## 11. Presentation layer

### Game UI

- 2D country/map view;
- dashboards;
- timelines;
- policy controls;
- economic event notifications;
- sector maps;
- financial network visualization.

### Research UI

- time series;
- uncertainty bands;
- scenario comparison;
- parameter sensitivity;
- network graphs;
- divergence from historical reality;
- reproducible experiment metadata.

## 12. Mod system

Long-term target:

```text
mods/
  my-policy/
    manifest.toml
    parameters.toml
    rules/
    data/
    localization/
```

A mod should be able to introduce a new country, policy, sector, financial rule, crisis mechanism or visualization without changing the simulation kernel.
