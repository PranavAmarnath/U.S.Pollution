# U.S. Pollution

A Python notebook for analyzing pollution CSV data.

## About the Data:
* Aims to analyze the change in air quality index (AQI) for 4 major pollutants (Nitrogen Dioxide, Sulphur Dioxide, Carbon Monoxide, Ozone) that cover all 50 states of the United States from 2000 to 2016
* Procured from the Environmental Protection Agency (EPA)
* Consists of daily pollution data for the 4 major pollutants over 16 years for all 50 states (382 MB, 1746661 lines)
* Key points:
    * Organized by Date, dates repeat per county where the source data was acquired
    * NO2 and SO2 are in parts per billion while O3 and CO are in parts per million
    * The max hour describes what hour of the day the AQI was highest

## Methods:
* Reading Data:
    * Pandas to read the CSV
    * Data relatively unorganized<sup>1</sup> but contained diverse information
        * Grouped data by date
        * Calculated the means for each state
* Visualization:
    * Matplotlib - Graphs
    * Cartopy - Maps
    * Types of Visualizations:
        * Multi-line charts
        * Bubble maps
        * Multivariate linear regressions
        * Heat maps

## Results:
Line Charts             |  Map Visualizations
:-------------------------:|:-------------------------:
![image](https://user-images.githubusercontent.com/64337291/176280152-e4422606-2c46-4b96-9719-fd65eb1a1b0e.png)  |  ![image](https://user-images.githubusercontent.com/64337291/176280355-b5eca852-e91c-4714-b1be-56d86baad2f3.png)
![image](https://user-images.githubusercontent.com/64337291/176280630-922abb09-aaf5-4025-97d5-6e0a6b92ec19.png)  |  ![image](https://user-images.githubusercontent.com/64337291/176280787-e3ffcbc4-32ce-4138-af97-a54353bfb7e0.png)

## Discussion:
* CO and NO<sub>2</sub> have decreased while O<sub>3</sub> and SO<sub>2</sub> have largely remained stagnant
* O<sub>3</sub> and NO<sub>2</sub> are recently the more prevalent pollutants compared to CO and SO<sub>2</sub>
* When looking at results, be aware of:
    * Results may be affected by holes in the data as shown in the multi line charts and the heat maps
    * Differentiating between interpreting results on actual AQI index versus the change on various factors
    * Analyzing on case-by-case basis per pollutant is necessary to understand trends and how factors such as laws may affect pollution
* Awareness of air pollution is one big factor in the slow decline in some pollutants

###### <sup>1</sup>  In comparison to other existing datasets
