# GEOG5990M - Final Project

## What are spatial patterns of socio-economic deprivation across Leeds Lower Super Output Areas (LSOAs) and how can these patterns be best utilised to target a support programme?

### Background
Socio-economic deprivation exhibits significant spatial patterns across urban areas with pockets of severe deprivation concentrated in certain LSOAs. This project investigates the spatial distribution of deprivation across Leeds LSOAs using 2011 census data. Through multivariate and spatial analysis techniques, it aims to identify the most deprived areas. The findings can inform targeted support programs and evidence-based strategies to address socio-economic inequalities and promote inclusive development in disadvantaged communities.

### Data Sources
- 2011 Census data on socio-economic deprivation variables for LSOAs can be sourced from https://www.nomisweb.co.uk/
- The shapefile for England LSOA is sourced from https://geoportal.statistics.gov.uk/
  - This shapefile was clipped to the extent of Leeds
- Leeds Ward's shapefile is sourced from https://infuse.ukdataservice.ac.uk/
  - This shapefile provided context to the map for easier interpretation of the results
  
### Objectives
The code in this repository aims to achieve the following objectives:
1. Data Preprocessing: Clean and transform the raw 2011 census data for Leeds LSOAs, handling missing values, and preparing the data for analysis.
2. Deprivation Index Calculation: Construct a composite deprivation index by combining multiple standardised socio-economic indicators.
3. Data Analysis: Employ Spearman's rank correlation to quantify the association between socio-economic variables and the calculated deprivation index.
4. Visualization: Generate non-spatial and spatial visualizations to represent the distribution of deprivation scores and identify the most deprived areas within Leeds.
5. Program Targeting: Explore how the spatial insights obtained from the analysis can inform the design and implementation of support programs to effectively address the specific needs of the most deprived communities in Leeds.

### Requirements and Setup
To run the code and reproduce the analysis, the following requirements and setup steps are necessary:
- Data
  
  The specific datasets required include:
  - The variables selected in this project to show spatial patterns of socio-economic deprivation are based on Townsend indexes (Townsend et al., 1988), which focus on 
    fewer, more direct indicators of 'lack' or 'want.' The variables selected are: Unemployed, Households with No Cars, Overcrowded Households, Lone Parent Households, Low      Social Class, Social Rented Housing.

- Software and Dependencies
  The code is written in Python and requires the following software and package dependencies:
    - The script could be run using google collab using this link: https://colab.google/ or install Anaconda using this link: https://www.anaconda.com/download
    - Required packages are:
      
        import pandas as pd                
        import numpy as np                 
        import matplotlib.pyplot as plt    
        import matplotlib.patheffects as path_effects   
        import seaborn as sns              
        import geopandas as gpd           
        import pyproj                      
        import contextily as ctx         
        import geoplot as gplt             
        import geoplot.crs as gcrs         
        from matplotlib_scalebar.scalebar import ScaleBar
        from sklearn.preprocessing import StandardScaler
      
### Configuration and Setup

Before running the code, the following configuration steps may be necessary:

   - Update the file paths in the code to match the locations of the downloaded datasets on your local machine.
   - Set any required environment variables or configuration parameters specific to your system


#### Contact

If you have any questions or concerns, please reach out at: baluwac@gmail.com / gy23c2b@leeds.ac.uk

