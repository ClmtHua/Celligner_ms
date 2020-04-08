# Celligner_ms
This repo contains code associated with the manuscript describing Celligner, our method for aligning tumor and cell line transcriptional profiles.

## Data

The data associated with this analysis is available from public data repositiories, supplementary data files associated with the manuscript (https://www.biorxiv.org/content/10.1101/2020.03.25.008342v1.supplementary-material), and in the figshare: https://figshare.com/articles/Celligner_data/11965269.

The cell line data used as input can be found at depmap.org (the file is DepMap Public 19Q4 CCLE_expression_full.csv)

The tumor data used as input is from the treehouse dataset, available here: https://xenabrowser.net/datapages/?dataset=TumorCompendium_v10_PolyA_hugo_log2tpm_58581genes_2019-07-25.tsv&host=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443

## Organization of repo

The code can be organized into config files, helper functions, and analysis/figure generation scripts.

NOTE: The functions can be run using data available with the manuscript and data from publicly available resources (primarily depmap.org and xena browser)

### Configs

global_params.R: Define global params shared across analysis scripts. Includes parameters used to run Celligner alignment and parameters used for creating plots.

### Helper functions

- analysis_helpers.R: Define helper functions used throughout the analysis and creation of figures
- Celligner_helpers.R : Define helper functions used for the Celligner alignment method

### Analysis/fig-gen

- Celligner_methods.R : Functions to run the various stages and entire Celligner alignment method
- There are separate scripts for each of the main and supplementary figure panels within the manuscript.
