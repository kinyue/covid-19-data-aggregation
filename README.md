# covid-19-data-aggregation
The aggregation of various datasets related to covid-19, being updated by scripts automatically.

## Type of source
All dataset comes from two types of sources, one is the other github repository like [JHU CSSE](https://github.com/CSSEGISandData/COVID-19) stat data, the other type is downloadable content from websites like [ecdc](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide). 

## Mode of archive
For some dataset which are providing historical data like [csse_covid_19_daily_reports](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Cases%20Stat%20from%20JHU%20CSSE/csse_covid_19_daily_reports), no archiving activate. For the other dataset, archive will saved in a sub-folder like [csse_covid_19_time_series](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Cases%20Stat%20from%20JHU%20CSSE/csse_covid_19_time_series) and file will be named with its md5 value.

## Folder structure

.
├── source1 (datasource 1, it may include few datasets)
│   ├── dataset_s1_1 (dataset 1 of datasource 1, no archive)
│   │   ├── datafile_s1_d1_1 (data file 1 of dataset 1 of datasource 1, no archive)
│   │   ├── datafile_s1_d1_2 (data file 2 of dataset 1 of datasource 1, no archive)
│   │   └── ...
│   ├── dataset_s1_2 (dataset 2 of datasource 1, with archive)
│   │   ├── archived (archive folder for dataset 2 of datasource 1)
│   │   │   ├── datafile_s1_d2_1_md5 (archived file with its md5 value)
│   │   │   └── ...
│   │   ├── datafile_s1_d2_1 (data file 1 of dataset 2 of datasource 1)
│   │   ├── datafile_s1_d2_2 (data file 2 of dataset 2 of datasource 1)
│   │   └── ...
│   ├── img
│   │   ├── figure1
│   │   └── ...
│   └── README.md (description of datasource 1)
├── source2 (datasource 2, it may include few datasets)
│   ├── ...
│   └── README.md
├── LICENSE
└── README.md

## List of datasets
|Source|Data Set|Source Type|Have Archive? |Data Type|
|---|---|---|---|---|
|[Cases Stat from JHU CSSE](https://github.com/CSSEGISandData/COVID-19)|[csse_covid_19_daily_reports](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Cases%20Stat%20from%20JHU%20CSSE/csse_covid_19_daily_reports)|Github Repository|No|Daily report|
|[Cases Stat from JHU CSSE](https://github.com/CSSEGISandData/COVID-19)|[csse_covid_19_time_series](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Cases%20Stat%20from%20JHU%20CSSE/csse_covid_19_time_series)|Github Repository|Yes|Time series|
|[Cases Stat from JHU CSSE](https://github.com/CSSEGISandData/COVID-19)|[who_covid_19_sit_rep_time_series](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Cases%20Stat%20from%20JHU%20CSSE/who_covid_19_sit_rep_time_series)|Github Repository|Yes|Time series|
|[ECDC](https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide)|[Geographic distribution of COVID-19 cases worldwide from ecdc](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Geographic%20distribution%20of%20COVID-19%20cases%20worldwide%20from%20ecdc)|Web Page|Yes|Daily report|
|[Oxford](https://www.bsg.ox.ac.uk/sites/default/files/OxCGRT_Download_latest_data.xlsx)|[Oxford covid 19 government response tracker](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Oxford%20covid%2019%20government%20response%20tracker)|Web Page|Yes|Policy|
|[Nextstrain](https://github.com/nextstrain/ncov)|[SARS-CoV-2 genomes from Nextstrain](https://github.com/kinyue/covid-19-data-aggregation/tree/master/SARS-CoV-2%20genomes%20from%20Nextstrain)|Github Repository|Yes|Gene Data|
|Others|[Static data or metadata](https://github.com/kinyue/covid-19-data-aggregation/tree/master/Static)|Various|Yes|Metadata|