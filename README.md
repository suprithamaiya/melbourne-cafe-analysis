# melbourne-cafe-analysis

## Overview
Analysis of Melbourne's café seating trends from 2002–2024 using City of 
Melbourne CLUE business census data and ABS 2021 Census income and 
population data.

## Research Question
How has Melbourne's café and dining scene evolved over two decades 
(2002–2024), and is seating capacity distributed equitably across suburbs?

- How has Melbourne's café scene grown from 2002 to 2024, and which suburbs have consistently dominated by seating capacity?
- Did COVID-19 (2020–2021) cause a measurable shift from indoor to outdoor seating across Melbourne?
- Do higher-income suburbs have disproportionately more seating capacity per resident? 

## Data Sources
- City of Melbourne Open Data Portal — Café, Restaurant and Bistro Seats
- ABS 2021 Census DataPacks — G01 (population) and G02 (income), Victoria, SA2
- ABS ASGS 2021 Geographic Descriptor File

## File Structure
data/
  raw/
    2021Census_G01_VIC_SA2.csv
    2021Census_G02_VIC_SA2.csv
    cafes-and-restaurants-with-seating-capacity.csv
    postcodes/
      postcodes.shp
      postcodes.dbf
      postcodes.prj
      postcodes.cpg
      postcodes.shx
    Metadata/
      2021Census_geog_desc_1st_2nd_3rd_release.xlsx
  processed/
    cafes_filtered.csv
    cafe_equity_analysis.csv
  metadata.csv
  data-dictionary.csv
  sample-clue.csv
  sample-equity.csv

## How to Reproduce
1. Download data files from sources listed above and place in data/raw/
2. Open WCD Assignment 4.Rproj in RStudio
3. Render assignment4_35196726.qmd

## Requirements
R packages: tidyverse, here, sf, readxl, ggrepel, patchwork