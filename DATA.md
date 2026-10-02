# Data policy and data architecture

## Principle

The project should separate **code**, **model parameters**, **source data**, and **derived datasets**.

Do not assume that a dataset being publicly downloadable means that it can be redistributed inside a commercial game.

## Required metadata

Each dataset or series should record, where available:

- source;
- publisher;
- dataset name;
- series identifier;
- country / region;
- frequency;
- unit;
- seasonal-adjustment status;
- observation date;
- release date;
- vintage / realtime period;
- retrieval date;
- original license;
- transformation applied;
- notes on breaks in methodology.

## Historical data vintages

Historical simulation has two different concepts:

### Observation time

When the economic quantity refers to.

### Information time

When a decision-maker could have known the value.

For example, an experiment labeled “decision in 2005” should, where possible, use the information set available in 2005 rather than today's revised estimate.

## Data adapters

The codebase should prefer adapters over hard-coding a single provider.

Candidate providers include public statistical institutions such as:

- FRED / ALFRED;
- IMF;
- OECD;
- BIS;
- ECB;
- national statistical offices.

Provider access, licensing and API terms must be checked before redistribution or commercial use.

## Derived data

Transformations such as inflation adjustment, log transforms, ratios, rolling averages and risk indicators should be reproducible from source data and documented in code or metadata.

## Data quality

A data contribution should identify:

1. what the data represents;
2. why it is needed;
3. its source and license;
4. known limitations;
5. any required preprocessing.

## No hidden hindsight

A research experiment should declare whether it uses:

- realtime/vintage information;
- final revised historical data;
- perfect historical knowledge;
- analyst assumptions.

Those are different experimental modes and should never be silently mixed.
