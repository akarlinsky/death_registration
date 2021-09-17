# International Completeness of Death Registration 2015-2019
This repository contains inputs and outputs of the paper: _International Completeness of Death Registration 2015-2019_, which contains the most up to date estimates of the completness of death registration in 147 countries around the world. 

Paper and sources are detailed in (preprint): https://doi.org/10.1101/2021.08.12.21261978

Contrbuitions and suggestions of information and data are welcome and will be credited.

## Contents

### 
`death_reg_final` is a csv file in easy to use machine-readable, longditundal format, from which all the analyses in _International Completeness of Death Registration 2015-2019_ can be reproduced. The variables in the file are:

* `country_name`: Name of the country. 
* `year`: Year, ranges from 2015 to 2019.
* `reg_deaths`: The number of deaths registered in the vital registration system for the country-year. NA denotes no registerd deaths data was obtained.
* `expected_wpp`: The number of deaths expected to occur for the country-year from [World Population Prospects 2019](https://population.un.org/wpp/).
* `expected_gbd`: The number of deaths expected to occur for the country-year from [Global Burden of Disease 2019](http://ghdx.healthdata.org/gbd-results-tool).
* `expected_deaths`: The mean of `expected_wpp` and `expected_gbd`.
* `death_comp`: The estimated completness rate, ranges from 0 to 100. Derived as `reg_deaths` divided by `expected_deaths`. See paper for details.
* `source`: Whether the source is WMD (World Mortaity Dataset) or other.
