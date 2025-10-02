# Detecting Anomalous Market Stress Periods (2007–2009)

A compact notebook that flags unusual “stress” days in financial markets around the 2008 crisis using unsupervised anomaly detection.

## What it does

- Pulls/loads key stress indicators (e.g., VIX, TED spread, yield/credit spread proxies).
- Cleans/aLigns daily time series and visualizes distributions/correlations.
- Scores each day for “outlierness” (Isolation Forest), then highlights high-stress windows on a timeline.
- Compares model scores to well-known 2008 events for sanity-check.

## Why it’s useful

- Shows a practical, end-to-end anomaly-detection workflow on real market data.
- Emphasizes interpretability with clear plots and thresholding logic.
- Minimal dependencies; easy to reuse on other time-series feature sets.

## Results (high level)

- The anomaly score surfaces concentrated stress windows in 2008 consistent with major crisis headlines (e.g., mid-September and October).
- Plots include: distributions, correlations, rolling trends, and a time-axis with shaded “anomaly” periods.

## Tech stack

- Python (pandas, numpy, scikit-learn, matplotlib)
- Method: Isolation Forest (unsupervised), plus simple statistical baselines/visual checks.
