# MERRA-2 GLOBAL DUST AND ITS IMPLICATIONS
 
## Aidin Raphael Abramowitz

## Introduction

I am applying MERRA-2 Global Data to a variety of different dust related variables to determine unique phenomena.
In general, the aim to to describe the influence of dust on a global scale during a selected year, and visualise certain regions throughout the globe that are uniquely prone to anomalies, correlations, and other interpretations.

## Data

From the year of 2015:
The Modern-Era Retrospective analysis for Research and Applications, Version 2 (MERRA-2) , NASA GLOBAL MODELING AND ASSIMILATION OFFICE
Spatial Grid: 2D, single-level, full horizontal resolution
Dimensions: longitude=576, latitude=361, time=24, Global 
Data includes 115 different data variables

AND 

North Atlantic Oscillation (NAO) Climate Index from [NOAA](https://psl.noaa.gov/data/climateindices/list/) that has monthly data from 1948-2023.

## Code Description (Links Included)

- Average Submicron Dust Emissions (Bin 001) globally on the day of [August 25th, 2015](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/Plotmean.ipynb).

- Next, I wanted to show how each month varied in regards to Aerosol Optical Thickness (AOT) at (550 nm) - PM 1.0 um. AOT is a measure of aerosols distributed with a column of air.
    - To seperate by month, we used the groupby function. This can be found in other codes used throughout this project. [AOT link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/CompositeAOT.ipynb)


- Using an NAO index from NOAA and Previous AOT data, I looked at Positive and Negative months in the year of 2015, to determine where AOT Anomalies were positive or negative. [NAO To AOT composite link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/NAOtoAOTcomposite.ipynb)

- Calculated the temporal coorelation coefficient between Submicron Dust Emissions (Bin 001) and Dust Extinction AOT (550 nm) - PM 1.0 um. This is of specific interest, as it allows us to determine if the correlation between the two are linearly related enough to be of research interest. Therfore, I applied code that found the [Coorelation Coefficient](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/CoorelationCoef.ipynb) throughout the globe. As well, I used a function to create the tick marks for the latitude and longitude for the plot.

- I created a composite the year of 2015 for both Submicron Dust Emissions (Bin 001) and Submicron Sea Salt Emissions (Bin 001) , and made a scatter plot to demonstrate if globally there was a coorelation that was signficant. [Coorelation With Statistical Signficance link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/ComparisonBetter.ipynb)


## Results

Firstly, on August 25th of the year 2015, Submicron Dust Emissions (Bin 001) values were the largest in Western Sahara. Other larger amounts across the globe comparitively include spots in Somalia, the Middle East region, and Northern China.

Higher values in the composite graphs represent where dust is most commonly distributed throughout the globe during various months. From there, we can extrapolate its meaning. The composite of the AOT show larger values in west Africa. The months of March, April, and December have the highest AOT during the month of 2015. Winter and Spring dust storms are common in west Africa, so the results match up with what is expected. However, the higher values of AOT are located south of the Sahara, which was unexpected. 

Comparing the Aerosol Optical Thickness to the North Atlantic Oscillation Index. During the year of 2015, there were 9 months that were in a positive phase, and 3 that were in a negative phase. During the positive phase, positive AOT anomalies were most common. Notable locations include the Sahara and West Africa, Saudi Arabia, and Northern China.
In the negative phase months, there was a fairly even mix of positive and negative anomalies thoughout the previous regions listed. 

Next, the correlation between Submicron Dust Emissions (Bin 001) and Dust Extinction AOT (550 nm - PM 1.0) um during the year of 2015 was found. As reinforced by previous code, Saharan Africa is particularly notable. However regions such as the western coast of South America, Western North America, and Australia show coorelations. In Australia, The Middle East, Most of Saharan Africa, and areas of North America (such as Arizona and surrounding areas), South America, and Northern China, a positive coorelation coefficient could be found. Small areas of South America, North America, Saharan Africa, and China experienced negative, and less pronounced, correlation coefficients. Areas with Positive coorelation coefficients have dusty and desert-like climates, so a coorelation between the two is not unexpected.

Finally, submicron dust emmisions are particuarly week monthy. However, months with relatively larger values include, January, March, March and December in the center of Northern Africa. For Sea Salt Emissions, particularly large averages occured in June, July, and August. These occured around the Arabian Sean and Indian Ocean. As well as off the Eastern Coast of China. With a scatter plot, it was found that there was a very small negative coorelation between the two with a p-value of 0.05. This suggests that there is likely little no no coorelation between the two variables.  

## Summary

Many of the results found were expected as Saharan and African dust would be expected to influence many of the global results. For example, areas with Positive coorelation coefficients have dusty and desert-like climates, so a coorelation between Submicron Dust Emissions and Dust Extinction AOT is not unexpected. However, since winds pick up aerosols from the ocean and well as land, I expected there to be a statistically signficant coorelation between dust and sea salt. However, this did not seem to be the case. In regards to the project, I learned to use various statistical techniques and learned out to organize data to produce meaningful composites and plots. One issue I had to overcome however was how my data was initially. There were many variables within the initial file, which made it particualry difficult to load within Jupyter. In the future, finding datasets with less variables might be more conducive to efficiently making plots. 






