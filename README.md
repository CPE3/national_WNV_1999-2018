# Mapping an Arbovirus: Timeline of West Nile Virus in the United States, 1999 to 2018 (Directory name: national_WNV_1999-2018)

## <b>Final Project - MAP 673</b>

## <b>Link to Student Portfolio:</b> [CPE3.github.io](CPE3.github.io)

## Description
    Description: My web map will display the reported number of West Nile Virus cases, by state, from 1999 to 2018 using data from the Centers for Disease Control (CDC).	

## Title
* Title: "Mapping an Arbovirus:"
* Subtitle: "Timeline of West Nile Virus in the United States, 1999 to 2018"

## Data Sources
			
* Data Sources: 
    * West Nile virus disease cases reported, by state, 1999-2018
        * Link: https://www.cdc.gov/westnile/statsmaps/cummapsdata.html
        * Table was copied and pasted , as it only exists on the web page as an HTML table or as a downloadable pdf.	
    * County-level data were not readily available				

    * State Boundaries: cb_2018_5m.geojson
        * Link: https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html
    * State boundaries zipfiles were downloaded and opened as shapefiles in QGIS. They were then saved as geojson files with a number of fields removed and a precision of 4 in the output. I downloaded both the 5m and 500k resolution files. While I prefer the detail available in the 500k file, it's not necessarily to visualize state level data. Additionally, it caused a bug in the legend where the total number of cases were a multiple of the high value in the data. Root cause unknown.
    
    * County Boundaries: us-counties.json (SEE NOTE ABOVE)
    

## Identify your anticipated methods of thematic representation methods (e.g., dot map, choropleth, prop symbols, etc.)
The data will be represented using a dynamic choropleth map


## Briefly describe your anticipated user interface (UI)
This map will use a time slider to visualize year-to-year changes, with a tooltip displaying state names, and sparkline statistics, at a minimum.


## User Needs
Users need to quickly view the data by state and/or county, and quickly select the year they're interested in examining. As a supplemental visual, sparklines will show changes over time for each state (or county, if the data are available) for the entire time series.


# Technology stack

## Data and information processing tools, web-based or desktop (i.e., QGIS, MapShaper)
* Visual Studio (VS) Code
* Microsoft Excel

## The format you'll use to store your data (i.e., flat files such as CSV or GeoJSON, database technology such as CARTO)
* West Nile Virus data will be contained in a CSV file
* State boundaries will be contained in a geoJSON file 

## The JS libraries you anticipate using or need (include any relevant plugins, like omnivore) and other relevant web technologies you'll be using (i.e., HTML, CSS)


* JavaScript
    * Leaflet
    * JQuery
    * JQuery Sparklines
    * Papa Parse 
    * chroma
* HTML
* CSS
* GitHub

## The hosting platform you intend to use to host your map (i.e., GitHub pages, your web server, http://surge.sh/)
* GitHub Pages portfolio at [cpe3.github.io](cpe3.github.io)

## "Wish List"

### Data and Overall Concept
* Higher resolution GeoJSON boundaries
    * IMPLEMENTED: Originally used 1:5,000,000 resolution but changed this to 1:500,000 resolution; Change reverted: more detailed boundaries create a bug that creates a large and incorrect legend value
* Higher resolution dataset - data for individual counties
* Better metrics for choropleth - % of total population doesn't necessarily make sense in this situation, as it would be a vanishingly small number. 
* Center map using data extent
* Different template or css framework with room for additonal text in a sidebar


### UI Controls
* Pop-up on slider control to show year in addition to year shown in the upper right
    * Was able to include year in tooltip popup which provides some measure of this  
* Different shape for slider control button 
    * default pentagonal shape isn't that exciting
* Sparklines
* Dropdown options for different basemaps
    * Would be a nice addition for the user






