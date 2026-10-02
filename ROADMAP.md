# Roadmap

## Phase 0 — Open the research project

**Status: starting**

- publish project vision;
- establish contribution rules;
- agree on research questions;
- collect candidate datasets;
- define reproducibility requirements;
- recruit the first collaborators.

## Phase 1 — Minimal research core

Build a small, testable model in Python.

Target components:

- sectors and agents;
- basic national accounts;
- household consumption;
- firm production and investment;
- government budget;
- central-bank policy rate;
- simple banking balance sheet.

Deliverable:

> a reproducible simulation notebook / script with tests.

## Phase 2 — U.S. 2000–2008 challenge

Add:

- housing;
- mortgages;
- household leverage;
- bank capital;
- credit growth;
- selected financial-market variables.

Deliverables:

- historical baseline;
- out-of-sample protocol;
- vulnerability indicators;
- policy counterfactual experiments.

## Phase 3 — Financial network

Add:

- interbank exposures;
- short-term funding;
- liquidity shocks;
- collateral and fire sales;
- default propagation.

## Phase 4 — Production network and international sector

Add:

- multiple sectors;
- imports/exports;
- exchange rate;
- commodity inputs;
- energy sector;
- external financing.

## Phase 5 — 2D simulation interface

Implement a lightweight client with dashboards, maps, timelines and policy controls.

## Phase 6 — Mod architecture

Define stable schemas for:

- countries;
- policies;
- sectors;
- institutions;
- models;
- historical scenarios.

## Phase 7 — Multiple historical episodes

Potential validation episodes:

- Great Depression;
- post-war inflation;
- Japan asset bubble;
- Asian financial crisis;
- dot-com bubble;
- Global Financial Crisis;
- euro-area sovereign stress;
- pandemic shock.

Each episode must use a clearly defined information set and evaluation protocol.

## Phase 8 — Current-data scenario engine

Connect licensed public data adapters and allow users to define explicit forward-looking assumptions.

## Phase 9 — Research/report integration

Add tools that can translate published research into explicit assumptions and model components, while keeping a clear distinction between source claims and simulation-generated results.

## Phase 10 — Mature ecosystem

Potential targets:

- mod marketplace / catalog;
- model comparison leaderboards;
- reproducible experiment packages;
- educational scenarios;
- researcher APIs;
- optional commercial game front end.

## Guiding rule

**Do not move to a later phase merely because the previous phase “runs.” Move when the previous phase can be independently validated.**
