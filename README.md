# Ethan Levy

I trained in geology, physics and mathematics, then completed a master's in
hydrology and water quality. I have worked on environmental data and on
fraud-detection models in production, and I am now the founding engineer at a
small AI startup. The projects below apply that background to public
earth-science data. Each asks one question, states its finding, and documents
the sampling, measurement and modelling choices that affect the conclusion.

[Portfolio and study reports](https://ethannol.github.io/portfolio/)

## Studies

| Project | Finding | Approach |
| --- | --- | --- |
| [Groundwater audit](https://github.com/ethannol/groundwater-audit) | County-wide shifts in nitrate and arsenic reflect a change in which wells were sampled. At wells sampled in both periods nitrate did not decline, and the arsenic change is within measurement noise. An LLM analyst got the numbers right; its errors were definitional. | Censored measurements, consistent-cohort comparison, and a bounded evaluation of AI-assisted analysis. |
| [Mineral prospectivity](https://github.com/ethannol/mineral-prospectivity) | Reported skill falls when nearby locations are kept together during validation. The model misses the useful-skill threshold set before fitting, and the remaining signal reflects rock type. | Geochemical features, spatial cross-validation, and laboratory effects in Nevada gold-producer data. |
| [Animas River after Gold King](https://github.com/ethannol/animas-gold-king) | No lasting change in dissolved zinc at Cement Creek is detected. The estimate depends on the comparison period, and the treatment plant started too soon after the release to separate the two. | Flow adjustment, interrupted time series, and a sensitivity grid over the comparison period. |
| [Produced-water lithium](https://github.com/ethannol/produced-water-lithium) | The database supports a first screen of measured wells but cannot say how much lithium a basin contains. Prediction error rises for a new basin, and non-detects cannot be identified. | Missingness audit, dataset effects, clustered uncertainty, and prediction across basins. |

## Tools and worked examples

- [Statistics cheat sheet](https://github.com/ethannol/stats-cheatsheet): runnable examples for environmental and mining data, with assumptions and interpretation.
- [Cairn](https://github.com/ethannol/cairn): verification and reproducibility tooling for AI-assisted analysis.
- [Groundwater BI](https://github.com/ethannol/groundwater-bi): a dbt/DuckDB warehouse, offline LookML validation, and an authenticated embed host, all runnable from a fresh checkout. A published Hex app, a live Looker instance and an exercised Metabase dashboard are planned, not shown.

## How AI was used

I chose the questions and reviewed each pre-registration, test suite and set of
findings. The code was written in Claude Code sessions, and every number in a
report is a ledger value produced by a script. Each study README says exactly
what the agent did and distinguishes recorded evidence from claims the data
cannot support.
