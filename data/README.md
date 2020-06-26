
Final Project - MAP 673 draft
# national_WNV_1999-2018
# 🚀

## Description
    Description: My web map will display the reported number of West Nile Virus cases, by state, from 1999 to 2018 using data from the Centers for Disease Control (CDC).	

## Title
* Potential titles: "Mapping an Arbovirus:"
* Potential subtitles: "Timeline of West Nile Virus in the United States, 1999 to 2018", or "Tracking West Nile Virus in the United States, 1999 to 2018"

## Data Sources
			
* Data Sources: 
    * West Nile virus disease cases reported, by state, 1999-2018
        * Link: https://www.cdc.gov/westnile/statsmaps/cummapsdata.html
        * Note: This will have to be copied and pasted into an appropriate file, as it only exists on the web page or in a downloadable pdf.	
    * I haven't found this data by county for the US, but will continue looking. If it's available from a single source, and doesn't require piecing together from 50 state health departments, I plan to use those boundaries.				

    * State Boundaries: us-states.json
        * Link: https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html
    * County Boundaries: us-counties.json (SEE NOTE ABOVE)



## Identify your anticipated methods of thematic representation methods (e.g., dot map, choropleth, prop symbols, etc.)
The data will be represented using a dynamic choropleth map


## Briefly describe your anticipated user interface (UI)
This map will use a time slider to visualize year-to-year changes, with a tooltip displaying state names, and sparkline statistics, at a minimum.


## User Needs
Users need to quickly view the data by state and/or county, and quickly select the year they're interested in examining. As a supplemental visual, sparklines will show changes over time for each state (or county, if the data are available) for the entire time series.


## Technology stack

While your answer to this question need not be definite at this point, briefly describe the "technology stack" you plan to use for your final map. Your description of the technology stack should include:

## Data and information processing tools, web-based or desktop (i.e., QGIS, MapShaper)
* Visual Studio Code
* Microsoft Excel

## The format you'll use to store your data (i.e., flat files such as CSV or GeoJSON, database technology such as CARTO)
* West Nile Virus data will be contained in a CSV file
* State boundaries will be contained in a geoJSON file 

## The JS libraries you anticipate using or need (include any relevant plugins, like omnivore) and other relevant web technologies you'll be using (i.e., HTML, CSS)

* JavaScript
    * Leaflet
    * JQuery
    * Papa Parse 
* HTML
* CSS
* GitHub

## The hosting platform you intend to use to host your map (i.e., GitHub pages, your web server, http://surge.sh/)
* GitHub Pages portfolio at cpe3.github.io


## "Wish List"

### Data and Overall Concept
* Higher resolution GeoJSON boundaries
* Higher resolution dataset - data for individual counties
* Better metrics for choropleth - % of total population doesn't necessarily make sense in this situation, as it would be a vanishingly small number. 


### UI Controls
* Pop-up on slider control to show year in addition to year shown in the upper right
* Different shape for slider control button

