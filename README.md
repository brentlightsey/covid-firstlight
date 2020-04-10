# Power BI Report for COVID-19
## by Brent Lightsey of FirstLight Analytics

### Overview
This repo contains a Power BI file useful for processing the COVID-19 data provided on the [Johns Hopkins github repo](https://github.com/CSSEGISandData/COVID-19). 

A preview of the finished dashboard can be viewed [here](https://app.powerbi.com/view?r=eyJrIjoiMzVkNGY5NzYtMmQxMS00YmI4LTk1YWUtYmQ4MmU0Y2M4ODg3IiwidCI6Ijg3YzgyMjg3LWRkOGMtNGEzZC1hNzFhLWUxMTc0ZDdiOTgxYyIsImMiOjF9). 

### The Data
Daily, Johns Hopkins publishes updated data to their github repo. The data is organized as a series of files, one for each day. Each day's file has the number of confirmed cases, deaths, and recovered cases for a given geography, usually at the county level in the US or as low a level as possible in the given country.

The Power BI file uses PowerQuery (M) to combine these files into one dataset. It also reaches out to other websites for helpful information like population data and geographic abbreviations. It also makes use of the [MapBox visual](https://docs.mapbox.com/help/troubleshooting/integrate-mapbox-visual-with-power-bi/). (I have noticed that the LastPass browser extension can interfere with this visual. If you use that extension, please open the report in a different browser or use private mode to temporarily disable it.)

This data is also presented in this [ARC GIS dashboard](https://www.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6). It's very useful but the purpose of this file is to put all the data behind this dashboard in your hands.

### How to Use This on your PC
#### Clone the data from the COVID-19 repo to your PC
1. Go to [https://github.com/CSSEGISandData/COVID-19](https://github.com/CSSEGISandData/COVID-19)
2. Either download the files as a ZIP, or...
3. Use git to clone the repository locally (for information on how to do this, see [this article](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository))
4. Clone this repository locally to your PC. Note the path to the location where the files were cloned (Ex: _"C:\Data\COVID"_).

#### Clone the Power BI report and set the parameters

5. Open the Power BI file **covid\_firstlight\_analytics.pbix**. This was devloped with the February 2020 version of Power BI Desktop version 2.78.5740.861. Will require this or higher to open.
6. The file has data through 4/9/2020 in it, but to use the latest data, we will edit to the parameters to point to your locally downloaded data. Click "Transform Data" -> "Edit Parameters" 
![Screenshot: edit parameters](http://firstlightanalytics.com/wp-content/uploads/2020/04/2020-04-10_11-00-17.png)
7. Enter the path to the folder where your data was cloned. (Ex: _"C:\Data\COVID"_ from above)
![Screenshot: new parameter](http://firstlightanalytics.com/wp-content/uploads/2020/04/2020-04-10_11-00-34.png)

8. Click OK
9. Refresh the Report


### Support
I hope you find this report useful to make the best decisions for you, your loved ones, and your business. Use this report or the code it contains in any way you see fit!

If I can help you with this report, or anything else, please feel free to reach out to me at [brent@flda.io](mailto:brent@flda.io), or find me [here on LinkedIn](https://www.linkedin.com/in/brentlightsey/) 

![LinkedIn Logo](https://content.linkedin.com/content/dam/me/business/en-us/amp/brand-site/v2/bg/LI-Bug.svg.original.svg)<a href="http://firstlightanalytics.com"><img src="http://firstlightanalytics.com/wp-content/uploads/2020/04/IconTranspColor-12.png" width="90" /></a>





