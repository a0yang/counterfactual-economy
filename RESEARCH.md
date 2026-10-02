# Research Questions

This file is the open research agenda. Questions are expected to change as contributors test the system.

## RQ-001 — Accounting consistency

Can a lightweight Stock-Flow Consistent core reproduce basic national-accounting identities while remaining suitable for high-frequency simulation?

## RQ-002 — Heterogeneous agents

What level of household and firm heterogeneity is necessary to reproduce important macro-financial outcomes without making the simulation computationally impractical?

## RQ-003 — Expectations

How much do alternative expectation mechanisms change counterfactual results?

## RQ-004 — Housing and credit

Can household leverage, housing prices and mortgage-credit mechanisms reproduce major features of the pre-2008 U.S. financial expansion?

## RQ-005 — Financial contagion

How should balance-sheet exposures and liquidity mechanisms be represented so that systemic stress can propagate without becoming arbitrary?

## RQ-006 — Crisis early warning

Can a model using only information available before an event identify rising systemic vulnerability out of sample?

## RQ-007 — Policy counterfactuals

Do plausible changes in policy parameters produce robustly different outcome distributions across model specifications?

## RQ-008 — Calibration versus overfitting

How can the project calibrate historical parameters without tuning the model so heavily that it only reproduces one known episode?

## RQ-009 — Structural breaks

How should the simulation respond when institutions, technology, regulation or financial practices change fundamentally?

## RQ-010 — Model disagreement

Can the platform present disagreement between economic models as useful information rather than hiding it behind an averaged forecast?

## RQ-011 — Real-time scenario analysis

How should current economic data be incorporated so that future scenarios remain explicit about assumptions and do not masquerade as certainty?

## RQ-012 — Policy-search methods

Can constrained search over policy combinations identify robust trade-offs without pretending that the optimization objective is politically neutral?

## RQ-013 — Game/research dual use

How much of the research engine can be shared with a game without compromising transparency, extensibility or scientific reproducibility?

## Falsification agenda

For every major model, contributors should try to find:

- periods it cannot reproduce;
- variables it gets systematically wrong;
- parameter regions that make it unstable;
- counterfactuals that are highly sensitive to small assumptions.

A documented failure is a first-class research result.
