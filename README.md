EOSC410 — PCA of U.S. Daily Climate Normals (1991–2020)

Daniel Kua & Henry Liang

🔎 Overview

This repository analyzes whether a small set of PCA modes can capture the dominant annual-cycle shapes of daily mean temperature across U.S. stations (1991–2020), and how these modes map onto spatial regimes (e.g., coastal–continental contrasts, latitude belts).

❓ Research Question

Can a few PCA modes of daily mean temperature normals (1991–2020) explain ≥90% of variance and reflect recognizable spatial regimes?

🗂️ Data

Source: NOAA/NCEI Daily Climate Normals 1991–2020, variable: daily mean temperature (Tmean)

Station selection: subset filtered to stations with complete normals.

🧰 Methods

Pre-processing (per station):

Verify completeness of normals.

Remove the station’s annual mean to emphasize the curve shape.

Standardize (z-score) the daily series.

Harmonize to 365 days.

PCA on a stations × day-of-year (365) matrix:

Choose number of components k to achieve ≥90% cumulative variance explained.

Visualize:

Cumulative variance explained curve.

Modes 1–3: spatial loadings maps + day-of-year principal component curves.

Reconstruction for contrasting stations (e.g., coastal vs interior), with RMSE/MAE and correlation metrics.
