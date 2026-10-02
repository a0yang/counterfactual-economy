# Counterfactual Economy
### An Open-Source Platform for Simulating Alternative Economic Histories

> **Explore possible economic worlds — not a single predicted future.**

Counterfactual Economy is an open-source project exploring whether historical economies can be reconstructed as transparent, extensible simulation systems.

The long-term vision is to connect:

- historical and real-time economic data;
- multiple economic theories and mechanisms;
- households, firms, banks, governments and other agents;
- production and trade networks;
- financial balance sheets and contagion;
- policy decisions;
- uncertainty, Monte Carlo simulation and scenario analysis;
- a 2D interactive interface and an extensible mod system.

The same simulation core could eventually power both a **historical economic simulation game** and an **open research / policy experimentation platform**.

---

## Why this project?

History happened once, but the economic state of the world always contained multiple possible paths.

A government could have chosen a different interest-rate path. A regulator could have imposed a different mortgage standard. A country could have changed its tax policy, trade policy, industrial policy or capital controls.

This project asks:

> **What other plausible paths might have emerged under different decisions?**

The project does not assume that a model can reveal a single “true” alternative history. Counterfactual results depend on data, model structure, parameters, expectations and assumptions.

The goal is to make those assumptions explicit and computationally testable.

---

## Core research question

One of the first major validation experiments is the **2000–2008 U.S. financial crisis challenge**:

> Can a transparent model using only information that would have been available at each historical point identify rising systemic financial vulnerability before the 2008 crisis?

The project should not claim that a model can know the exact date of a crisis or the identity of a specific failed institution. A stronger and more reproducible test is whether pre-crisis conditions produce measurable changes in risk indicators, and whether counterfactual policies alter the distribution of outcomes.

---

## High-level architecture

```text
Historical / Real-Time Data
            │
            ▼
     Data Normalization
   Vintage / Revisions / Units
            │
            ▼
   ┌──────────────────────────┐
   │      Economic Core       │
   │                          │
   │ SFC + ABM + IO +         │
   │ Financial Networks       │
   └────────────┬─────────────┘
                │
                ▼
      Theory / Policy Modules
                │
                ▼
    Calibration / Validation /
       Monte Carlo / Search
                │
                ▼
       Counterfactual Engine
                │
          ┌─────┴─────┐
          ▼           ▼
        Game       Research
         UI           UI
```

The initial repository intentionally contains more design documentation than code. The first milestone is to establish a reproducible research problem before building a large user interface.

---

## Design principles

### 1. Model first, graphics second

The first version should prioritize reproducible economic calculations over visual fidelity. A low-resolution 2D interface is sufficient.

### 2. Multiple mechanisms, not ideological “modes”

Economic theories should be represented as explicit mechanisms and interchangeable assumptions rather than a single winner-takes-all economic ideology.

### 3. Historical information sets matter

When replaying history, the simulation should avoid hindsight whenever the experiment is intended to reproduce what decision-makers could have known at the time. Historical data vintages are therefore a first-class concept.

### 4. Reality is an anchor, not a forced answer

The historical record should be used to calibrate and validate the model and to measure divergence. The simulation should not silently overwrite player outcomes just because they differ from history.

### 5. Uncertainty is a feature

Outputs should often be distributions, ranges and scenario trees rather than a single deterministic number.

### 6. Reproducibility is a product feature

A serious experiment should be reconstructible from its dataset versions, parameters, model version, assumptions and random seed.

### 7. Falsification is valuable

A model that demonstrates why an approach does not work is a useful contribution.

---

## Long-term capabilities

### Historical simulation

Start from a historical year and simulate forward using information and institutional conditions appropriate to the chosen date.

### Counterfactual policy experiments

Change a policy or institutional rule and compare the resulting path with the historical baseline.

### Economic theory modules

Potential modules include Keynesian demand mechanisms, New Keynesian rules, monetary mechanisms, financial accelerator effects, Minsky-style financial fragility, adaptive expectations, rational expectations and heterogeneous-agent behavior.

### Financial crisis simulation

Represent leverage, collateral, short-term funding, bank capital, securitization, liquidity shocks and network contagion.

### Production and trade networks

Model industries, supply chains, energy inputs, international trade and cross-industry propagation.

### Real-time scenarios

Connect current public data through licensed adapters and run forward-looking scenarios under explicit assumptions.

### Modding

Enable contributors to add countries, industries, policies, institutions, crisis mechanisms, datasets and visualizations without rewriting the simulation kernel.

---

## Proposed first milestone: U.S. 2000–2008

### Scope

Initial agents:

- households;
- non-financial firms;
- commercial banks;
- government;
- central bank.

Initial variables:

- GDP;
- inflation;
- unemployment;
- interest rates;
- household income;
- household debt;
- housing prices;
- mortgage credit;
- bank capital;
- bank leverage;
- government revenue and spending.

Initial policy levers:

- policy interest rate;
- bank capital requirement;
- mortgage LTV limit;
- fiscal spending;
- selected tax parameters.

### Validation goal

The model should be evaluated against historical data without using future information during the simulated period.

### Success criteria

A successful prototype should be:

1. reproducible;
2. transparent enough for a researcher to inspect assumptions;
3. capable of reproducing broad pre-crisis relationships;
4. capable of running controlled counterfactual experiments;
5. explicit about where it fails.

---

## Possible technology stack

The technology stack is intentionally not fixed yet.

A possible direction is:

- **Python** for rapid prototyping, calibration and research workflows;
- **Rust or C++** for performance-critical simulation components if needed;
- **Godot** for a lightweight 2D client and visualization layer;
- **SQLite / DuckDB / Parquet** for local research datasets;
- standard scientific Python tools for statistics, optimization and analysis.

The first contributors should be allowed to propose alternatives.

---

## Who should contribute?

The project is especially interested in people with experience in:

- macroeconomics;
- economic history;
- computational economics;
- agent-based modeling;
- stock-flow consistent modeling;
- system dynamics;
- financial economics;
- quantitative finance;
- data engineering;
- scientific computing;
- Python, C++, Rust or similar languages;
- 2D game development and visualization;
- machine learning / AI for research workflows.

You do not need to agree with every initial design choice. Critical discussion is explicitly welcome.

---

## Current status

**Stage: Concept / Research Design**

There is no finished game and no validated general-purpose economic simulator yet.

The repository is intended to turn the concept into an open, testable and collaborative research program.

---

## Roadmap

See [ROADMAP.md](ROADMAP.md).

Research questions are tracked in [RESEARCH.md](RESEARCH.md).

Architecture is described in [ARCHITECTURE.md](ARCHITECTURE.md).

Historical data and data-vintage requirements are described in [DATA.md](DATA.md).

---

## Project identity

**Project name:** Counterfactual Economy  
**Repository:** `counterfactual-economy`  
**Primary language:** English  
**Chinese documentation:** `README.zh-CN.md`

Suggested GitHub description:

> Open-source platform for simulating alternative economic histories, policies, financial systems and possible futures.

Suggested topics:

`economics` `macroeconomics` `economic-history` `agent-based-modeling` `sfc` `system-dynamics` `financial-crisis` `simulation` `counterfactual` `policy-analysis` `economic-game` `scientific-computing`

---

## License

The initial software and documentation in this repository are released under the Apache License 2.0 unless a file states otherwise.

Third-party data and external research materials remain subject to their original licenses. See [DATA.md](DATA.md).
