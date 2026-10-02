# GitHub setup checklist

This file is for the project maintainer when creating the public repository.

## 1. Create the repository

Recommended name:

`counterfactual-economy`

Visibility:

`Public`

Initialize without an additional README if you are uploading this package as-is.

## 2. Repository description

> Open-source platform for simulating alternative economic histories, policies, financial systems and possible futures.

## 3. Topics

Suggested topics:

`economics`, `macroeconomics`, `economic-history`, `agent-based-modeling`, `sfc`, `system-dynamics`, `financial-crisis`, `simulation`, `counterfactual`, `policy-analysis`, `economic-game`, `scientific-computing`

## 4. Enable Discussions

Recommended categories:

- General
- Economics
- Models
- Data
- Historical Cases
- Simulation
- Architecture
- Game Design
- Research Papers
- Ideas

## 5. Branch strategy

For the early project, a simple strategy is enough:

- `main` — stable public branch;
- short-lived feature branches for contributions.

Avoid a complicated branching policy until multiple maintainers exist.

## 6. Labels

Suggested labels:

- `model`
- `data`
- `research`
- `historical-case`
- `enhancement`
- `bug`
- `documentation`
- `good first issue`
- `help wanted`
- `discussion`
- `validation`
- `performance`

## 7. First pinned issues

Suggested pinned items:

1. **Project introduction** — explain the vision and how to participate.
2. **2000–2008 U.S. challenge** — define the first validation experiment.
3. **Architecture discussion** — ask contributors to challenge the proposed stack.
4. **Data sources** — collect candidate public datasets and licensing notes.

## 8. First discussion post

Question:

> What should the smallest scientifically meaningful economic simulation contain?

Invite contributors to propose the minimum set of agents, accounting identities, behavioral rules and validation tests.

## 9. Do not over-configure

Do not add a large governance system, multiple services or an elaborate CI pipeline before the first reproducible simulation exists.

The project should earn complexity as contributors and validated capabilities grow.
