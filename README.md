# power-query-tableau-rest-api-samples

This project will provide various samples for using the Tableau Server Rest API from Power Query in both Power BI and Excel.  The main goal is to provide information to those that support Tableau Server and Content contained in the server with information not accessible via the Server Portal or even Tableau reports.  Unfortunately, ability to access Rest API's in Tableau (Desktop or Server) cannot be done without writing custom Web connectors.  Power Query in Excel or Power BI does not have this limitation. In addition due to its powerful M language power Query can do more than just access Rest API it can process the retrieved content either in various formats such as ZIP files, XML and JSON to name a few.

## Prerequisites
In order to use the provided samples you will need to have either Excel with Power Query abd Power Pivot enbaled or Power BI Desktop. Latest versions would be recommended.

To run these Power Queries successfully you will need a non-SAML account set-up in Tableau Server with the required priveledges.  I built the smaples were built using version 3.0 of the Tableau _Rest API but they should work with minor tweaks with older versions.

## Installing
The samples are self contained Excel XLSX or Power BI PBIX files.  So once you download if you have Excel or Power BI installed you should be good to go.  

You will need to update the 3 parameters in the Power Query Editor.  

* Host - This is URL of your Tableau Server ex.  https://tableau.mydomain.com
* username - User name of the acount you want to use to make Rest calls. 
* password - Password for the account used to make the Rest API calls.

## Notes
The queries are not tuned and are greedy in how they operate.  I have maxed out the page setting to the max per site of 1000.  So if you have alot of content the queried may need to be adjusted to page the data.  I will update the queries to reduce the chatty nature but want to get them out there for those that need the information that can be pulled now.

## Authors
* **Rob Reilly**

## Acknowledgments
* Thanks to Mark White for his example Power Query on Reading Zip Files
    * http://sql10.blogspot.com/2016/06/reading-zip-files-in-powerquery-m.html
