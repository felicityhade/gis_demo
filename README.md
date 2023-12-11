# Providence Crime Dataset

## Introduction

The Providence Crime Dataset is a geodataset created by the Brown University Library [GeoData@SciLi](https://libguides.brown.edu/geodata/) team for the analysis of crimes by location and type through time. It is derived from the [Providence Police Case Log](https://data.providenceri.gov/Public-Safety/Providence-Police-Case-Log-Past-180-days/rz3y-pz8v/about_data), updated nightly with the past 180 days of crime incidents in Providence. Longitude and latitude coordinates were derived from three sources: RIGIS's E911 landmark point layer, the RIDOT geocoder, and ______ (wherever the landmark locations come from). The coordinate source is determined by the format of the location attribute in the original dataset: block number, intersection, or landmark. Locations which do not fall into these categories, including standalone street names, were not geocoded due to their imprecise nature. Successfully geocoded results are stored as a point layer ([shapefile name]) in the Rhode Island State Plane (ft-US) coordinate system, EPSG 3438. Results are also available in Excel format ([excel file name]), with 'latitude' and 'longitude' columns in WGS 84. Cases which could not be accurately geocoded are stored in ([excel file name]). Cases are stored in separate files by year. In addition to these output files, this repository includes metadata in the OSM Aardvark standard, documentation, and Python scripts for generating the results.

Note that coordinates in the output files are inexact, particularly for crimes associated with block-level locations in the original datasets. These locations do not represent the precise location where the incident occured.

## Rights and Use

The dataset and associated documentation are licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/) CC BY-NC-SA ![CC BY-NC-SA](/images/cc_license.png). You are free to share and to adapt the work as long as you cite the source, do not use it for commercial purposes, and release adaptations under the same license.

*Disclaimer: Every effort was made to insure that the data, which was compiled from public sources, was processed and presented accurately. The creators and Brown University disclaim any liability for errors, inaccuracies, or omissions that may be contained therein or for any damages that may arise from the foregoing. Users should independently verify the accuracy and fitness of the data for their purposes.*

## Downloads

<u>CURRENT VERSION</u>: geodata_pvdcrime_2023_12

TODO: REPLACE THIS SECTION

- [OSSDB SQLite](https://github.com/Brown-University-Library/geodata_ossdb/raw/main/current_db/ossdb_sqlite.zip): the primary database, a SQLite / Spatialite database that can be used in desktop GIS packages such as QGIS and ArcGIS Pro, and SQL database tools like the QGIS DB Manager, Spatialite GUI, and DB Browser for SQLite

- [OSSDB File Geodatabase](https://github.com/Brown-University-Library/geodata_ossdb/raw/main/current_db/ossdb_esri_gdb.zip): a copy of the database in the ESRI File Geodatabase format, which can be edited in ArcGIS Pro (the Spatialite format in ArcGIS Pro is read only)

- [Summary](https://raw.githubusercontent.com/Brown-University-Library/geodata_ossdb/main/current_db/bul_ossdb_summary.pdf): a two-page summary of the database with instructions on how to connect to it in QGIS and ArcGIS Pro (included with the database download)

- [Documentation](https://raw.githubusercontent.com/Brown-University-Library/geodata_ossdb/main/current_db/bul_ossdb_guide.pdf): in-depth documentation that describes database updates, contents, structure, and instructions for accessing via GIS and database software (included with the database download)

- [Metadata](https://github.com/Brown-University-Library/geodata_ossdb/tree/main/current_db/metadata): one record for each feature and table in the database; click on the markdown (.md) copy for a readable version (included with the database download)

## Features

| column    | description                                                                                                  |
| --------- | ------------------------------------------------------------------------------------------------------------ |
| casenumber | Case number assigned by Providence Police records management system  |
| location  | Street Number and Street Name or nearest intersection of reported incident.
A street number does not always indicate the incident took place on the property. |
| reported_date  | Date and Time reported to Providence Police.
When a crime is reported does not always indicate when it took place  |
| month | ...                              |
| year  | ... |
| offense_desc     | ...                                                |
| statute_code  | a four-letter code corresponding to a particular retail price category (see below for full list)             |
| statute_desc     | the full name of the retail price category                                                                   |
| counts    | US Dollar nominal monthly expenditure by an average UN staff member                                          |
| reporting_officer     | numerical Post Adjustment Index value                                                                        |
| unique_id | |
| latitude* | Approximate latitude in WGS 84 |
| longitude* | Approximate longitude in WGS 84 |
| source* | Source of the generated coordinates |
| violent_cat | Category of violent crime |
| property_cat | Category of property crime | 
| ------- | ------ |

*Only present for successfully geocoded results


