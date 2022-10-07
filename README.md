# cmp-2019-expressway-lottr-metrics
Calculate AM and PM LOTTR metrics for 2019 CMP Expressways

This repository contains a Jupyter notebook and associated CSV input files to calculate the TMC-by-TMC level of travel-time reliability metrics for
the AM and PM peak periods for express highways for the 2019 Congestion Management Process. After being calculated, the metrics are saved to a CSV file.

The CSV input files were obtained by extracting the 'tmc' and 'travel_time' fields from all records in the Google BigQuery tables:
* ctps-traffic-1.INRIX_2019_All.INRIX_2019_cmp_dates_exp_am
* ctps-traffic-1.INRIX_2019_All.INRIX_2019_cmp_dates_exp_pm
