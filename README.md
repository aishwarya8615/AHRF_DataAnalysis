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
**Processed File Sample Images**
Note: Unable to upload the complete processed file due to its size.

* Processed Input File-Generic
![processedfile1](https://user-images.githubusercontent.com/54454914/97843676-b539f780-1cb7-11eb-9649-cfd5f9fc3bb9.JPG)

* Processed Input File - Data specific
![processedfile2](https://user-images.githubusercontent.com/54454914/97843731-cf73d580-1cb7-11eb-9753-a1ddaaf6de99.JPG)

**Few Visualizations:**
* Interactive HeatMap of the number of primary care physicians by county in 2017
![HEatMap](https://user-images.githubusercontent.com/54454914/97842560-c71a9b00-1cb5-11eb-8f38-0c6f0170c03a.JPG)

* Yearwise comparison barchart for different groups of primary care in USA
![barchart](https://user-images.githubusercontent.com/54454914/97842764-237dba80-1cb6-11eb-95bc-01cac36fed64.JPG)

* Percentage of MD's in different age groups across 3 years
![MD%_diffagegroups](https://user-images.githubusercontent.com/54454914/97842878-62ac0b80-1cb6-11eb-9c3d-3fac86321a1c.JPG)

* Interactive scatterplot of Total MD's per state in 2017
![TotalMD_perstate](https://user-images.githubusercontent.com/54454914/97843013-9129e680-1cb6-11eb-95e3-07a92ebfcf8e.JPG)

* Comparison plot of total MD's in 2017 and 2010
![Comparisonplot](https://user-images.githubusercontent.com/54454914/97843124-c1718500-1cb6-11eb-9e04-48efe5cec250.JPG)

**Technical References:** 
* 1.	Pandas API Reference - https://pandas.pydata.org/docs/reference/index.html#api
* 2.	https://regex101.com/  - to quickly validate regex expressions
* 3.	How to expand lists in a dataframe - https://stackoverflow.com/questions/53218931/how-to-unnest-explode-a-column-in-a-pandas-dataframe
* 4.	Choropleth map - https://plotly.com/python/choropleth-maps/

**Issues faced:**
*	Jupyter nbextensions does not appear - https://stackoverflow.com/questions/49647705/jupyter-nbextensions-does-not-appear/50663099
*	Writing to csv one row of dataframe at a time seemed to be time consuming.  So opted to group writing to file as 100 rows
*	FIPS code was getting converted to integer and the leading '0' was getting omitted
*	Interactive plots were not getting displayed In Github. Showed the static plot. Please run the notebook with the data file to see the interactive maps


