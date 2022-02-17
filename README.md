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

## Observations
1. <ins>Student Attendance vs Crime Rate</ins>: Overall, there is a moderate negative correlation, where increase in crime rate leads to a decrease in student attendance, but the correlation is becoming less significant over the past 10 years. A linear regression analysis does not fit this dataset well (r2-values < 0.25).  Was there a COVID-19 impact in 2021?  
2. <ins>College Enrollment vs Crime Rate</ins>: In contrast to the trend in attendance, college enrollment is becoming more strongly correlated over the past 10 years, where more crime correlates to lower college enrollment. Similar to attendance, the linear regression analysis does not fit this dataset well.  
3. <ins>College Enrollment vs Attendance</ins>: There was a high correlation between college enrollment and attendance. The linear regression model fits about 54% of the data, which is a moderate to high degree of correlation. This is in line with our hypothesis, as students who regularly attend school, either for the drive to do well, or the enjoyment, or other reasons, would want to continue their education studies in college.  

## Opportunities for Follow-up
* Different subsets of crime (violent crime, gun violence, drugs, etc.) and the impact on education metrics.
* Other measurements of education success (test scores, job placement, etc.).
* Different statistical models which might better explain the data (other than linear modeling).
* Compare to other cities, or other zip codes in the state of Illinois to determine if similar correlations exist.
