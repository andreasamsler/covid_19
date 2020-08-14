<img src="https://github.com/openZH/covid_19/blob/master/statistisches_amt_kt_zh.png" alt="OpenZH-logo" width="180"/>
<img src="https://github.com/openZH/covid_19/blob/master/gd.png" alt="GD-logo" width="200"/>

[![GitHub commit](https://img.shields.io/github/last-commit/openZH/covid_19)](https://github.com/openZH/covid_19/commits/master)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openZH/covid_19/master?filepath=visualise.ipynb)

# SARS-CoV-2 open government datasets 

## Aim

The aim of this repository is to provide open government datasets for SARS-CoV-2 related data reported by the Swiss Cantons and the Principality of Liechtenstein. Since Jun 8, 2020 most cantons report case numbers once or twice a week. Updates of cantonal case numbers during weekends are infrequent.

If you have any questions, please don't hestitate to contact us: <br>
https://twitter.com/OpenDataZH (follow us, we send you a private Direct Message, thanks!) <br>
mailto:info@open.zh.ch <br>

## List of open government datasets published in this repository

**Swiss Cantons and Principality of Liechtenstein** <br>
- [Unified dataset](https://github.com/kalakaru/covid_19/blob/master/README.md#swiss-cantons-and-principality-of-liechtenstein-unified-dataset) <br>
- [More detailed dataset](https://github.com/kalakaru/covid_19/blob/master/README.md#swiss-cantons-and-principality-of-liechtenstein-more-detailed-dataset) <br>

**Conton Zürich** <br>
- [Unified dataset](https://github.com/kalakaru/covid_19/blob/master/README.md#conton-z%C3%BCrich--unified-dataset) <br>
- [More detailed dataset](https://github.com/kalakaru/covid_19/blob/master/README.md#conton-z%C3%BCrich-more-detailed-dataset)<br>
- [Postal codes (Postleitzahl)](https://github.com/kalakaru/covid_19/blob/master/README.md#conton-z%C3%BCrich-postal-codes-postleitzahl)<br>
- [Districts (Bezirk)](https://github.com/kalakaru/covid_19/blob/master/README.md#conton-z%C3%BCrich-districts-bezirk)<br>

Don't forget to take a look at the [community contributions](https://github.com/kalakaru/covid_19/blob/master/README.md#community-contributions).

## Swiss Cantons and Principality of Liechtenstein: Unified dataset

**General description** <br>
This data is generated and validated daily at 6pm using manual and automated procedures. Note that we only publish data that are reported by the Swiss Cantons and the Principality of Liechtenstein. Thus, gaps result if Swiss Cantons or the Principality of Liechtenstein do not report data for the specific date. 

**Data** <br>

>**https://github.com/openZH/covid_19/tree/master/fallzahlen_kanton_total_csv_v2** <br>
>*Description:* Case numbers for each spatial unit separately.  <br>
>*Spatial unit:* Swiss cantons and Principality of Liechtenstein <br>
>*Format:* csv <br>
>??? *Additional remark*: In contrast to https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv/ 

>**https://github.com/openZH/covid_19/blob/master/COVID19_Fallzahlen_CH_total_v2.csv** <br>
>*Description:* Case numbers for all spatial units in one single file.  <br>
>*Spatial unit:* Swiss cantons and Principality of Liechtenstein <br>
>*Format:* csv <br>
>??? *Additional remark*: In contrast to https://github.com/openZH/covid_19/blob/master/COVID19_Fallzahlen_CH_total.csv ... 


**Metadata**

| Field Name          | Description                                | Format     | Note |
|---------------------|--------------------------------------------|------------|------|
| __date__              | Date of notification                       | YYYY-MM-DD | |
| __time__                 | Time of notification                       | HH:MM      | |
| __abbreviation_canton_and_fl__  | Abbreviation of the reporting canton       | Text       | |
| __ncumul_tested__      | Reported number of tests performed as of date| Number     | Irrespective of canton of residence |
| __ncumul_conf__          | Reported number of confirmed cases as of date| Number     | Only cases that reside in the current canton |
| __new_hosp__        | new hospitalisations since last date | Number     | Irrespective of canton of residence |
| __current_hosp__       | Reported number of hospitalised patients on date | Number     | Irrespective of canton of residence |
| __current_icu__       | Reported number of hospitalised patients in ICUs on date| Number     | Irrespective of canton of residence |
| __current_vent__        | Reported number of patients requiring invasive ventilation on date | Number     | Irrespective of canton of residence |
| __ncumul_released__     |Reported number of patients released from hospitals or reported recovered as of date| Number     | Irrespective of canton of residence |
| __ncumul_deceased__     |Reported number of deceased as of date| Number     | Only cases that reside in the current canton |
| __source__              | Source of the information                  | href       | |
| __current_isolated__       | Reported number of isolated persons on date          | Number       | Infected persons, who are not hospitalised |
| __current_quarantined__    | Reported number of quarantined persons on date       | Number       | Persons, who were in 'close contact' with an infected person, while that person was infectious, and are not hospitalised themselves |

**Empty values vs. 0**

| Value    | Meaning |
|----------| --------|
| 0        | Zero cases are reported.
|empty     | No value is reported.

**Data collection** <br>

This list provides an overview of how the data is collected: <br>

 Canton / FL | updated by | data historized |
|-------------|------------|-----------------|
|[FL](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_FL_total.csv)|scraping|yes|
|[AG](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_AG_total.csv)|scraping|yes|
|[AI](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_AI_total.csv)|scraping|yes|
|[AR](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_AR_total.csv)|scraping|yes|
|[BE](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_BE_total.csv)|scraping|yes|
|[BL](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_BL_total.csv)|scraping|yes|
|[BS](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_BS_total.csv)|manually|yes|
|[FR](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_FR_total.csv)|scraping|yes|
|[GE](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_GE_total.csv)|scraping|yes|
|[GL](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_GL_total.csv)|scraping|yes|
|[GR](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_GR_total.csv)|scraping|yes|
|[JU](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_JU_total.csv)|scraping|yes|
|[LU](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_LU_total.csv)|scraping|yes|
|[NE](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_NE_total.csv)|scraping|yes|
|[NW](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_NW_total.csv)|scraping|yes|
|[OW](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_OW_total.csv)|scraping|yes|
|[SG](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_SG_total.csv)|scraping|yes|
|[SH](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_SH_total.csv)|scraping|yes|
|[SO](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_SO_total.csv)|scraping|yes|
|[SZ](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_SZ_total.csv)|scraping|yes|
|[TG](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_TG_total.csv)|scraping|yes|
|[TI](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_TI_total.csv)|scraping|yes|
|[UR](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_UR_total.csv)|scraping|yes|
|[VD](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_VD_total.csv)|scraping|yes|
|[VS](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_VS_total.csv)|scraping|yes|
|[ZG](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_ZG_total.csv)|scraping|yes|
|[ZH](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_total_csv_v2/COVID19_Fallzahlen_Kanton_ZH_total.csv)|scraping|yes|

**Latest updates** <br>
The latest updates are visualized [here](http://www.web.statistik.zh.ch/covid19_dashboard/index.html#/). Note that this images is updated every 20 minutes.

[![Dashboard of data updates](https://github.com/openZH/covid_19/raw/master/dashboard/dashboard.png "Dashboard of data updates")](http://www.web.statistik.zh.ch/covid19_dashboard/index.html) 

## Swiss Cantons and Principality of Liechtenstein: More detailed dataset 

**Data** <br>

>**https://github.com/kalakaru/covid_19/tree/master/fallzahlen_kanton_alter_geschlecht_csv** <br>
>*Description:* Selected cantons publish more detailed datasets.  <br>
>*Spatial unit:* Swiss cantons and Principality of Liechtenstein <br>
>*Format:* csv <br>
>*Additional remark*: Not all datasets are maintained. 

**Maintained datasets** <br>
- See: https://github.com/kalakaru/covid_19/blob/master/README.md#conton-z%C3%BCrich-more-detailed-dataset

**Unmaintained datasets** <br>
- [COVID19_Fallzahlen_Kanton_AG_alter_geschlecht.csv](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Fallzahlen_Kanton_AG_alter_geschlecht.csv)

- [COVID19_Fallzahlen_Kanton_AI_alter_geschlecht.csv](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Fallzahlen_Kanton_AI_alter_geschlecht.csv)

- [COVID19_Fallzahlen_Kanton_AR_alter_geschlecht.csv](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Fallzahlen_Kanton_AR_alter_geschlecht.csv)

- [COVID19_Fallzahlen_Kanton_BS_alter_geschlecht.csv](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Fallzahlen_Kanton_BS_alter_geschlecht.csv)

- [COVID19_Fallzahlen_Kanton_ZH_alter_geschlecht.csv](https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Fallzahlen_Kanton_ZH_alter_geschlecht.csv)

**Metadata for unmaintained datasets** <br>

| __Field Name__          | __Description__                                | __Format__     |__Reporting Cantons__|
|---------------------|--------------------------------------------|------------|--|
| __Date__              | __ZH__ = Date of test result (NewConfCases) / Date of death (NewDeaths) </br> __BL__ = Date of death </br> __BS__ = Date of notification | YYYY-MM-DD | |
| __Area__               | Abbreviation of the reporting canton|     | |
| __AgeYear__ |      | Number   |ZH,BS,BL |
| __Gender__     |  | Text    |ZH,BS,BL   |
| __NewConfCases__       | Number of Confirmed Cases | Number     | ZH  |
| __NewDeaths__       | Number of Deceased  | Number     | ZH,BS,BL  |
| __PreExistingCond__       | Pre-Existing Conditions | Text    | BL,BS |


## Conton Zürich:  Unified dataset

See: 
- https://github.com/kalakaru/covid_19/blob/master/README.md#swiss-cantons-and-principality-of-liechtenstein-unified-dataset 
- [open data swiss: COVID_19 Fallzahlen Kanton Zürich Total](https://opendata.swiss/de/dataset/covid_19-fallzahlen-kanton-zuerich/resource/3cc22355-dedd-461a-99dc-bb6de26db5a4)

## Conton Zürich: More detailed dataset 

**Data** <br>

>**https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Fallzahlen_Kanton_ZH_altersklassen_geschlecht.csv** <br>
>*Description:* [open data swiss: COVID_19 Verteilung der Fälle im Kanton Zürich nach Altersklasse, Geschlecht und Kalenderwoche](https://opendata.swiss/de/dataset>/covid_19-fallzahlen-kanton-zuerich/resource/fbf8fab6-1a9b-496d-9272-f398fb3a74ba) <br>
>*Spatial unit:* Conton Zürich <br>
>*Format:* csv <br>
>*Additional remark*: Comparable data for the canton of Thurgau is published at [opendata.swiss](https://opendata.swiss/de/dataset/covid_19-fallzahlen-kanton-thurgau).


**Metadata**

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __Week__  | Kalenderwoche des Befundes (NewConfCases) / Todesdatums (NewDeaths) | Calendar week of test result (NewConfCases) / Date of death (NewDeaths) |Zahl|
| __Year__  | Jahr des Befundes (NewConfCases) / Todesdatums (NewDeaths) | Year of test result (NewConfCases) / Date of death (NewDeaths) |Zahl|
| __Area__               | Kanton |   Abbreviation of the reporting canton   | Text|
| __AgeYearCat__ | 10-Jahres Altersklassen     | Age groups (10 year steps)   | Text |
| __Gender__     |Geschlecht  | Gender    |  Text|
| __NewConfCases__      | Neue bestätigte Fälle | Newly confirmed number of cases| Zahl   |  
| __NewDeaths__          | Neue Todesfälle | Newly confirmed number of deaths| Zahl     | 

**Data** <br>

>**https://github.com/openZH/covid_19/blob/master/fallzahlen_kanton_alter_geschlecht_csv/COVID19_Einwohner_Kanton_ZH_altersklassen_geschlecht.csv** <br>
>*Description:* Inhabitants per age category and gender. <br>
>*Spatial unit:* Conton Zürich <br>
>*Format:* csv <br>

**Metadata**

| Spaltenname / Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __Year__  | Stichtag ist jeweils der 31.12 des angegebenen  Jahres| The reporting date is the 31.12 of the indicated year |Zahl|
| __Area__               | Kanton |   Abbreviation of the reporting canton  | Text|
| __AgeYearCat__ | 10-Jahres Altersklassen     | Age groups (10 year steps) | Text |
| __Gender__  |Geschlecht  | Gender    |  Text|
| __Inhabitants__  | Anzahl Einwohner  |Number of inhabitants | Zahl |  

## Conton Zürich: Postal codes (Postleitzahl)

**Data** <br>

>**https://github.com/kalakaru/covid_19/blob/master/fallzahlen_plz/fallzahlen_kanton_ZH_plz.csv** <br>
>*Description:* [opendata.swiss: COVID_19 Fallzahlen Kanton Zürich nach Bezirk und Kalenderwoche](https://opendata.swiss/de/dataset/covid_19-fallzahlen-kanton-zuerich/resource/624eb0eb-d439-488b-bbde-1ca58ee62df4) <br>
>*Spatial unit:* Conton Zürich <br>
>*Format:* csv <br>
>*Additional remark*: <br>

**Metadata**

| Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __PLZ__ | Postleitzahl* |Postalcode* |Zahl|
| __Date__  | Datum des Befundes | Date of test result (NewConfCases)  |Zahl|
| __Population__| Einwohner mit Hauptwohnsitz | Inhabitants with main residency| Zahl   |  
| __NewConfCases_7days__ | Neue bestätigte Fälle in den letzten sieben Tagen (Kategorien) | Newly confirmed cases (Categories)| Text     | 

**Geodata** <br>

>**https://github.com/kalakaru/covid_19/blob/master/fallzahlen_plz/PLZ_gen_epsg4326_F_KTZH_2020.json** <br>

>**https://github.com/kalakaru/covid_19/blob/master/fallzahlen_plz/PLZ_gen_epsg2056_F_KTZH_2020.json**


## Conton Zürich: Districts (Bezirk)

**Data** <br>

>**https://github.com/kalakaru/covid_19/blob/master/fallzahlen_bezirke/fallzahlen_kanton_ZH_bezirk.csv** <br>
>*Description:* [opendata.swiss: COVID_19 Verteilung der Fälle im Kanton Zürich nach Postleitzahl](https://opendata.swiss/de/dataset/covid_19-fallzahlen-kanton-zuerich/resource/6129ae60-bd22-4809-a18b-55875352ee76) <br>
>*Spatial unit:* Conton Zürich <br>
>*Format:* csv <br>


**Metadata**

| Fieldname      | Beschreibung (DE)                               | Description (EN)   | Format |
|---------------------|--------------------------------------------|------------|------|
| __DistrictId__ |Bezirks-ID (BFS-Nummer)* |District (BFS-Id)* |Zahl|
| __District__ | Bezirksname*|  District name*   | Text |
| __Population__ | Wohnbevölkerung | Population |Zahl|
| __Week__  | Kalenderwoche des Befundes (NewConfCases) / Todesdatums (NewDeaths) | Calendar week of test result (NewConfCases) / Date of death (NewDeaths) |Zahl|
| __Year__  | Jahr des Befundes (NewConfCases) / Todesdatums (NewDeaths) | Year of test result (NewConfCases) / Date of death (NewDeaths) |Zahl|
| __NewConfCases__ |Neue bestätigte Fälle | Newly confirmed number of cases| Zahl|  
| __NewDeaths__| Neue Todesfälle | Newly confirmed number of deaths| Zahl| 
| __TotalConfCases__ |Total der bestätigten Fälle (kumuliert) | Total of confirmed cases (cumulated) | Zahl|  
| __TotalDeaths__|Total der Todesfälle (kumuliert) | Total of confirmed deaths (cumulated) | Zahl| 

**Geodata**

>**https://github.com/kalakaru/covid_19/blob/master/fallzahlen_bezirke/BezirkeAlleSee_gen_epsg4326_F_KTZH_2020.json** <br>

>**https://github.com/kalakaru/covid_19/blob/master/fallzahlen_bezirke/BezirkeAlleSee_gen_epsg2056_F_KTZH_2020.json**

# Community Contributions

### Visualization of Swiss and Cantonal Case Numbers over Time
- https://rsalzer.github.io/COVID_19_CH/
- https://rsalzer.github.io/COVID_19_KT_ZH/ 
<br>Robert Salzer on Twitter: https://twitter.com/rob_salzer

### ArcGIS Dashboard
- https://covid19.ddrobotec.com/ 
[github-repo](https://github.com/zdavatz/covid19_ch) 
<br>Zeno Davatz on Twitter: https://twitter.com/zdavatz

### corona-data.ch
- https://www.corona-data.ch/ 
[github-repo](https://github.com/daenuprobst/covid19-cases-switzerland) 
<br>Daniel Probst on Twitter: https://twitter.com/skepteis?lang=de

### Interactive Small Multiples of Case Numbers by Canton
- https://sars-cov-2-switzerland.netlify.com/

### REST-API
- [https://covid19-rest.herokuapp.com](https://covid19-rest.herokuapp.com)
- [github-repo](https://github.com/apfeuti/covid19-rest) <br>Andreas Pfeuti

### Estimated reproduction number by Canton
- https://amkuhn.shinyapps.io/restimate/
 <br>Alexandre Kuhn

### Data for Basel-Stadt
- https://data.bs.ch/pages/covid-19-dashboard/<br>Open Government Data Basel-Stadt on Twitter: https://twitter.com/OpenDataBS

### COVID-19 Data Hub
- https://covid19datahub.io
- https://github.com/covid19datahub/COVID19/

Many thanks for the great work!
