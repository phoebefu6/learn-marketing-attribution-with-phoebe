# Official course map - learn-marketing-attribution-with-phoebe

Two tracks, one running project (Lumen Skincare). Leader = 6 x 45 min, exec thinking-mode, no
code. Builder = 10 x 45 min, Python/SQL. 80% bar: each session teaches ~80% of its mapped
sources' working content; certificates/videos stay official.

## Source universe (verified July 2026)
- LinkedIn Learning - "Marketing Attribution and Mix Modeling" (Michael Taylor) - leader spine
- Udemy - "Marketing Measurement: Attribution to Incrementality" - modern-stack map
- PyMC Labs - "Bayesian Marketing Analytics" - builder MMM backbone
- Udemy - "Advanced Attribution using R" (ChannelAttribution) - Markov/Shapley code
- Meta Blueprint - Conversion Lift path (free) - incrementality
- Google Skillshop - Analytics Certification (free) - GA4 DDA as configured
- Udemy - "Fundamentals of MMM: Learn by Doing" - MMM on-ramp
- Coursera - "Data Science for Marketing" (CU Boulder) - Markov/Bayesian academic
- Papers: Shao & Li 2011 (data-driven MTA); DNAMTA (arxiv 1809.02230); DeepMTA (2004.00384);
  Shapley (1804.05327). Docs: GA4 attribution, Google Meridian, Meta Robyn.

## Coverage gaps this course OWNS (no existing course teaches well)
1. The actual math of Markov + Shapley from scratch in Python (B4, B5)
2. Same business question answered 3 ways (MTA/MMM/incrementality) + why they disagree (A4, B10)
3. 2026 cookieless reality tied to method choice (A5, B7, B10)
4. Leader "so what": credit -> defensible budget reallocation (A6)
5. SQL to build the touchpoint/journey table (B1)

## Leader track coverage (a1-a6)
| # | Session | Live parts | Maps to |
|---|---------|-----------|---------|
| A1 | The credit problem | one journey / 8 models / 8 answers; why attribution exists | LI Learning ch.1, Udemy measurement intro |
| A2 | The heuristics you already use | first/last/linear/time-decay/position - biases, reading platform reports | LI Learning ch.2, Skillshop |
| A3 | Data-driven decoded | Markov removal-effect + Shapley fairness (concept, no math); GA4 DDA black box | LI Learning ch.3, Skillshop DDA |
| A4 | MMM vs MTA vs Incrementality | same question 3 ways, why numbers disagree, decision-by-budget-tier | LI Learning ch.4, Udemy measurement |
| A5 | The 2026 cookieless break | ATT/SKAN-AAK/cookies killed MTA, MMM+lift resurgence, what to demand | Meta Blueprint, industry 2026 |
| A6 | Credit to budget (capstone) | turn attribution output into a spend reallocation a CDAIO signs; Lumen budget | synthesis |

## Builder track coverage (b1-b10)
| # | Session | Build-along | Maps to |
|---|---------|------------|---------|
| B1 | Touchpoint data model + SQL journeys | sessionize, path table, window functions | GAP #5 (original) |
| B2 | Heuristics in SQL/Python | first/last/linear/time-decay/position on Lumen | LI Learning, Udemy |
| B3 | Why heuristics fail -> data-driven leap | Shao-Li bagged logistic | Shao & Li 2011 |
| B4 | Markov from scratch | transition matrix, removal effect, ChannelAttribution | GAP #1, Udemy R course |
| B5 | Shapley from scratch | coalitions, marginal contribution, SHAP bridge, Monte-Carlo | GAP #1, Shapley paper |
| B6 | ML/DL attribution | LightGBM+SHAP; LSTM/attention concept (when worth it) | DNAMTA, DeepMTA |
| B7 | GA4 DDA + reconciliation | DDA in practice, double-counting across tools | Skillshop, GA4 docs |
| B8 | MMM pt1: adstock + saturation | Meridian/PyMC-Marketing, Hill curve, adstock | PyMC Labs, Meridian docs, Udemy MMM |
| B9 | Incrementality + geo-lift | holdout design, synthetic control, calibrate MMM priors | Meta Blueprint, GeoLift |
| B10 | The unified 2026 stack (capstone) | orchestrate MMM+MTA+lift, pitfalls, ethics | synthesis |

## Depth beyond 45 min
Folded into `Self-study` accordion cards inside each session (LSTM math, Bayesian MMM internals,
higher-order Markov, Monte-Carlo Shapley proofs). No separate deep-dive track for this course.

## Not covered by design (honest list)
- Vendor certificates/quizzes (Google Analytics cert, Meta Blueprint badges) - stay official.
- Full production data-engineering (Snowplow/Segment setup) - named, not built.
- Vendor-specific ad-platform UI clicks - we teach the method, not the button locations.
- Live API keys / real ad-account data - Lumen is synthetic.

Re-verify before delivery: MMM tooling (Meridian releases), Apple AAK changes, cookie status.
