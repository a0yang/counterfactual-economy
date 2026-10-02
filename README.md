<div align="center">

<img src="assets/banner.png" alt="Counterfactual Economy — explore alternative histories, build better models, shape possible futures" width="100%">

# Counterfactual Economy

### An open-source platform for simulating alternative economic histories, policies, and possible futures.

[![Status: Concept / Research Design](https://img.shields.io/badge/status-concept%20%2F%20research%20design-blue)](ROADMAP.md)
[![License: Apache 2.0](https://img.shields.io/badge/code%20license-Apache--2.0-green.svg)](LICENSE)
[![Discussions](https://img.shields.io/badge/community-GitHub%20Discussions-purple)](https://github.com/YOUR-USERNAME/counterfactual-economy/discussions)

</div>

> **What if governments had made different economic decisions?**

Counterfactual Economy is an open-source project exploring whether historical economies can be reconstructed as transparent, extensible simulation systems.

The long-term vision is to connect historical and real-time data, economic mechanisms, heterogeneous agents, production and financial networks, policy decisions, uncertainty, and a lightweight 2D interface in one extensible platform.

The same simulation core could eventually power both:

- a **historical economic simulation game**; and
- an **open research / policy experimentation environment**.

## Why this project?

History happened once, but the economic state of the world contained many possible paths.

A government could have chosen a different interest-rate path. A regulator could have imposed a different mortgage standard. A country could have changed its tax policy, fiscal policy, trade policy, industrial policy, or capital controls.

This project asks:

> **What other plausible paths might have emerged under different decisions?**

The goal is not to claim that a model can reveal one “true” alternative history. Counterfactual results depend on data, model structure, parameters, expectations, institutions, and assumptions.

The goal is to make those assumptions **explicit, reproducible, comparable, and testable**.

## The first research challenge: 2008

The first flagship experiment is the **2000–2008 U.S. Financial Crisis Challenge**.

> Can a transparent model, using only information available at each historical point, identify rising systemic financial vulnerability before the Global Financial Crisis became fully visible?

We are **not** asking a model to guess an exact date, name a failed institution, or produce a single deterministic prediction. We want to test whether pre-crisis conditions generate measurable early-warning signals, and whether counterfactual policies change the distribution of outcomes.

→ **[Read the full 2008 Challenge](docs/2008_CHALLENGE.md)**  
→ **[Join / publish the challenge call](docs/2008_CHALLENGE_CALL.md)**

## What we are building

| Layer | Purpose |
|---|---|
| Historical data | Reconstruct economies using time-appropriate information sets |
| Economic core | Combine stock-flow consistency, agent behavior, production networks, and financial balance sheets |
| Theory modules | Add mechanisms from multiple schools of economic thought without turning them into ideological “modes” |
| Policy engine | Represent taxes, interest rates, regulation, fiscal policy, trade policy, and institutional rules |
| Counterfactual engine | Run alternative histories and compare distributions of outcomes |
| Validation | Compare simulations with historical data and out-of-sample periods |
| 2D research/game UI | Make economic mechanisms visible without spending the compute budget on 3D graphics |
| Mod system | Let contributors add countries, sectors, policies, mechanisms, datasets, and visualizations |

## Architecture

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

See **[ARCHITECTURE.md](ARCHITECTURE.md)** for the current technical design and its open questions.

## Design principles

### Model first, graphics second

The first version should prioritize reproducible calculations over visual fidelity. A low-resolution 2D interface is enough.

### Mechanisms, not ideological modes

Economic theories should appear as explicit, testable mechanisms and assumptions that can be compared under the same historical conditions.

### Historical information sets matter

A simulation intended to reproduce what decision-makers could have known in 2005 should not quietly use revised data published years later. Historical data vintages are a first-class concept.

### Reality is an anchor, not a forced answer

Historical data should calibrate and validate the model and measure divergence. The simulation should not silently overwrite a player's alternative history simply because it differs from reality.

### Uncertainty is a feature

Prefer ranges, distributions, scenario trees, confidence/calibration measures, and model disagreement over false precision.

### Reproducibility is a product feature

A serious experiment should be reconstructible from data versions, parameters, model version, assumptions, and random seed.

### Falsification is valuable

A result showing that a model does not work is a useful scientific contribution.

## Long-term ambition

The platform could eventually support:

- historical simulations from the Industrial Revolution to the present;
- country and multi-country economic systems;
- sectoral production and trade networks;
- household, firm, banking, and government agents;
- financial contagion and crisis mechanisms;
- real-time public-data adapters;
- scenario exploration for current economic conditions;
- research workflows that translate published assumptions into explicit model mechanisms;
- a mod ecosystem for new theories, policies, countries, industries, crises, and visualizations.

The project is deliberately **not** positioned as a machine that predicts the future with certainty.

Its purpose is to provide a computational laboratory for asking:

> **What could have happened, and which assumptions make that result possible?**

## Current status

**Stage: Concept / Research Design**

The repository currently contains the project architecture, research questions, data principles, the 2008 validation challenge, contribution workflows, and a roadmap. The first implementation milestone is intentionally small: build a reproducible U.S. 2000–2008 prototype before attempting a global historical simulation.

## How to contribute

You do **not** need to agree with the initial design. Criticism, alternative architectures, failed experiments, and competing models are welcome.

Start here:

- **[Contributing guide](CONTRIBUTING.md)**
- **[Good first issues](docs/good-first-issues/README.md)**
- **[Research questions](RESEARCH.md)**
- **[Data specification](DATA.md)**
- **[2008 Challenge](docs/2008_CHALLENGE.md)**

If you are interested in the project but do not know where to start, open a Discussion and introduce your background.

## Community

The project is intended to bring together people from:

**macroeconomics · economic history · computational economics · agent-based modeling · stock-flow consistent modeling · financial economics · quantitative finance · data engineering · scientific computing · visualization · game development · AI research**

See **[GOVERNANCE.md](GOVERNANCE.md)** and **[CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)** for the community framework.

## License

Software is released under **Apache License 2.0**. Documentation and other non-code materials may use the licenses stated in their respective files. External datasets remain subject to their original licenses; see **[DATA.md](DATA.md)**.

---

<div align="center">

**Different policies. Different mechanisms. Different possible histories.**

</div>
