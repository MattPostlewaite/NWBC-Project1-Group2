# NWBC-Project1-Group2
Analysis of education success metrics of Chicago's Public School students (attendance and college enrollment) with respect to crime rate in the area. 
The following years were analyzed:
* 2011
* 2015
* 2021

## Education Data
Education data was pulled from progress report cards found at the City of Chicago, Education, data website.  
The data set was downloaded and organized to prepare for analysis.  
The data was grouped by zip code for comparison purposes.  
Reference program: project_1_analysis_Billy.ipynb  

## Crime Data  
Crime data was pulled from the City of Chicago, Public-Safety, data website.  
The data set was downloaded and organized to prepare for analysis.  
Zip code data needed to be integrated utilizing the latitude and longitude of the crime data as a reference.  
The module USZIPCODE was utilized for this cross-reference: (https://uszipcode.readthedocs.io/index.html#)  
The data was grouped by zip code for comparison purposes.  
Reference program for data organization: initial_crime_data_cleanup.ipynb  
Reference program for zip code reference: zipcode_lookup.ipynb  

## Analysis
Analysis was performed by looking at both attendance and college enrollment rate versus the crime rate for each zip code in the city of Chicago.  
Scatter plots were generated to visually display the relationship.  
Regression analysis and Pearson correlation coefficients were calculated to determine the correlation between education success (attendance and college enrollment rate) and crime rate.  
College enrollment rate versus attendance was also reviewed using the same analysis to determine if there was a correlation.  
Reference program: school_crime_analysis.ipynb
