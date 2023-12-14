# Land cover analysis around Mount Whitney
### Linus Ghanadan
## Purpose
In this analysis, I’ll use a raster dataset from the U.S. Geological Survey (USGS) to extract land cover statistics in a small region surrounding Mount Whitney in California. The numbers contained in the raster represent land cover classification, so I will also have to use an accompanying CSV file from USGS that tells us what classes of land cover correspond to these numbers. I’ll also be creating a simple map showing the area of analysis relative to Mount Whitney. An analysis of this kind has potential use for government agencies seeking to better understand land cover in a region.

## Highlights of analysis
- Exracting pixels per land cover class from raster dataset
- Marging extracted pixels with tabular dataset matching numeric codes to character strings
- Creating horizontal bar plot showing percent area of different land cover classes
- Extracting bounding box of raster dataset
- Creating map that shows area of land cover analysis relative to Mount Whitney with California boundaries as a basemap

## Dataset descriptions
1) The primary dataset comes from the 2011 National Terrestrial Ecosystems data, which was collected as part of the USGS Gap Analysis Project (GAP) by the U.S. Forest Service and Department of the Interior. For the purposes of this analysis, the full, nationwide dataset was pre-processed in Microsoft Planetary Computer to only include the area around Mount Whitney. With 30 meter by 30 meter pixel resolution, this raster dataset is a TIF file and contains numbers representing land cover classification.
2) The second dataset is also from the 2011 National Terrestrial Ecosystems data and helps us make sense of data in the raster dataset. This tabular dataset is a CSV file and has the land cover classification names associated with each code used in the raster dataset. This dataset was accessed from the same online source as the raster dataset.
3) Shapefile of California geographic boundaries, included in the U.S. Census Bureau's 2016 Topologically Integrated Geographic Encoding and Referencing (TIGER) database. We will use this shapefile to plot our basemap when visualizing our area of analysis.

## Data references
1) U.S. Geological Survey. 2016. “GAP/LANDFIRE National Terrestrial Ecosystems 2011.” https://doi.org/10.5066/F7ZS2TM0.
2) U.S. Geological Survey. 2016. “GAP/LANDFIRE National Terrestrial Ecosystems 2011.” https://doi.org/10.5066/F7ZS2TM0.
3) California Open Data. 2019. “CA State Boundary.” https://data.ca.gov/dataset/ca-geographic-boundaries/resource/3db1e426-fb51-44f5-82d5-a54d7c6e188b
