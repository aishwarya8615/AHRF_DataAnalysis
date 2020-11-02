# AHRF_DataAnalysis

**AHRF Data Parser:**
This Jupyter Notebook file helps in parsing the ascii file and maps it to the technical documentation to obtain a .csv file of the entire AHRF County Data
Some level of cleaning and preprocessing was done to the file to enable its usage for further data analysis and data visualizations.
Input: AHRF 2018-2019 Technical Documentation.xlsx
           AHRF2019.asc
Output: AHRF2019_processed.csv
**AHRF Data Processing Visualization:**
Preprocesses and normalizes the data for the various visualizations. A few of the visualizations are shown for different subsets of the data.
Input: AHRF2019_processed.csv
Output: Subset of data and visualizations

**Packages Installed [In addition to the required libraries]:**
1. ipynb
2. nbimporter
3. autopep8


**Technical References:** 
* 1.	Pandas API Reference - https://pandas.pydata.org/docs/reference/index.html#api
* 2.	https://regex101.com/  - to quickly validate regex expressions
* 3.	How to expand lists in a dataframe - https://stackoverflow.com/questions/53218931/how-to-unnest-explode-a-column-in-a-pandas-dataframe
* 4.	Choropleth map - https://plotly.com/python/choropleth-maps/

**Issues faced:**
•	Jupyter nbextensions does not appear - https://stackoverflow.com/questions/49647705/jupyter-nbextensions-does-not-appear/50663099
•	Writing to csv one row of dataframe at a time seemed to be time consuming.  So opted to group writing to file as 100 rows
•	FIPS code was getting converted to integer and the leading '0' was getting omitted
•	Interactive plots were not getting displayed In Github. Showed the static plot. Please run the notebook with the data file to see the interactive maps


