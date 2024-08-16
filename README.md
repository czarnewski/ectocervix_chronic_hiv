# RNA-seq of ectocervix under chronical HIV infection

## Description

This repository hosts the code used for analysis of bulk RNAseq samples from a Kenyan cohort, which is publicly available on Gene Expression Omnibus (GEO) public repository, accession ID [GSE217237](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE217237).

> Mathias Franzén Boger, Tyra Hasselrot, Vilde Kaldhusdal, Gisele H B Miranda, Paulo Czarnewski, Gabriella Edfeldt, Genta Rexaj, Frideborg Bradley, Julie Lajoie, Kenneth Omollo, Joshua Kimani, Keith R Fowke, Kristina Broliden, and Annelie Tjernlund. **Sustained immune activation and impaired epithelial barrier integrity in the ectocervix of women with chronic HIV infection**. _Unpublished_

## Analysis Reproducibility

Analysis done herein can be reproduced using conda environment for software version management. Please follow the link [here](https://docs.conda.io/en/main/miniconda.html#installing) for instructions setting up `miniconda3` for your operational system.

1. Then, you can start by installing `mamba` and `wget` to your `base` environemnt (to speed up environement creation):

```sh
conda install -c conda-forge mamba wget
```

2. Clone this repository to your computer:

```sh
git clone https://github.com/czarnewski/ectocervix_chronic_hiv.git -p $HOME/ectocervix_chronic_hiv
cd ectocervix_chronic_hiv
```

3. Next, create the environment from the file provided:

```sh
mamba env create -f environment_20230726.yml -n ectocervix_chronic_hiv
```

4. You can now activate your environment and launch Rstudio (or use another IDE of your choice)

```sh
conda activate ectocervix_chronic_hiv

rstudio DGE_chronic_hiv.Rmd &
```

5. All done.








