# Quant, Alternative Data, and Applied Statistics

I am interested in problems where the answer is not sitting in one clean dataset. The projects here use financial cash flows, fund metrics, environmental sensors, weather records, and time series to build evidence from incomplete information.

There are three main threads.

## Finance and decision tools

### [Private Markets Fund Comparison](https://fundperformanceframework.streamlit.app/)

I built this to compare funds when cash-flow timing, fees, strategy mix, and terminal value all differ. It calculates XIRR and investment multiples, runs deterministic and Monte Carlo scenarios, tests when the preferred fund changes, and exports an Excel audit.

The demo uses synthetic or anonymized inputs. It is a decision model, not a return forecast.

### [Mutual Fund Ranking Pipeline](https://github.com/jbhattac2323/mutual-fund-ranking-pipeline)

This is the publishable quantitative core of a larger fund-finder prototype. It applies eligibility rules first, then ranks funds against peers using rolling-return and Sharpe percentile scores. It also keeps a separate record of exclusions so the ranking is easier to inspect.

The public repo uses synthetic fund observations and has automated tests for thresholds, ties, weighting, and peer-group logic.

## Alternative data and environmental signals

To me, alternative-data work means using several imperfect sources together and checking whether they support the same conclusion.

### [Golf Courses, Climate, and Water-Use Signals](https://github.com/jbhattac2323/evapotranspiration-land-cover-analysis)

I compared golf-course evapotranspiration with forest, urban, residential, and desert-adjacent sites, then joined the series to NOAA temperature and precipitation. The goal was to see whether ET could provide a useful water-demand signal across New York and Arizona.

The important limit is that ET is not metered irrigation. The project is useful because it combines sources and comparison groups, not because one proxy answers the whole question.

### [Environmental Sensor Quality Control](https://github.com/jbhattac2323/environmental-sensor-quality-control)

Raw station data can look precise while still being wrong. This R workflow checks physical bounds, sensor tilt, battery state, missingness, and sampling intervals before using the observations.

### [Flood-Stage Monitoring](https://github.com/jbhattac2323/flood-stage-monitoring)

This project joins river-gauge readings to site-specific thresholds, finds the first action and flood-stage crossings, and measures major-stage exceedance.

### [Climate, Emissions, and Space-Data Visualization](https://github.com/jbhattac2323/climate-emissions-visualization)

A visualization-focused R exercise using long-run emissions, temperature anomalies, and space-launch records. These are separate descriptive questions; I do not treat space activity as an explanation for climate trends.

## Statistical foundations

### [Regression and Time-Series Forecasting](https://github.com/jbhattac2323/regression-time-series-forecasting)

My strongest R coursework project. It covers transformations, multivariate regression, residual diagnostics, AIC-based selection, seasonal decomposition, autoregressive models, ARIMA forecasting, and prediction intervals.

### [R Environmental Data Fundamentals](https://github.com/jbhattac2323/r-environmental-data-fundamentals)

An early R exercise in vectorized calculations, unit conversion, data frames, indexing, and subsetting.

## Early Python work

### [Introductory Python Projects](https://github.com/jbhattac2323/intro-python-course-projects)

A clearly labeled course archive covering audio processing, text analysis, CSV grids, image manipulation, and web scraping. I kept it separate because it shows where I started, not where my quantitative work is now.

## What I am building toward

The next step is a finance-focused alternative-data project with a real validation design: a signal defined before testing, a clean train/validation split, stability checks through time, and a short write-up connecting the result to an actual decision.
