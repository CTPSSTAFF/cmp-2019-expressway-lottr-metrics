# cmp-2019-expressway-lottr-metrics
Calculate AM and PM LOTTR metrics for 2019 CMP Expressways

This repository contains a Jupyter notebook and associated CSV input files to calculate the TMC-by-TMC level of travel-time reliability metrics for
the AM and PM peak periods for express highways for the 2019 Congestion Management Process. After being calculated, the metrics are saved to a CSV file.

The CSV input files are too large (approximately 300 MB each) to store in GitHub. They must be extracted by the user from Google BigQuery and downloaded as CSV files to the _data_ directory before the notebook is run.  

The relevant BigQuery tables are:
* ctps-traffic-1.INRIX_2019_Perf_Measures.INRIX_2019_cmp_dates_exp_am
* ctps-traffic-1.INRIX_2019_Perf_Measures.INRIX_2019_cmp_dates_exp_pm

Only the 'tmc' and 'travel_time' columns need be extracted, using the following queries:
```
SELECT tmc, travel_time FROM `ctps-traffic-1.INRIX_2019_Perf_Measures.INRIX_2019_cmp_dates_exp_am`
```
and
```
SELECT tmc, travel_time FROM `ctps-traffic-1.INRIX_2019_Perf_Measures.INRIX_2019_cmp_dates_exp_pm`
```
