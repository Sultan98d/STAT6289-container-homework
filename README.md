# STAT 6289 — Reproducible R Environment

This repository demonstrates how to reproduce a historical R computing environment using Docker and GitHub Codespaces.

## Environment

- R version: 4.0.5
- dplyr version: 1.0.5
- Docker image: rocker/r-ver:4.0.5

## Files

- `.devcontainer/devcontainer.json`: Configures the Codespaces environment.
- `.devcontainer/install-packages.R`: Installs dplyr using a historical CRAN repository.

## How to Reproduce

1. Open this repository on GitHub.
2. Select Code > Codespaces.
3. Create a new Codespace on the main branch.
4. Wait for the automatic package installation to finish.
5. Open the terminal and check the R and dplyr versions.

## Test

The sample analysis groups observations by A and B and calculates the mean of x and y.

Expected results:

- Group A: x = 11, y = 6
- Group B: x = 22, y = 10

The analysis uses the historical dplyr functions `summarise_each()` and `funs()`, which produce deprecation warnings.
