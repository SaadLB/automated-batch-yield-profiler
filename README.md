# Automated Yield Profiler

An R-based pipeline for programmatic exploratory data analysis (EDA) and univariate statistical profiling of continuous manufacturing processes. Built to accelerate root-cause analysis for batch yield variances.

## Data Privacy & Synthetic Data

The dataset provided in this repository (`synthetic_vaccine_batch_data.csv`) is synthetically generated. In highly regulated environments like biopharma and continuous manufacturing, production data is strictly proprietary. 

This synthetic dataset is engineered to mirror the statistical distributions, noise, and variance patterns of real-world biological manufacturing pipelines. This approach allows for a full demonstration of the statistical architecture and reporting automation without violating NDAs or exposing sensitive client data.

## Architecture

* **Engine:** R
* **Processing:** `dplyr`, `tidyr`
* **Visualization:** `ggplot2`
* **Reporting:** `RMarkdown` (compiles to standalone HTML for non-technical stakeholders)

## Usage

1. Clone the repository and ensure `synthetic_vaccine_batch_data.csv` is in the root directory.
2. Open `yield_optimization_profiler.Rmd` in RStudio.
3. Execute the script via the R console:
   ```R
   rmarkdown::render("yield_optimization_profiler.Rmd")
   ```
   *(Alternatively, use the 'Knit to HTML' function directly in the IDE).*
4. The pipeline outputs `yield_optimization_profiler.html`, containing the distribution profiles and variance mapping.