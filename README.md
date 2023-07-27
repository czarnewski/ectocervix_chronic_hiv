# RNA-seq of ectocervix under chronical HIV infection

## Description

This repository hosts the code used for analysis of bulk RNAseq samples from Kenyan donor cohort, which is publicly available on Gene Expression Omnibus (GEO) public repository, accession ID [GSE217237](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE217237).

> Mathias Franzén Boger,1 Tyra Hasselrot,1 Vilde Kaldhusdal,1 Gisele H B Miranda,2,3 Paulo Czarnewski,4 Gabriella Edfeldt,1 Frideborg Bradley,1 Julie Lajoie,5 Joshua Kimani,5,6,7 Julius Oyugi,5,6 Kenneth Omollo,6 Keith R Fowke,5,6,7,8 Kristina Broliden,1 and Annelie Tjernlund1. **Downregulation of Epithelial Junction Proteins and Structural Disruption of the Ectocervical Epithelium in Women with Chronic HIV Infection**. _Unpublished_

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








