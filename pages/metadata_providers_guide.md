# PUBLISHING METADATA AND DATA TO THE BC DATA CATALOGUE

This document provides a set of standards, guidelines, and procedures around loading and maintaining data to be served by the DataBC Program's access channels, which are:
+ [_The BC Geographic Warehouse (BCGW)_](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/bc-spatial-data-infrastructure/bc-geographic-warehouse)
   + [_iMapBC_](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/web-based-mapping/imapbc)
   + [_Data Download Services_](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/data-distribution-services)
+ [_The BC Data Catalogue (BCDC)_](https://catalogue.data.gov.bc.ca)
+ [_Web Map and Feature Services (WMS/WFS)_](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/web-based-mapping/map-services)
+ [_BC Map Hub (ArcGIS Online)_](https://www2.gov.bc.ca/gov/content/data/geographic-data-services/web-based-mapping/agol)

-----------------------
## Table of Contents
+ 	[**HOW TO BECOME A PROVIDER**](#how-to-become-a-provider)
+   [**HOW TO REQUEST A GROUP**]()
+   [**WHICH LICENCE TO USE**](#which-licence-to-use)
+   [**HOW TO CREATE A NEW METADATA RECORD**](#how-to-create-record)
+   [**HOW TO EDIT A METADATA RECORD**](how-to-edit-record)
+   [**HOW TO MANAGE METADATA RECORD RESOURCES**](#how-to-manage-record-resources)
+   [**HOW TO PUBLISH A METADATA RECORD**](#how-to-publish-record)
+   [**HOW TO PUBLISH UNDER THE BC OPEN DATA LICENCE**]()
+   [**HOW TO ARCHIVE A METADATA RECORD**]()
+   [**FREQUENTLY ASKED QUESTIONS**]()

-----------------------

# Audience

This document is meant for people who want to make metadata and data available through the BC Data Catalogue (BCDC), which is part of the DataBC Program. It does not contain any DataBC Program internal operational information.

For recommendations on how to publish your data, please refer to the [Before you start](pages/before_you_start.md#before-you-start) and the [_Frequently Asked Questions_](pages/faq.md#frequently-asked-questions-faq) pages. 

Feel free to contact the [DataBC Data Architecture Services](mailto:databc.da@gov.bc.ca) team.

# Purpose

The contents of this space are provided as a set of 
  
-----------------------------------------------------------

## How to become a provider

## How to become a provider as a steward for another organization

## How to request a group

## How to get an organization added or renamed

## Which licence to use

### Access Only
_Access only_ is the standard and is [restrictive](https://www2.gov.bc.ca/gov/content/home/copyright). 

### Open Government Licence - British Columbia

Whenever possible we recommend data be published under an Open Government Licence which is much more permissive.

+ 	[Open Information and Open Data Policy](https://www2.gov.bc.ca/assets/gov/british-columbians-our-governments/services-policies-for-government/information-management-technology/information-privacy/resources/policies-guidelines/open-information-open-data-policy.pdf)

+ 	[Open Data Licence - British Columbia (OGL-BC)](https://www2.gov.bc.ca/gov/content?id=A519A56BC2BF44E4A008B33FCF527F61)
    
+ 	[Open Data - Physical Datasets](https://www2.gov.bc.ca/assets/gov/government/services-for-government-and-broader-public-sector/information-technology-services/standards-files/open_data_physical_dataset_extract.pdf) is a list of open format file. This document is slated for update as there are other modern open formats.

+ 	[Open Data Assessment and Checklist](https://www2.gov.bc.ca/assets/gov/data/open-data/open_data_assessment_and_checklist.docx)

To publish something under OGL-BC you will need to contact multiple people for authorization. Names of who to contact and other resources are included in the [Open Data Assessment and Checklist](https://www2.gov.bc.ca/assets/gov/data/open-data/open_data_assessment_and_checklist.docx) document.

+ The [Ministry Information Security Officer (MISO)](https://intranet.gov.bc.ca/intranet/content?id=DC4623F6F1944065B83F70297ED419D7)

+ The [Intellectual Properties Office](https://www2.gov.bc.ca/gov/content?id=4F03158C0AF84EC08DBB5BE3E873C33E) - email [QPIPPCopyright@gov.bc.ca](mailto:QPIPPCopyright@gov.bc.ca)

+ Sign off from the Custodial organization's Deputy Minister or designated alternate is required.

Once these approvals are in place, Data can be published under OGL-BC if:

+ it is in an open format, e.g., CSV, Shape File (SHP), JSON, or additional formats noted by the OCIO's [Open Data Physical Dataset Format Standard](https://www2.gov.bc.ca/assets/gov/government/services-for-government-and-broader-public-sector/information-technology-services/standards-files/open_data_physical_dataset_extract.pdf). 

+ The BC Data Catalogue record links to the appropriate Open Data Licence.


### Other Open Government Licences

### Creating an Open Government Licence

The Broader Publish Sector (BPS) is not permitted to use the OGL-BC and thus must create their own. These steps are what is suggested:

1. Copy our Open Government Licence - British Columbia, as it is consistent with the Feds and other Local Governments
	+ examples, BC Assessment and Elections BC
1. Modify the identified text to personalize it for your org
	1. Licence Name – change ‘Open Government License – British Columbia’ to ‘Open Government License – BC Oil and Gas Commission’
		+ This name should be the same that is found on the BC List of Agencies, Crown Corps, etc
	1. Change line: ‘Contains information licensed under the Open Government Licence – British Columbia.’ to ‘Contains information licensed under the Open Government Licence – BC Oil and Gas Commission’
	1. Information Provider – change ‘means Her Majesty the Queen in right of the Province of British Columbia.’ to ‘means BC Oil and Gas Commission’
	1. Versioning – change ‘This is version 2.0 of the Open Government Licence for Government of British Columbia Information’ to ‘This is version 1.0 of the Open Government Licence for BC Oil and Gas Commission Information’
	1. Remove: ‘Note’ line re: copyright can be removed
1. Publish the OGL to a public site so that it can add it to the drop down list of licence options.

## How to create a new metadata record

1.   Log into the [BC Data Catalogue](https://catalogue.data.gov.bc.ca/dataset) with the *Log in* button the upper right.
	+ This will take you to your dashboard that may or may be useful for you.
1.   Click on the *Datasets* button on the toolbar or navigate to [Datasets](https://catalogue.data.gov.bc.ca/dataset) page. 
1. 	Click the [Add Dataset](https://catalogue.data.gov.bc.ca/dataset/add) button.
1.   Choose a dataset type from one of the four types available that best fits your data, service or application.

	|Dataset Type|Description|Requirements|
	|:---|:---|:---:|
	|Dataset| These are tables in Comma Separated Value (CSV) files, or MS Excel Spreadsheets (XLS) or possibly even tabular PDF files.| |
	|Geographic Dataset|This is data that contains geospatial information along with other data.  Additional geospatial metadata elements are available to be populated, e.g., spatial reference system.|Must be used for all BCGW Datasets|
	|Application Dataset|Metadata records in this category describe applications that are available for use.  Applications provide access to data.| |
	|Web Service - API|Metadata records in this category describe available web services, or application programming interfaces.| |

1.  Click the *Create Dataset* button.
1.	Fill in all [manditory fields](https://github.com/pumapants/data-standards/blob/master/pages/metadata_standards.md#MANDATORY-METADATA-FOR-THE-BC-DATA-CATALOGUE) and highly suggest filling in all non manditory fields as well to assist the users to understand and use the data better. Mandatory fields are marked with an *.
1.   After filling in the details in the **Create dataset** tab, click **Next: Add Data** to save your changes.

_**Dataset**_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**State**|DRAFT|This changes the state of the publication workflow.|
|**Title**|should be written in a way the general public can understand|Do not include organization or program names in titles as these may change over time. Unless there is no other way to distiguish a dataset from another of similar title.<br>For records that will include multiple years, do not include the year in the title.|
|**URL**| | Will be auto-populated based on the title.<br>If the title includes a parenthasis at the end then recommend removing this from the URL.|
|**Organization**|Ministry of Citizen Services|Required|
|**Sub-Organization**|DataBC|Required|
|**Description**|_detailed description about the data_|If there is a accronym, always spell out the name in full and then include the accronym in parentases|
|**Purpose**|_summary of the intentions for which the dataset was developed_|Include more information about a record will aid users and allow for more self serve of information.|
|**Data Quality**|_descriptive text that can include info about issues, completeness, consistency, etc._|Include more information about a record will aid users and allow for more self serve of information.|
|**Lineage Statement**|_information about the events or source data used in constructing the data_|Include more information about a record will aid users and allow for more self serve of information.|
|**More Info**|_supporting url(s)_|Links should be added to provide more information a user can go to.<br> These should use https:// instead of http://. <br>For pages within the BC Gov webpages, if possible, the permalinks should be used as this allows the pages to move around but the links will not become broken.<br>At the bottom right is a gray icon with an arrow pointing to the right.<br>Click this and then hit the **Copy** button.|
|**Keywords**|_searchable term(s)_|Are important words related to a dataset and can include common words, phrases or accronyms.|
|**ISO Topic Category**|boundaries|[For more information](https://www2.usgs.gov/science/about/thesaurus-full.php?thcode=15)|

_**Contact**_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**Name**|_contact's first and last name_|This may a name for a generic inbox.|
|**Email**|_someone@somewhere.ca_|This may be the email of a generic inbox.|
|**Organization**|Ministry of Citizen Services|The organization or ministry the contact is from.|
|**Sub-Organization**|DataBC|The sub-organization, branch or program area the contact is from.|
|**Role**|pointOfContact|Most often this is set to pointOfContact. Custodian is reserved for the Director or a Executive Director of a branch.|
|**Contact Displayed**|Yes|Set to Yes when the contact is to be visisble to the public. No, allows the contact to only be visible when logged in.|

_Data Currency / Update_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**Resource Status**|planned|Describes the state of the data. Choose the most relevant Resource Status and Date Type that best matches the currency of the data.<br> Multiple dates can be added to track the progress of the data.|
|**Data Type**|Created, Published||
|**Date**|_YYYY-MM-DD_||

_**Access & Security**_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**Who can view this data?**|Public|This is intended to be who can view the data in a web application.<br>For data in the BCGW, this refers to the security applied to in iMapBC.<br>If there is a desire to change this security setting contact [Data Architecture Services](mailto:databc.da@gov.bc.ca) as changing it in the metadata record will not apply the change at the application level.|
|**Who can view this record?**|Public|This allows a provider to make a metadata record visible only when logged in, i.e., IDIR.|
|**Who can download this data?**|Public|This is intended to be who can download the data. For data in the BCGW, this refers to the security applied to the Distribution Service.<br>If there is a desire to change this security setting contact [Data Architecture Services](mailto:databc.da@gov.bc.ca) as changing it in the metadata record will not apply the change at the application level.|
|**Who can access this application?**|Public|Required|
|**Licence**|Open Governement Licence - British Columbia|This is very important as it determines [how the data can be used](#which-licence-to-use)|
|**Security Classification**|LOW-PUBLIC|Describes how secure the data is. [See the Security Classification Standard](https://www2.gov.bc.ca/assets/gov/government/services-for-government-and-broader-public-sector/information-technology-services/standards-files/information_security_classification_standard_july_17_2018.pdf)|

_Preview Information_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**Layer name**|Name of the layer for preview|This is autopopulated when a BCGW dataset is made available through publical WMS|
|**Preview latitude**|Latitude of layer for preview|This is autopopulated when a BCGW dataset is made available through publical WMS|
|**Preview longitude**|Longitude of layer for preview|This is autopopulated when a BCGW dataset is made available through publical WMS|
|**Preview map service URL**|URL of map service for preview|This is autopopulated when a BCGW dataset is made available through publical WMS|
|**Preview zoom level**|Zoom level for preview|This is autopopulated when a BCGW dataset is made available through publical WMS|
|**Image URL**|_URL for non map service images| |
|**Link to iMap**| |This link is autopopulated when a BCGW dataset is publically visisble in iMapBC|

_**Geographic extent**_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**North**|60.0|This is the bounding box of the province and autopopulated for Geographic type resources|
|**South**|48.0|This is the bounding box of the province and autopopulated for Geographic type resources.|
|**East**|-113.5|This is the bounding box of the province and autopopulated for Geographic type resources.|
|**West**|-139.5|This is the bounding box of the province and autopopulated for Geographic type resources.|
|**Spatial Datatype**|SDO_GEOMETRY|N/A|

_**Object Description**_
|Data Element|Example(s)|Recommendations|
|:---|:---|:---|
|**Object Name**|_schema.table(view)_|This is use by Services tied to the BCGW|
|**Column Name**||This is use by Services tied to the BCGW|
|**Short Name**| |This is uneditable and autopopulated from metadata in the BCGW|
|**Data Type**| |This is uneditable and autopopulated from metadata in the BCGW|
|**Data Precision**| |This is uneditable and autopopulated from metadata in the BCGW|
|**Comments**| |This is uneditable and autopopulated from metadata in the BCGW|



## How to edit a metadata record

1.   Log into the BC Data Catalogue.
1.   Navigagte to the metadata record to be edited and click the "wrench" tool icon (top right corner) to start editing the record.  The "Edit Metadata" allows for the editing of all content.
1.   After making edits in the **Edit Metadata** tab, click **Update Dataset** to save your changes.

*   To add or manage data resources, see **_[How to manage metadata record data resources](https://www2.gov.bc.ca/gov/content/data/bc-data-catalogue/bc-data-catalogue-about/bc-data-catalogue-user-guide#how-to-manage-record-resources)_**.



## How to manage metadata record resources

*   Log into the BC Data Catalogue.
*   Locate the metadata record to be edited and click the "wrench" tool icon (top right corner) to start editing the record.
*   Select the "Resources" tab.

### Adding a new resource

*   Click the "Add New Resource" button.
*   Upload or provide a link to your data and provide information about the data resource.
    *   **Upload**: To upload a file, e.g., CSV, directly into the Catalogue, click the **Upload** button and select the file to upload from your local computer.
    *   **Link**: To link to a file stored elsewhere, e.g., a website or FTP site, click **Link **and enter the URL of the file.
	
*	For BC Geographic Warehouse datasets (spatial or none)
1. Click on

**Note: Only files less than 150MB in size can be uploaded to the Catalogue.**

**Note: If the file is less than 150MB limit we recommend uploading the file to the Catalogue vs. storing the data elsewhere. **

*   Complete the resource metadata.  Mandatory fields are marked with an *.
*   Additional resources can be added by clicking **Add** and repeating the process above.

### Editing the properties of an existing resource

*   Click the **Manage** button to edit the resource.
*   Make edits.
*   Click **Update Resource** to save your changes.

### Replacing an existing resource

*   Click the **Manage** button to edit the resource.
*   Click on the **Remove** button at the end of the **File** URL.
*   Re-upload or provide a new link to your data.
*   Click **Update Resource** to save your changes.

### Deleting an existing resource

*   Click the **Manage** button to edit the resource. 
*   Scroll to the bottom of the page and click **Delete** to remove the resource.


## How to publish a metadata record 

Metadata records have a life cycle from Draft to Pending Publish to Published to Pending Archive to Archived.

*   Log into the Catalogue.
*   Locate the metadata record to be edited and click the "wrench" tool icon (top right corner) to start editing the record.
*   Change the dataset record state to **Pending Publish**.
*   Click **Update Dataset**.
	+ This will then send an email to the Catalogue team that you are ready to publish the record.
	
Publicaiton timing: if there is a specific time and date that the release of these records is required contact the Catalogue team to work on timing that is withing regular government business hours.

The Catalogue team will validate the record and if all is in order will change the state to **Published** and you will be notified of this by email; or a Catalogue team member may contact you with questions about your record.