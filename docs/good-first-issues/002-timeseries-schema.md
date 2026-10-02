# [DATA] Define a canonical time-series metadata schema

**Labels:** `good first issue`, `data`, `area:data`, `priority:starter`

## Goal

Define the minimum metadata needed to store a macroeconomic time series in a reproducible way.

## Suggested fields

```text
series_id
source
country_or_region
concept
frequency
unit
seasonal_adjustment
currency_basis
price_basis
observation_start
observation_end
release_timestamp
vintage_timestamp
transformation
source_url
license
notes
```

## Acceptance criteria

- Add the schema to `DATA.md`.
- Explain required vs optional fields.
- Include at least two worked examples.
- Explicitly distinguish observation date from release/vintage date.
