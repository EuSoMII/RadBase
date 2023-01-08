# EuSoMII Radiomics Auditing Initiative

Welcome to the official repository of the EuSoMII Radiomics Auditing Initiative. We are currently exploring different approaches to understand the radiomics research landscape.

All researchers interested in this field are welcome to join our efforts and contribute. Please contact one of the members for further details.

## Radiomics reproducibility

We are currently compiling a list of previously published radiomics studies along with relevant metadata. Some time in the future this might be made available in a more comprehensive database.

Until then all data is collected in the CSV-file of this repository. You can either download the file or access it directly from your software.

### Accessing the CSV file directly in R

```R
library(tidyverse)
library(janitor)
library(curl)

raw_csv <- curl("https://raw.github.com/EuSoMII/Radiomics/master/test.csv")
df <- read_csv2(raw_csv) %>% clean_names()
```