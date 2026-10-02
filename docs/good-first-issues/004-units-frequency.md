# [DATA] Add units and frequency normalization rules

**Labels:** `good first issue`, `data`, `area:data`, `priority:starter`

## Goal

Document and prototype rules for normalizing common economic units and frequencies.

## Examples to cover

- percent vs percentage points;
- USD vs local currency;
- nominal vs real values;
- monthly vs quarterly frequency;
- annualized rates vs period rates;
- index levels vs percentage changes.

## Acceptance criteria

- Add a short normalization specification to `DATA.md`.
- Provide at least five examples of ambiguous transformations.
- State which transformations must never be performed automatically without an explicit rule.
