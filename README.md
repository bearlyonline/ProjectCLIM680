# Analysis of Phenomena Related to Submicron Dust and Aerosol Optical Thickness (AOT) Throughout 2015 

## Introduction

I am applying MERRA-2 Global Data to a variables concerning submicron dust and the Aerosol Optical Thickness of submicron dust. 
In general, the aim to to describe the influence of submicron dust on a global scale during a selected year, and visualise certain regions throughout the globe that are uniquely prone to anomalies, correlations, etc.

## Data

From the year of 2015:
- The Modern-Era Retrospective analysis for Research and Applications, Version 2 (MERRA-2) , NASA GLOBAL MODELING AND ASSIMILATION OFFICE
- Spatial Grid: 2D, single-level, full horizontal resolution
- Dimensions: longitude=576, latitude=361, time=24, Global 
- Data includes 115 different data variables

AND 

North Atlantic Oscillation (NAO) Climate Index from [NOAA](https://psl.noaa.gov/data/climateindices/list/) that has monthly data from 1948-2023.

## Code Description (Links Included)

- Average Submicron Dust Emissions (Bin 001) globally on the day of [August 25th, 2015](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/Plotmean.ipynb). When a bin is mentioned it refers to the contraption that measures various sizes of aerosols. For our purposes (Bin 001) refers to the smallest dust particles MERRA-2 can measure at a submicron level with a max radius of 0.73 microns for dust.

- Next, I wanted to show how each month varied in regards to Aerosol Optical Thickness (AOT) at (550 nm) - PM 1.0 um. AOT is a measure of aerosols distributed with a column of air, which can signify its abundance in the air within various regions.
    - To seperate by month, we used the groupby function. This can be found in other codes used throughout this project. [AOT link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/CompositeAOT.ipynb)


- Using an NAO index from NOAA and Previous AOT data, I looked at Positive and Negative months in the year of 2015, to determine where AOT Anomalies were positive or negative. For reference, the NAO refers to surface sea-level pressure differences between the subtropical high and subpolar low.  [NAO To AOT composite link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/NAOtoAOTcomposite.ipynb)

- Calculated the temporal coorelation coefficient between Submicron Dust Emissions (Bin 001) and Dust Extinction AOT (550 nm) - PM 1.0 um. This is of specific interest, as it allows us to determine if the correlation between the two are linearly related enough to be of research interest. Therfore, I applied code that found the [Coorelation Coefficient](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/CoorelationCoef.ipynb) throughout the globe. As well, I used a function to create the tick marks for the latitude and longitude for the plot.

- I created a composite for the year of 2015 for both Submicron Dust Emissions (Bin 001) and Submicron Sea Salt Emissions (Bin 001), and made a scatter plot to demonstrate if globally there was a coorelation that was signficant. For Bin 001 for Sea Salt Emissions, this max radius sizes of note are 0.079 and 0.316 for sea salt. [Coorelation With Statistical Signficance link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/ComparisonBetter.ipynb)


## Results

Firstly, on August 25th of the year 2015, Submicron Dust Emissions (Bin 001) values were the largest in Western Sahara. Other larger amounts across the globe comparitively include spots in Somalia, the Middle East region, and Northern China.

![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/cefbf2ed-e146-4ebd-aeb0-a560d739a691)
*Figure 1: Average Submicron Dust Emmisions On August 25th, 2015*


Higher values in the composite graphs represent where dust is most commonly distributed throughout the globe during various months. From there, we can extrapolate its meaning. The composite of the AOT show larger values in west Africa. The months of March, April, and December have the highest AOT during the month of 2015. Winter and Spring dust storms are common in west Africa, so the results match up with what is expected. However, the higher values of AOT are located south of the Sahara, which was unexpected. 

![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/b47957c4-38eb-4b4e-b91b-9e985c14afa5)
*Figure 2: Dust Extinction AOT (550 nm) - PM 1.0 um*


Comparing the Aerosol Optical Thickness to the North Atlantic Oscillation Index. During the year of 2015, there were 9 months that were in a positive phase, and 3 that were in a negative phase. During the positive phase, positive AOT anomalies were most common. Notable locations include the Sahara and West Africa, Saudi Arabia, and Northern China.
In the negative phase months, there was a fairly even mix of positive and negative anomalies thoughout the previous regions listed. 

![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/fabbc7fd-7c68-4246-8cdf-5ecfb6ab72d6)
*Figure 3: Composite AOT Anomalies during NAO in 2015*


Next, the correlation between Submicron Dust Emissions (Bin 001) and Dust Extinction AOT (550 nm) - PM 1.0 um during the year of 2015 was found. As reinforced by previous code, Saharan Africa is particularly notable. However regions such as the western coast of South America, Western North America, and Australia show coorelations. In Australia, The Middle East, Most of Saharan Africa, and areas of North America (such as Arizona and surrounding areas), South America, and Northern China, a positive coorelation coefficient could be found. Small areas of South America, North America, Saharan Africa, and China experienced negative, and less pronounced, correlation coefficients. Areas with Positive coorelation coefficients have dusty and desert-like climates, so a coorelation between the two is not unexpected.

![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/ec4cc7cc-e41d-4dd2-be1a-e1bb2577bce3)
*Figure 4: Correlation between Submicron Dust Emission (Bin 001) and Dust Extinction AOT (550 nm) - PM 1.0 um* 


Finally, submicron dust emmisions are particuarly week monthy. However, months with relatively larger values include, January, March, March and December in the center of Northern Africa. For Sea Salt Emissions, particularly large averages occured in June, July, and August. These occured around the Arabian Sean and Indian Ocean. As well as off the Eastern Coast of China. With a scatter plot, it was found that there was a very small negative coorelation between the two with a p-value of 0.05. This suggests that there is likely little to no coorelation between the two variables.  

![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/6a20c595-7f98-4aea-952d-d46a502c9509)
*Figure 5: Composite Average Submicron Dust Emission (Bin 001)*


![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/e7727f0f-7a0c-45df-af9a-c182d7a6404f)
*Figure 6: Composite Average Submicron Sea Salt Emission (Bin 001)*


![download](https://github.com/bearlyonline/ProjectCLIM680.github.io/assets/135748104/ffafd276-d3bd-4504-9b26-d4a7659facb0)
*Figure 7: Signficance of Composite Average Submicron Dust Emission Compared to Composite Average Submicron Salt Emission*

## Summary

Many of the results such as those related to Saharan and African dust were be expected to influence many of the global results. For example, areas with positive coorelation coefficients have dusty and desert-like climates, so a coorelation between Submicron Dust Emissions and Dust Extinction AOT is not unexpected. In general, Submicron Dust Emmisions and Dust Extinction AOT throughout the project had expected results based on global geography. However, since winds pick up aerosols from the ocean and well as land, I expected there to be a statistically signficant coorelation between dust and sea salt. However, this did not seem to be the case. In regards to the project, I learned to use various statistical techniques and learned out to organize data to produce meaningful composites and plots. One issue I had to overcome however was how my data was initially. Firstly, my files were seperated by day initally, and have over 115 data variables, making them quite large in size. Pulling out the required data, was time consuming, but was eventually overcome. In the future, finding datasets that are better organized could be more conducive to the research process. 






