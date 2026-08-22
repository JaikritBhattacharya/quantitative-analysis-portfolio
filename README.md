# Quantitative Analysis Portfolio

A curated portfolio spanning financial modeling, alternative data, statistical analysis, time-series methods, data quality, and reproducible analytical software.

## Alternative data and triangulation

A recurring research theme is extracting defensible signals from unconventional or fragmented data. My approach is to:

1. define what each dataset measures—and what it only approximates;
2. validate provenance, coverage, timing, and missingness before modeling;
3. triangulate independent sources or comparison groups;
4. quantify uncertainty and sensitivity; and
5. connect the resulting signal to a concrete decision without presenting correlation as causation.

The golf-course sustainability study is the clearest environmental example: site-level evapotranspiration is treated as a proxy for landscape water demand, NOAA temperature and precipitation provide climate context, nearby land-cover types provide benchmarks, and New York–Arizona comparisons test whether observed patterns persist across very different climates. The analysis does **not** claim to measure irrigation withdrawals directly.

## Featured work

### [Private Markets Fund Performance & Fee Comparison Framework](https://fundperformanceframework.streamlit.app/)

A tested Python and Streamlit decision system for comparing private-market funds.

**Methods:** dated cash-flow analysis, XIRR, DPI/RVPI/TVPI, deterministic scenarios, exact Shapley attribution, decision-switch thresholds, paired Monte Carlo simulation with correlated drivers, sensitivity diagnostics, and formula-backed Excel reconciliation.

The application uses synthetic or anonymized demonstration inputs and is designed for transparent assumption analysis rather than return prediction.

### [Mutual Fund Ranking Pipeline](https://github.com/jbhattac2323/mutual-fund-ranking-pipeline)

A privacy-safe Python case study extracted from an advisor-facing research prototype. It screens a synthetic fund universe, normalizes rolling-return and Sharpe observations within peer categories, produces configurable weighted rankings, and reports every exclusion reason for auditability.

**Methods:** universe construction, explicit eligibility rules, midrank percentiles, category-relative scoring, deterministic tie handling, data-governance boundaries, and unit-tested methodology.

### [Regression Diagnostics and Evapotranspiration Forecasting](https://github.com/jbhattac2323/regression-time-series-forecasting)

An applied R project combining multivariate regression, transformations, residual diagnostics, AIC-based model selection, time-series decomposition, and ARIMA forecasting with prediction intervals.

### [Environmental Sensor Quality-Control Pipeline](https://github.com/jbhattac2323/environmental-sensor-quality-control)

An R workflow for converting raw weather-station telemetry into trustworthy analytical evidence using physical bounds, sensor tilt, battery state, temperature-dependent precipitation screening, missingness checks, and sampling-interval diagnostics.

### [Golf-Course Water Sustainability Through Alternative Data](https://github.com/jbhattac2323/evapotranspiration-land-cover-analysis)

An exploratory R time-series study that triangulates site-level evapotranspiration, NOAA climate observations, nearby land-cover benchmarks, and cross-region comparisons. ET is used as a proxy for landscape water demand—not as a direct measure of irrigation withdrawals—to examine how golf-course water signals vary by season and climate context.

**Methods:** multi-source joins, temporal aggregation, seasonal decomposition, proxy validation, benchmark construction, distributional comparison, and correlation analysis with explicit causal limits.

### [Flood-Stage Monitoring in R](https://github.com/jbhattac2323/flood-stage-monitoring)

A hydrology analysis that joins gauge observations to site-specific thresholds, detects the first crossing of action and flood stages, and measures major-stage exceedance.

## Coursework archive

### [Introductory Python Course Projects](https://github.com/jbhattac2323/intro-python-course-projects)

An openly labeled CPSCI 101 archive covering audio remixing, NLTK-based text analysis, CSV-grid validation, pixel-level image processing, and web scraping. Shared-author submissions, course materials, personal contact details, full literary texts, and media with uncertain reuse rights are excluded.

## Technical toolkit

| Area | Tools and methods |
|---|---|
| Programming | Python, R, SQL-oriented data modeling |
| Alternative data | Source triangulation, proxy validation, provenance, benchmark construction, coverage and missingness diagnostics |
| Statistical analysis | Regression diagnostics, transformations, peer-relative normalization, correlation, model selection, uncertainty intervals |
| Time series | Seasonal decomposition, autoregressive models, ARIMA forecasting |
| Quantitative finance | Cash-flow modeling, XIRR, investment multiples, fund screening, scenario analysis, Monte Carlo |
| Data engineering | Validation rules, joins, reproducible pipelines, provenance, sensor quality control |
| Software quality | Unit, integration, and regression tests; CI; Docker; audit-ready Excel exports |

## Current direction

I am developing this portfolio for quantitative-analyst roles and data-science-oriented graduate study. The next phase is to extend the alternative-data theme with research-grade projects that use explicit train/validation/test design, signal-stability analysis, stronger causal or predictive evaluation, and concise write-ups connecting evidence to decisions.

> Course exercises are labeled honestly as instructional work. Project READMEs distinguish reproducible results from archived analyses and state important statistical limitations.
