---
layout: default
title: Before You Start
nav_order: 2
nav_exclude: true
has_toc: false
---

# BEFORE YOU START 

Do you have a dataset that you'd like to publish through the [_DataBC Program_](https://data.gov.bc.ca/)? Before your data is published, we will need to gather some information from you. The questions on this page will help the [DataBC Data Architecture Services](faq.md#data-architecture-services) team learn about your requirements and to determine whether the DataBC Program can meet them.

|**AUDIENCE**|
|:---:|
| *Data Publishers* | 

## Table of Contents
+ [**DATA PUBLICATION CHANNELS**](#data-publication-channels)
+ [**QUESTIONS**](#questions)
	+ [Questions about the Data](#questions-about-the-data)
	+ [Custodianship Considerations](#custodianship-considerations)
	+ [Relationship to Legislation](#relationship-to-legislation)
	+ [Audience Considerations](#audience-considerations)
	+ [Dataset Readiness](#dataset-readiness)
	+ [Financial Obligations](#financial-obligations)
+ [**NEXT STEPS**](#next-steps)

-----------------------

## DATA PUBLICATION CHANNELS

The DataBC Program makes data available through combinations of several different channels:

+ the [_BC Geographic Warehouse_](https://www2.gov.bc.ca/gov/content?id=18B291A12B4F42EA98169892F4B46D61)
+ the [_BC Data Catalogue_](https://catalogue.data.gov.bc.ca)
+ [_iMapBC_](https://www2.gov.bc.ca/gov/content?id=C52F8C3BFE8C4110A63171337F363F43)
+ [_BC Map Services (WMS and WFS)_](https://www2.gov.bc.ca/gov/content?id=95D78D544B244F34B89223EF069DF74E)
+ [_BC Map Hub_](https://www2.gov.bc.ca/gov/content?id=DE0602BB42664AA28C9F059D45CC1CC2)
+ [_Data Distribution Services_](https://www2.gov.bc.ca/gov/content?id=B19E16070B824DB481F49CEE3B9AF1F8) through the BC Data Catalogue, iMapBC and (___coming soon___) the Order Fulfiller Interface (OFI) Application Programming Interface (API)

In addition, other agencies provide mechanisms for accessing DataBC data:

+ the Geographic Terminal Servers (GTS - available through [dts.gov.bc.ca](https://dts.gov.bc.ca))
+ [_BCData R package_](https://github.com/bcgov/bcdata)

There are five options for where data gets stored in the DataBC Program, each with its own benefits and drawbacks:

| | BC Geographic Warehouse | BC Data Catalogue | BC MapHub | pub.data.gov.bc.ca | External site |
|:---|:---:|:---:|:---:|:---:|:---:|
**Security** - Public | ![](/images/green_check.png) | ![](/images/green_check.png)  | ![](/images/green_check.png) <br /> through the public publication request form | ![](/images/green_check.png)  | ![](/images/green_check.png) |
**Security** - IDIR	| ![](/images/green_check.png) <br /> for metadata only | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Security** - Named Users | ![](/images/grey_dash.png) | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Security** - Role-based | ![](/images/grey_dash.png) | ![](/images/green_check.png) <br /> in comination with Public, IDIR, Named Users | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Security** - BCeID | ![](/images/grey_dash.png) | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Format** | BCGW dataset (Oracle object), ArcGIS Rest, atom, cded, cvs, e00, fgdb, geojson, georss, gft, html, json, kml, kmz, openapi-json, pdf, rdf, shp, tsv, txt, wms, wmts, xls, xlsx, xml, zip, other | Oracle object (spatial and non-spatial) | WMS, WFS, Shapefile, CSV, TXT, GPX, GeoJSON | Any | Any
**File Size** | < 150 mb | datasets configured for distribution: < 2 GB zipped | < 500 mb | > 150 mb | Any
**Download** - entire dataset | ![](/images/green_check.png) | ![](/images/green_check.png) | ![](/images/green_check.png) <br /> for BCGW datasets: re-directed to the BC Data Catalogue <br /> for standalone datasets: direct download | ![](/images/green_check.png) | ![](/images/green_check.png)
**Download** - subset dataset | ![](/images/grey_dash.png) | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Spatial data** - view in iMap BC | ![](/images/grey_dash.png) | ![](/images/green_check.png) | ![](/images/grey_na.png) | ![](/images/grey_na.png) | ![](/images/grey_na.png)	
**Spatial data** - view in desktop mapping applications (i.e. ArcGIS, QGIS) | ![](/images/green_check.png) <br /> once downloaded | ![](/images/green_check.png) | ![](/images/green_check.png) <br/> can open data in ArcGIS via BC MapHub | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Spatial data** - view WMS (Web-Map Service) | ![](/images/green_check.png) <br /> once downloaded | ![](/images/green_check.png) | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Spatial data** - view WFS (Web Feature Service) | ![](/images/green_check.png) <br /> once downloaded | ![](/images/green_check.png) | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Spatial data** - view in BC MapHub | ![](/images/grey_dash.png) | ![](/images/green_check.png) | ![](/images/green_check.png) | ![](/images/grey_dash.png) | ![](/images/grey_dash.png)
**Non-spatial data (csv)** - view preview | ![](/images/green_check.png) | ![](/images/grey_na.png) | ![](/images/grey_na.png) | ![](/images/grey_na.png) | ![](/images/grey_na.png)
**Non-spatial data (csv)** - view point data on a map | ![](/images/green_check.png) | ![](/images/grey_na.png) | ![](/images/green_check.png) | ![](/images/grey_na.png) | ![](/images/grey_na.png)

[RETURN TO TOP][1]

-----------------------------------------

## QUESTIONS

In order to help us determine how your data best fits into these options and services, please take a moment to answer the following questions (copy and paste into an email or word doc), and send your responses, or questions/concerns to the [DataBC Data Architecture Services](faq.md#data-architecture-services) team.

### Questions about the Data

+ Provide a short description of the dataset(s).
+ Does the data already exist in the DataBC Program? (e.g., the BC Geographic Warehouse, the BC Data Catalogue, etc.)
   + If these are replacement dataset(s), what are the dataset(s) to retire?
+ Does this data belong with any other groupings of data in the BC Geographic Warehouse?
+ Is the data provincial in extent? This doesn't mean that the dataset necessarily contains data for all parts of the province.  It just means that if there were data for some other part of the province then it would be included in the dataset.
   + If not provincial in extent now, is there an intent to make the dataset provincial in extent in the future?

#### Dataset Complexity

+ How many datasets (please indicate if point, line, polygon, or non-spatial) and approximately how many attribute field columns are there in each dataset? 
+ What is the size of each dataset (approx. how many features/records?)
+ What is its intended growth (e.g., it will grow 10% over the next year and 1% after?)
+ How frequently is the data to be updated? (nightly, weekly, monthly, annually, ad-hoc)
+ What is the file format and where is the source data currently stored? 
   + Is it in database or a file store?

-----------------------------------------

### Custodianship Considerations

+ Has this dataset been created by the Province of British Columbia?
   + If no, is your business area the authorized [_Data Steward_](dsg_bcdc_roles_responsibilities.md#the-data-steward)?
   		+ For example, BCStats acts as the authorized _Data Steward_ for data collected and disseminated by Statistics Canada.
+ Do you have Director level approval? 
   + Your Director will be the _Data Custodian_, and ultimately accountable for the dataset.
   + Refer to [_What is a Data Custodian_](dsg_bcdc_roles_responsibilities.md#what-is-a-data-custodian) for further details.
+ Is there a program (staff and resources) in place to ensure this data kept up-to-date? Are there identified staff managing the data, i.e., Data Manager?
   + Refer to [_What it means to be a Data Manager_](dsg_bcdc_roles_responsibilities.md#what-it-means-to-be-a-data-manager) for further details.

-----------------------------------------

### Relationship to Legislation

+ Is this dataset associated with legislation or policy? In other words, is the dataset:
   + required by legislation or policy? (e.g., to provide public access)
   + necessary to assist staff in carrying out tasks required by legislation or policy?

-----------------------------------------

### Audience Considerations

+ Who is the intended audience? Public, BC Government, People with a Business BCeID, Individual specific people. 
   + If the audience is the public, is the intention to make the data under the [_BC Open Government Licence_](https://www2.gov.bc.ca/gov/content?id=A519A56BC2BF44E4A008B33FCF527F61)?  
+ Are there existing or new applications that will use this data?    
+ What tools (visualize or otherwise) will be used to access the data?
   + [BC Data Catalogue](https://catalogue.data.gov.bc.ca)
   + [iMapBC](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/web-based-mapping/imapbc) 
   + [Web-mapping Frameworks](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/bc-spatial-data-infrastructure/webmapping)
   		+ [BC's Map Hub (ArcGIS Online)](https://www2.gov.bc.ca/gov/content?id=DE0602BB42664AA28C9F059D45CC1CC2) 
   + [Data Distribution Services (Downloads)](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/data-distribution-services)
   + Direct Connect for internal government GIS users (e.g., ArcGIS/ArcMap, SQL Developer) 
   + Outside DataBC tools/application (existing applications or potentially a new application)

[RETURN TO TOP][1]

-----------------------------------------

### Dataset Readiness

To find out if your data is ready for the BCGW, see [Workflow - Is my data ready for the BCGW?](dps_bcgw_w.md#workflow---is-my-data-ready-for-the-bcgw)

-----------------------------------------

### Financial Obligations

DataBC operates on a cost-recovery basis, so there _may_ be a charge to your branch for making your data available through the DataBC program. 

This one-time charge covers not only the initial loading of the dataset, but also the ongoing maintenance and refreshing of the data.

Whether or not there is a charge depends on how the data is to be made available and on the size of the potential audience.  

These are some rough guidelines:
+ Depending on DataBC resources, datasets that are considered foundational (of use to many different business areas) might be loaded at no charge.
+ Data to be made available solely within the BC Data Catalogue (i.e., not stored in the BC Geographic Warehouse) will be loaded at no charge. 

If there is a charge it will generally be between $1500 and $7000, depending on:

+ the number of datasets
+ the complexity (number of columns) of the datasets
+ the security requirements (e.g., public vs access by only named individuals)
+ the access channels to be used (e.g., iMapBC, data download, etc.)

In certain circumstances there may be additional charges for the following:

+ the dataset is extremely large (several million rows or larger)
+ the load requires extensive manipulation and transformation of the input data
+ we need to be heavily involved in operational planning (planning preparation of the data set)  
+ the data source is nonstandard
   + Standard sources are:
         + Oracle operational BC Government databases, 
	   + csv files, 
	   + shape files, 
	   + file geodatabases, 
	   + text files, 
	   + rest APIs.

The amount of the charge will be discussed at the [_Discovery Whiteboard_](dps_bcgw_w.md#discovery-whiteboard), held at the beginning of the publication process.

Changes to the structure of the dataset after the initial load may incur additional charges. Examples of changes are addition and removal of columns, changes in column names, etc. If you envision many changes over time or the addition of new datasets or continuing support in preparing data you may wish to enter into a support agreement with DataBC, which can also be discussed at the Discovery Whiteboard.

-----------------------------------------

## NEXT STEPS

Please send answers to the questions above to the [DataBC Data Architecture Services](faq.md#data-architecture-services) team. 

In addition, the following resources will help to answer any questions you may have on the publication process:

+ BC Geographic Warehouse > [_Publication Workflow_](dps_bcgw_w.md): a step by step guide to the data onboarding process for data to be loaded into the BC Geographic Warehouse.
+ [_Frequently Asked Questions_](faq.md)
+ [_DataBC Program Key Contacts_](faq.md#WHOS-WHO-AT-DATABC)

-----------------------------------------

[RETURN TO TOP][1]

[1]: #before-you-start
