# Chapel Thrill Escapes Customer Geospatial Analysis

## Project Overview

This project aims to map out the locations of Chapel Thrill Escapes customers to inform future marketing strategies better. By identifying areas with higher concentrations of customers, we can target our marketing efforts more effectively. This analysis uses geospatial data to create visualizations that highlight regions with a significant number of customers, suggesting where future sales might be maximized.

## Data Preparation

The analysis begins with data cleaning steps applied to the customer address list. These steps include standardizing address formats, correcting misspellings, and removing unnecessary details such as room numbers. The cleaned addresses are then geocoded to obtain latitude and longitude coordinates for mapping.

### Key Steps:

1. **Address Cleaning**: Standardize and correct address formats.
2. **Geocoding**: Convert cleaned addresses to geographic coordinates.
3. **Data Filtering**: Exclude specific addresses known to cause issues in the geocoding process.

## Geospatial Analysis

With the geocoded addresses, we perform a geospatial analysis to visualize the distribution of Chapel Thrill Escapes customers across the area. The analysis involves creating a heatmap overlay on a dynamic Leaflet map, providing insights into customer density in different regions.

### Visualization:

- **Static Maps**: Initial exploration with `tmap` to plot customer locations within North Carolina.
- **Interactive Map**: Use `leaflet` to create an interactive map with a heatmap layer. This map allows users to zoom in and out to explore areas of interest, with the heatmap indicating the density of customers.

## How to Run the Analysis

The analysis is performed in R, utilizing packages such as `sf`, `tmap`, `leaflet`, `dplyr`, and others for data manipulation and visualization. To reproduce the results, follow the setup instructions and execute the R code blocks as outlined in the project script.

### Prerequisites:

- R and RStudio installed.
- Required R packages installed: `here`, `sf`, `dplyr`, `tmaptools`, `tmap`, `knitr`, `wk`, `stringr`, `ggmap`, `leaflet`, `leaflet.extras`, `htmlwidgets`.

### Instructions:

1. Clone the repository to your local machine.
2. Open the R project in RStudio.
3. Run the setup block to install and load necessary packages.
4. Execute the code blocks sequentially to perform data cleaning, geocoding, and map visualization.
5. The final map can be viewed by opening the generated HTML file in a web browser.

## Conclusion

This geospatial analysis of Chapel Thrill Escapes customers provides valuable insights for targeted marketing. Areas with higher customer density represent regions where marketing efforts could be intensified to maximize future sales.

---
