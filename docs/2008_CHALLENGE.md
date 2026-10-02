# The 2008 Challenge

## Question

Can an economic simulation, trained and calibrated only with information that would have been available before the Global Financial Crisis, identify rising systemic vulnerability before the crisis became fully visible?

## Important distinction

The goal is **not** to predict an exact date, institution failure, or single deterministic path.

The goal is to test whether a model can:

1. reproduce important pre-crisis relationships;
2. show rising financial vulnerability before the crisis;
3. produce materially different outcome distributions under specified counterfactual policies;
4. generalize outside the exact period used for calibration.

## Information-set rule

Every experiment must state its information set.

Possible modes:

- **Vintage mode:** only information available at the historical date;
- **Final-data mode:** revised historical series;
- **Perfect-information mode:** full historical knowledge;
- **Mixed research mode:** explicitly declared analyst assumptions.

The main challenge should use vintage mode whenever feasible.

## Suggested phases

### Phase A — Baseline reconstruction

Build a model using data up to an agreed cutoff date and evaluate its ability to reproduce broad historical relationships.

### Phase B — Out-of-sample monitoring

Freeze the model and simulate subsequent periods without recalibrating on future outcomes.

### Phase C — Vulnerability indicators

Track variables such as:

- credit growth;
- household leverage;
- housing prices;
- debt-service burdens;
- bank leverage;
- capital ratios;
- short-term funding;
- asset-price volatility;
- default rates;
- liquidity stress.

### Phase D — Counterfactual policy experiments

Change one or more policies while holding other assumptions constant as far as practical.

Examples:

- stricter mortgage LTV limits;
- higher bank capital requirements;
- alternative interest-rate paths;
- alternative fiscal policy.

## Evaluation

Evaluation should include:

- forecast error metrics where meaningful;
- calibration quality;
- timing of vulnerability signals;
- false positives;
- false negatives;
- parameter sensitivity;
- model disagreement;
- reproducibility.

## What counts as success?

Success does not mean “the model predicted 2008 perfectly.”

Success means that the model demonstrates useful, transparent and reproducible information about systemic vulnerability and counterfactual policy effects without relying on hidden hindsight.

## What counts as failure?

Examples include:

- vulnerability signals appear only after the crisis;
- results depend on a narrow parameter set;
- the model only works for the calibration period;
- different reasonable assumptions create radically different conclusions with no way to diagnose why;
- accounting identities break;
- results cannot be reproduced.

Failure should be documented rather than hidden.
