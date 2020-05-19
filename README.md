# Data-Science-Analytics-and-Exploration_Capstone-Project-III

## Purpose
The Capstone Project III is conducted as an EDA on data selected from a source of my choosing. For this EDA, a data set containing historic dam level info for the period from November 2015 to March 2016. The overall purpose is to review and provide clarity on the information contained within the data set and explore any trends or underlying information that we can extract from the state of the dams during the period in question. 

## Data Set
The dam levels data set contains records of 211 water bodies across South Africa. The set includes geographic coordinates, dam capacities, catchment areas and additional water management descriptors. Furthermore, there is a bank of continuous type data columns depicting the dam levels in both volumetric parameters and as a percentage of actual design capacity. 

The set did however contain a large amount of columns with a high degree of missingness. The columns and specific dam records showing a large portion of missing values were dropped and therefore not included in the analysis. 

## Data Analysis
**Data Cleaning and Missing Data**

A series of scatter and line plots are generated to explore the overall data distribution. Additionally to highlight any trends or relationships between the columns as well as clearly showing any outliers present within the set. Some outliers were further assessed and found to be true, such as the volume of Gariep Dam which is the country's largest body of water. Finally, the formatting was formalised and data types set correctly to ease the modelling process.

**Data Stories and Visualisations**

The actual locations of the dams are provided as GPS coordinates. This data is plotted using Geoplotlib and provides a great visual of these positions across the country. 

Additional histograms and scatter plots were utilised to provide time series illustrations of the level fluctuations over time, and give insight into the overall dam design capacities and volumes of water recorded. 

## Findings
A list of the top 15 dams ranked by design capacity provides a list of familiar names, the largest being the Gariep Dam. Based on these findings, a time series line plot of the actual Gariep Dam levels was plotted against the design capacity. Throughout the period the dam was seen to consistently be recorded at around 50% capacity. 

This may have been an indication of a poor water level status across the country. A similar plot was generated depicting the percentage volume of the top 15 largest dams. This plot however showed a wide spread distribution of levels ranging from roughly 15% up to 100%. 

Further to these findings, in order to determine the status of all dams in the country (not just the 15 largest), percentage full plots were generated for each month during the period. Initially, we see a skewed distribution with a high number of dams reflecting near 100% capacity, over the months we see a shift as water levels begin to drop and the population adjust to show a lower level across the population.

A further analysis was conducted on the water bodies found within the Gauteng province, this provided details on the main dams that service the region as well as the volumes and proportions contributed per dam. **NOTE: The Rietvlei Dam records showed high degrees of missingness and were therefore dropped from the data set during the cleaning stage.**

A stacked area plot visual was used to best show the volumes per dam over the period. The two largest dams (being the Roodeplaat and Bronkhorstspruit) held the large majority of water with the third contributor (the Bon Accord Dam) holding a small percentage. 

Lastly, to determine the effect of the catchment area on the actual design dam capacity and the overall percentage full, two scatter plots were generated to find any relationship of correlation between these parameters. It was found that the larger catchment areas almost always resulted in the dams showing a volume of 80% or higher, this is an intuitive relationship and the data seems to hold. The dam capacity however did not show a direct correlation, in fact the opposite could be argued based on the data. This metric is however not likely to provide usable information but merely an interesting comparison.
