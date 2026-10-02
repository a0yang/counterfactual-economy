# [DATA] Add a sample public time-series adapter interface

**Labels:** `good first issue`, `data`, `python`, `area:data`, `priority:starter`

## Goal

Create a small Python interface showing how a public macroeconomic data source can be adapted into the project's canonical time-series representation.

This does not need to download real data yet. A clean interface and mocked example are enough for the first PR.

## Suggested scope

- Define a `SeriesMetadata` structure.
- Define a `SeriesObservation` structure.
- Define an adapter interface with `fetch_series()`.
- Add a mocked example.

## Acceptance criteria

- No API key is committed.
- The interface preserves source, license, release/vintage metadata, and units.
- Example output is documented.
- The design can later support multiple sources, not only FRED.
