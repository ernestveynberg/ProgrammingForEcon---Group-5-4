# Income Inequality and Education in the Netherlands
### Group 5.4 — Programming for Economists, VU Amsterdam

Diana Zhdanova, Ernest Veinberg, Sofiia Tataryn, Victoria Tîbuleac, Yurii Kashubin

---

## What this project does

This project examines the relationship between educational attainment and personal 
income across Dutch provinces between 2013 and 2024, using public data from 
Statistics Netherlands (CBS).

---

## How to reproduce this report

**Step 1 — Download the datasets from CBS**

Dataset 1 (Income):
https://opendata.cbs.nl/statline/#/CBS/nl/dataset/86162NED

Dataset 2 (Education):
https://opendata.cbs.nl/statline/#/CBS/nl/dataset/85525NED

The data are loaded automatically via the `cbsodataR` package — 
no manual download is needed if you have an internet connection.

**Step 2 — Clone this repository**

git clone https://github.com/ernestveynberg/ProgrammingForEcon---Group-5-4

**Step 3 — Restore packages**

Open R and run:
```r
renv::restore()
```

**Step 4 — Run the report**

```r
rmarkdown::render("Template_Assignment.Rmd")
```

Or simply run `run_all.R`, which does both steps automatically.

---

## Required packages

- tidyverse
- ggplot2
- dplyr
- sf
- knitr
- cbsodataR
- renv

All package versions are locked in `renv.lock`.

---

## Data sources

| Dataset | Description | Period | Source |
|---|---|---|---|
| 86162NED | Personal income by region | 2011–2024 | CBS StatLine |
| 85525NED | Educational attainment by region | 2013–2024 | CBS StatLine |
