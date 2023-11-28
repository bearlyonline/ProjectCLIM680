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

Based on my own graduate research, the day of August 25th, 2015 is of specific interest. While my own research is focused on a much smaller region, I was curious to know the level of submicron dust globally on the day of [August 25th, 2015](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/Plotmean.ipynb).

Next, I wanted to show how each month varied in regards to Aerosol Optical Thickness (AOT). AOT is a measure of aerosols distributed with a column of air. Higher values in the composite graphs I made should represent where dust is most commonly distributed throughout the globe during various months. From there, we can extrapolate its meaning. [AOT Link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/CompositeAOT.ipynb)

As well, it is important to compare Aerosol Optical Thickness to various atmospheric phenomena. More specifically, I decided to focus on the North Atlantic Oscillation (NAO). NAO refers to changes in pressure patterns in the atmosphere over the north Atlantic. As a signficant amount of dust comes from the Sahara in Africa and is picked up by those winds influenced by pressure patterns, this was of specific interest. Using an NAO index from NOAA and Previous AOT data, I looked at Positive and Negative months in the year of 2015, to determine where AOT Anomalies were positively or negatively coorelated. [NAO To AOT composite Link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/NAOtoAOTcomposite.ipynb).

Next, I wanted to determine the coorelation between Submicron Dust Emission (Bin 001) and Dust Extinction AOT (550 nm) - PM 1.0 um. This is of specific interest, as it allows us to determine if the correlation between the two are linearly related enough to be of research interest. Therfore, I applied code that found the [Coorelation Coefficient](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/CoorelationCoef.ipynb) throughout the globe.

Finally, As previous code assessed the North Atlantic Oscillation. Therefore, I thought it would be of interest to compare submicron dust emiisions to an submicron sea salt emissions. I created a composite the year of 2015, and made a scatter plot to demonstrate if there was a global coorelation that was signficant. [Coorelation With Statistical Signficance Link](https://github.com/bearlyonline/ProjectCLIM680.github.io/blob/master/ComparisonBetter.ipynb)

## Results

