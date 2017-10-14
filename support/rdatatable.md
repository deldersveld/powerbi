# R Data Table - Support

Power BI custom visual by David Eldersveld  

### Contact me on Twitter - @dataveld 
### Log an Issue on [GitHub](https://github.com/deldersveld/rDataTable/issues)  

Based on the [DT package](https://rstudio.github.io/DT/), **rDataTable** is an interactive Power BI **R** custom visual that helps you easily explore table data.  

![](https://github.com/deldersveld/rDataTable/raw/master/images/rDataTable.PNG)

  
## Functionality  
Some of the benefits of rDataTable include:  

* **Search** 
  * Global search field to filter data across all columns  
  ![](https://github.com/deldersveld/rDataTable/raw/master/images/GlobalSearch.PNG)  
  
* **Pagination**
  * Use "Show # of entries" to choose between 5, 10, 25, 50, 100, or 1000 records to display per page  
  ![](https://github.com/deldersveld/rDataTable/raw/master/images/ShowEntries.PNG)  
  
* **Column-level filters**
  * Conveniently filter column values using the option below each column header  
  ![](https://github.com/deldersveld/rDataTable/raw/master/images/ColumnFilters1.PNG)  
  ![](https://github.com/deldersveld/rDataTable/raw/master/images/ColumnFilters2.PNG)  
  ![](https://github.com/deldersveld/rDataTable/raw/master/images/ColumnFilters3.PNG)  
  
## Format Options
Under *Format*, a section called *Visual Settings* contains various format options:
* **Initial Entries** - Choose the default number of entries/records per page
* **Filters** - Choose how to display the column filters (Top, Bottom, None)

![](https://github.com/deldersveld/rDataTable/raw/master/images/FormatOptions.PNG)  


## NOTES
* User-defined selections and filters are not preserved between sessions. When used in a report, the initial view will appear with all of the data specified under Values (defaults to 5 entries to page, no in-visual filters applied, no search value). This limitation makes it a good exploratory but not necessarily a good explanatory visual.
* Optimal visual height is **415px or greater**.

## Environments  

### Power BI Desktop
rDataTable requires the **htmlwidgets** and **DT** packages installed in your local R environment to work with Power BI Desktop.

### Power BI Service
All required packages are currently available in the Power BI Service. rDataTable runs in Power BI Service and has been tested in Chrome, Firefox, and Edge.

### Power BI Mobile
rDataTable runs as a fully interactive visual in the Mobile app and has been tested in iOS (Android testing still needed).  
![](https://github.com/deldersveld/rDataTable/raw/master/images/iOS0.jpg)   
![](https://github.com/deldersveld/rDataTable/raw/master/images/iOS1.jpg)   
![](https://github.com/deldersveld/rDataTable/raw/master/images/iOS2.jpg)

### Embedded or Publish to Web
This functionality is not available to any R Visuals in Power BI as of July 2017.
  

## Changelog
* 1.1.0 - October 10, 2017
  * Corrected issue where unicode characters were not appearing correctly
* 1.0.1 - July 15, 2017
  * Added Format options for Initial Entries and Filters
  * Adjusted Dependencies.json
