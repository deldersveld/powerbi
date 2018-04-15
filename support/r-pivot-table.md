# R Pivot Table - Support

Power BI custom visual by [BlueGranite](https://www.blue-granite.com)  

### [Log an Issue on GitHub](https://github.com/BlueGranite/RPivotTable-for-Power-BI/issues)  
# R Pivot Table for Power BI
An interactive R HTML *Pivot Table* for Microsoft Power BI from [BlueGranite](https://www.blue-granite.com).

### PREVIEW
R Pivot Table is in early preview. It is in the process of being submitted to Microsoft AppSource. For limited use and testing, you can download **RPivotTable-1.0.2.3.pbiviz** for non-production environments from the [*packaged-versions*](https://github.com/BlueGranite/RPivotTable-for-Power-BI/tree/master/packaged-versions) folder in this repository. There is no support currently offered for this visual while in preview, but please log any problems in the Issues section of this repository. 

### Using R Pivot Table by BlueGranite  
R Pivot Table for Power BI is an interactive R HTML visual that relies on R's *rpivotTable* package. This visual is available for use in both Power BI Desktop and Service. As an R visual, it will not render in Power BI Report Server or the Mobile app. If using this visual in Power BI Desktop, be sure to install the *htmlwidgets*, *jsonlite*, and *rpivotTable* packages in your local R environment.

1) Add an instance of the R Pivot Table visual to the report canvas.  
2) Add data to *Values*. The first value in the list will default to Rows. The second (if available) will default to columns. Additional fields will be available for use as desired.  
3) Click and drag available fields to the dark "Row" and "Column" panes to dynamically build a pivot table.  
4) Select options to change the appearance of the pivot table.  


### Format options

**Font Size** - set the font size ranging from 10 to 20 (default 12)  
**Decimal digits - Header Labels** - set the number of decimal places to use if a numeric field appears as a Row or Column header

### Limitations
There are several limitations to this pivot table that make it a good *exploratory* visual but not a good *explanatory* visual:
1) Although R HTML visuals are interactive, you cannot select and filter other visuals by clicking inside the R visual.  
2) There is no "freeze header" capability like you have in Excel.  
3) The Custom Visuals API does not currently expose format string for R visuals. The number of decimal places and formatting may not be what you expect based on other, non-R, visuals.  
4) Printing or exporting the filtered view is not available from the pivot table.  
5) In-visual filter selections are not retained. If you want a persistent filter applied to the visual for different fields, use the native Power BI page- or visual-level filter options.  
6) Data type formatting is not available for R visuals. Use the Decimal Digits - Header Labels option under Format-Visual Settings to specify the number of digits to display when a numeric field is used as a Row or Column header.  
7) Visual load time increases substantially as you increase the number of records available for the visual to use.

R Pivot Table requires the htmlwidgets, jsonlite, and rpivotTable R packages installed if you use the visual in Power BI Desktop. These packages are already available in Power BI Service.

![](https://github.com/BlueGranite/RPivotTable-for-Power-BI/raw/master/images/RPivotTableSample.gif)  
![](https://github.com/BlueGranite/RPivotTable-for-Power-BI/raw/master/images/rpivotTable.PNG)  
![](https://github.com/BlueGranite/RPivotTable-for-Power-BI/raw/master/images/rpivotTable.gif)

## Version History  
### 1.0.2.3
- Initial AppSource submission
- Font size format option
- Decimal digit format option
- Save state based on report developer's field selections (not user in read-only)
### 1.0.1.6
- Initial public version


## License  
The R Pivot Table for Power BI is licensed under the MIT License.
