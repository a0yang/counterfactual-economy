# Public Launch Post — Counterfactual Economy

## Title options

### Option A — Research-focused
**Can we build an open-source simulator for alternative economic histories?**

### Option B — More provocative
**What if governments had made different economic decisions? Let’s simulate it.**

### Option C — 2008 Challenge-focused
**The 2008 Challenge: Could an open-source model detect the financial crisis before it happened?**

---

## Main post

What if economic history had not been inevitable?

A government could have changed its interest-rate path. A regulator could have imposed different mortgage rules. A country could have chosen different fiscal, trade, industrial, or capital-control policies.

We know what happened. The interesting question is:

> **What other plausible paths might have emerged under different decisions?**

I am starting an open-source project called **Counterfactual Economy** to explore this question.

The idea is larger than a strategy game. The long-term goal is an extensible computational platform that connects:

- historical economic data;
- economic mechanisms from multiple schools of thought;
- households, firms, banks, governments, and other agents;
- production and trade networks;
- financial balance sheets and contagion;
- policy decisions;
- uncertainty and Monte Carlo experiments;
- and a lightweight 2D interface.

The same simulation engine could eventually support a game, research experiments, and current-data scenario analysis.

### The first test is intentionally small

Rather than trying to simulate the entire world from the Industrial Revolution on day one, the first target is:

**The United States, approximately 2000–2008.**

The central research question is:

> Can a transparent model using only information available at each historical point identify rising systemic financial vulnerability before the 2008 crisis became obvious in hindsight?

This is not a request for a magic prediction machine.

We do not expect a model to know the exact day of a crisis or the exact institution that will fail. We want to test something more useful and more reproducible: whether the structure of the pre-crisis economy produces measurable warning signals, and whether different policy choices change the distribution of outcomes.

### What I am looking for

I am looking for people interested in any of these areas:

**macroeconomics · economic history · computational economics · agent-based modeling · stock-flow consistent modeling · financial economics · quantitative finance · data engineering · scientific computing · Python · C++ · Rust · visualization · 2D game development · AI research**

You do not need to agree with the initial architecture. In fact, alternative approaches and failed experiments are valuable.

### What a first contribution could look like

It could be as small as:

- documenting a historical dataset;
- designing a time-series metadata schema;
- implementing one accounting identity;
- testing a household balance-sheet model;
- building a simple chart;
- proposing a financial-risk variable;
- improving documentation;
- or reviewing the architecture.

There are already starter issues for these tasks.

### A principle I want to keep from the beginning

The project should never present one model as “the truth.”

The system should make data, assumptions, parameters, mechanisms, and uncertainty visible. If two reasonable models disagree, that disagreement is part of the result.

Likewise, the real historical record should be an anchor for calibration and validation—not a hidden force that overwrites every alternative outcome.

### If this idea interests you

The repository is open for discussion, criticism, research proposals, and code contributions.

**Repository:** `https://github.com/YOUR-USERNAME/counterfactual-economy`

**Start here:**

- Project overview: `README.md`
- Research questions: `RESEARCH.md`
- Architecture: `ARCHITECTURE.md`
- 2008 Challenge: `docs/2008_CHALLENGE.md`
- Starter tasks: `docs/good-first-issues/README.md`

The project is currently at **Concept / Research Design** stage. There is deliberately more design documentation than software.

The first goal is not to build the perfect game.

It is to answer one difficult question with a transparent experiment:

> **Can we build a model that helps us explore the economic paths that history did not take?**

---

## Short version for Reddit / X / LinkedIn

**What if governments had made different economic decisions?**

I'm starting **Counterfactual Economy**, an open-source project to explore alternative economic histories through simulation.

Long-term: historical data + economic models + agents + financial networks + policy experiments + uncertainty + a lightweight 2D interface.

First target: **the U.S. 2000–2008 financial system.**

Research question: can a model using only information available at the time identify rising systemic vulnerability before the 2008 crisis became obvious in hindsight?

I'm looking for economists, computational modelers, data engineers, developers, visualization specialists, and researchers who want to challenge the idea—not just agree with it.

GitHub: `https://github.com/YOUR-USERNAME/counterfactual-economy`
