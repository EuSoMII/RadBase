# EuSoMII Radiomics Auditing Initiative

Welcome to the official repository of the EuSoMII Radiomics Auditing Initiative. We are currently exploring different approaches to understand the radiomics research landscape.

All researchers interested in this field are welcome to join our efforts and contribute. Please contact one of the members for further details.

If you find this repository useful for your research, please consider citing our paper: Akinci D’Antonoli, T., Cuocolo, R., Baessler, B. et al. Towards reproducible radiomics research: introduction of a database for radiomics studies. Eur Radiol (2023). https://doi.org/10.1007/s00330-023-10095-3

## Radiomics reproducibility

We are currently compiling a list of previously published radiomics studies along with relevant metadata. Some time in the future this might be made available in a more comprehensive database.

Until then all data is collected in the (`;`-separated) CSV-file of this repository. You can either download the file or access it directly from your software.

### Accessing the CSV file directly in R

```R
library(tidyverse)
library(janitor)
library(curl)

raw_csv <- curl("https://raw.github.com/EuSoMII/RadBase/master/RadBase.csv")
df <- read_csv2(raw_csv) %>% clean_names()
```
