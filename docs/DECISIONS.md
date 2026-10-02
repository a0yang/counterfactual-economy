# Architecture Decision Log

Use this file to record decisions that materially affect the project.

## ADR-0001 — Model before game UI

**Decision:** Build a minimal research-grade simulation before investing heavily in graphics.

**Reason:** Scientific validity and reproducibility are harder to retrofit after a game has been built around an unstable model.

**Status:** Accepted

## ADR-0002 — Treat data vintages as a first-class concept

**Decision:** Experimental metadata should distinguish observation time from information availability.

**Reason:** A historical counterfactual should not accidentally use hindsight.

**Status:** Accepted

## ADR-0003 — Use modular economic mechanisms

**Decision:** Implement theories as explicit mechanisms and assumptions rather than fixed ideological game modes.

**Reason:** The project is intended to compare mechanisms and expose uncertainty.

**Status:** Accepted
