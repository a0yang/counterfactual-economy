# Call for Participants: The 2008 Challenge

> **Could an economic simulation detect the growing risk of the 2008 financial crisis before it happened?**

Counterfactual Economy is looking for researchers, developers, economists, data scientists, and curious independent contributors to build a reproducible open-source experiment around the U.S. financial system from roughly 2000 to 2008.

## The question

Can a model, calibrated only with information that would have been available at each historical point, identify increasing systemic financial vulnerability before the Global Financial Crisis became obvious in hindsight?

This is deliberately a harder and more scientific question than “can we predict 2008?”

We want to separate:

- pre-crisis vulnerability;
- model assumptions;
- observable information;
- unexpected triggers;
- and the final historical outcome.

## Rules for the main track

The main track should use a **historical information set**.

For each simulated date, contributors should document what data, revisions, model updates, and external information were available at that time.

We encourage three tracks:

### Track A — Vintage / real-time information

Use the best available historical-vintage data and freeze the information set as the simulation advances.

### Track B — Final revised data

Use today's revised historical series. This is useful as a benchmark but should not be confused with an ex-ante test.

### Track C — Alternative models

Use deliberately different model structures, expectations, or financial mechanisms and compare the results.

## Suggested initial variables

Contributors may use different datasets and models, but the first prototype should try to cover some combination of:

- housing prices;
- mortgage credit;
- household leverage;
- debt-service burdens;
- bank leverage;
- bank capital ratios;
- short-term funding;
- interest rates;
- unemployment;
- household income;
- asset prices;
- securitization;
- defaults and delinquencies;
- government fiscal conditions.

## What to submit

A useful contribution can be a model, a dataset adapter, a validation experiment, or a research note.

At minimum, a model submission should document:

1. data sources;
2. information-set / vintage rules;
3. equations or decision rules;
4. calibration procedure;
5. parameters and ranges;
6. random seed or deterministic execution settings;
7. validation method;
8. what would count as a failure of the model.

## What counts as a meaningful result?

Examples include:

- an interpretable vulnerability signal that appears before major crisis events;
- a model that reproduces important pre-crisis relationships;
- a counterfactual policy experiment with clearly separated assumptions;
- evidence that a commonly used mechanism is not sufficient by itself;
- a comparison showing why two reasonable models disagree.

A failed prediction is still useful when the failure is reproducible and diagnostically explained.

## What we do not claim

This challenge is not intended to prove that one economic theory is “correct,” that a crisis can be predicted exactly, or that any policy can be shown to have one inevitable outcome.

Economic models are conditional systems. Their conclusions depend on structure, data, calibration, expectations, institutions, and shocks.

## How to join

Start by opening a GitHub Discussion or a Research/Data issue and state:

- your background;
- what part of the challenge you want to work on;
- what data or model you propose;
- and whether you intend to work in Track A, B, or C.

For people who want a smaller first contribution, see **[Good First Issues](good-first-issues/README.md)**.

## Long-term goal

If the first 2000–2008 experiment is successful, the framework can be generalized to other historical episodes, countries, sectors, financial systems, and current-data scenarios.

The ambition is to make alternative economic history something that can be **simulated, inspected, debated, and reproduced**.
