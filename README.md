# Climate Data Store (CDS) by COPERNICUS

The Climate Data Store (CDS) by Copernicus provides free access to a wide range of environmental data for use in climate and weather research, forecasting, and decision-making. You can access it [here](https://cds.climate.copernicus.eu/datasets). There's a companion to *CDS* called *Atmosphere Data Store (ADS)* focused more on atmosphere and air quality monitoring - you can access it [here](https://ads.atmosphere.copernicus.eu/user-guide).

The CDS is a service of the Copernicus Climate Change Service (C3S) and provides:
	- Datasets: Historical, real-time, and forecasted climate data.
	- Tools: APIs, web interfaces, and ready-to-use scripts for data access and analysis.
	-	Applications: User-friendly widgets and workflows for data visualization and decision-making.

It covers domains like:
	-	Temperature, precipitation, and extreme weather trends.
	-	Ocean conditions, sea level, and ice coverage.
	-	Energy, agriculture, and health impact modeling.

In this project the I:
  1. Export data about temperature from CDS with the largest resolution possible (i.e. smaller grid), filter it to fit Portugal geographical region.
  2. Combine the different exports into a single ```xarray```.
  3. To obtain a temperature summary variable for each municipality in Mainland Portugal, I used a municipality ```shapefile``` to be defining border region. Each datapoint that is contained in a municipality polygon contributes to the average temperature computed for that polygon. I created my own code just for this purpose.
  4. Performed some EDA and map representions.

![Average Temperature on August 15th 2018 across Mainland Portugal](https://github.com/andrebrito0/climate_data_store/blob/main/mean%20temperature.png)


 
