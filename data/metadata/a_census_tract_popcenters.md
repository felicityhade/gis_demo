---
# TITLE
dct_title_s: Providence Crime, Rhode Island, 2023-

# DESCRIPTION
dct_description_sm:
- This is a point layer of crime incidents in Providence. This layer was created from the Providence Police Department's Case Log, which is updated nightly with the most recent 180 days of data. Each incident is assigned a unique case number; multiple offenses may be associated with same incident/case number and are stored as separate datapoints. Each offense has a 'counts' attribute which indicates the number of instances of that offense. Crime locations are geocoded according to the location type. Intersections are geocoded using the RIDOT geocoder. Block locations are geocoded using the E911 point layer provided by RIGIS. Landmark coordinates are derived from a manually generated points-of-interest file. Coordinates from these sources are converted to the Rhode Island State Plane Zone. Locations which do not fall into the aforementioned categories (e.g. street names) and locations which could not be geocoded are ommited from this dataset and stored in a separate file. Offenses are uniquely identifiable by the 'unique_id' attribute, which is an extension of the associated case number. Offenses are also categorized by type: 'violent_cat' indicates the classification of violent crime, and 'property_cat' indicates the classification of property crime if applicable. Offenses are categorized using the 'offense_desc' (offense description) attribute according to the FBI's guidelines. This layer was created by the Brown University Library.
- More information regarding the Providence Police Department's original dataset can be found [here](https://data.providenceri.gov/Public-Safety/PPD-Arrest-and-Case-Logs-FAQ/4t25-ekcs/about_data).

# LANGUAGE
dct_language_sm:
- eng

# CREATOR
dct_creator_sm:
- Brown University Library

# PUBLISHER
dct_publisher_sm:
- Providence Police Department

# PROVIDER
schema_provider_s: Brown

# RESOURCE CLASS
gbl_resourceClass_sm: 
- Datasets

# RESOURCE TYPE
gbl_resourceType_sm:
- Point data

# LC SUBJECT
dct_subject_sm:
- Crime

# ISO THEME
dcat_theme_sm:
- Events
- Society

# TEMPORAL
dct_temporal_sm:
- '2023 - 2024'

# DATE ISSUED
dct_issued_s: '2023-12'

# SPATIAL
dct_spatial_sm:
- Providence, Rhode Island, United States

# BOUNDING BOX
TODO: REPLACE WITH FINAL BOX
dcat_bbox: 'ENVELOPE(-71.9073,-71.0886,42.0189,41.0958)'

# RIGHTS
dct_rights_sm: 
- The data are licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. You are free to share and to adapt the work as long as you cite the source, do not use it for commercial purposes, and release adaptations under the same license.
- Disclaimer. Every effort was made to insure that the data, which was compiled from public sources, was processed and presented accurately. The creators and Brown University disclaim any liability for errors, inaccuracies, or omissions that may be contained therein or for any damages that may arise from the foregoing. Users should independently verify the accuracy and fitness of the data for their purposes.

# LICENSE
dct_license_sm:
- https://creativecommons.org/licenses/by-nc-sa/4.0/

# ACCESS RIGHTS
dct_accessRights_s: Public

# FILE FORMAT
dct_format_s: 
- Shapefile
- Tabular data

# UNIQUE ID
TODO: ASK WHAT TO PUT HERE
id: brown-04042023AAI

# IDENTIFIER
dct_identifier_sm:
- https://github.com/Brown-University-Library/geodata_pvdcrime/data

# METADATA MODIFIED
gbl_mdModified_dt: '2023-12-8'

# METADATA VERSION
gbl_mdVersion_s: Aardvark

# GEOREFERENCED
gbl_georeferenced_b: True
