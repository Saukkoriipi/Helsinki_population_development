## Population in Helsinki metropolitan area years 1997 to 2019

### Introduction
Tekstiä....

### Results

Results page can be found from the link bellow
[Link to Stations population 1997 to 2019](https://saukkoriipi.github.io/StationsPopulation/)



## Guide to notebooks

### Use following sequence when running the notebooks

###### First use following notebooks to clean and modify data
1. CreatePopulation.ipynb
2. CreateStations.ipynb
3. GetRailsData.ipynb
4. CreatStationsPopulation.ipynb
###### Then visualize cleaned data
5. CreatePicsPopByStation.ipynb
6. CreatePicsPopulation.ipynb
7. CreatePicsStationsPopulation.ipynb
8. CreateGifs.ipynb
9. CreateBokeh.ipynb

### Introduction to notebooks

##### CreatePopulation.ipynb
Read population data from folder population_data, join tables and save result as shapefile in same folder.

##### CreateStations.ipynb
Read stations data from folder stations_data, clean data and save result as shapefile to same folder.

##### GetRailsData.ipynb
Get rails data from osmnx, then filter rails only to cover area with stations and save result to railway_data as shapefile.

##### CreateStationsPopulation.ipynb
Reads population and station data. Creates 500 meters buffer around stations, then calculates population size for every station and year and saves result to population_data folder as station_population shapefile.

##### CreatePicsPopByStation.ipynb
Reads stations_population data and creates graphs for every station. Result is saved in folder pics_stations_graphs.

##### CreatePicsPopulation.ipynb
Reads population, railways and stations data and creates map figure for every year. Result is saved in folder pics_all_population.

##### CreatePicsStationsPopulation.ipynb
Reads stations_population, railways and stations data and creates map figure for every year. Result is saved in folder pics_stations_population.

##### CreateGifs.ipynb
Create gif animations of images in folders pics_all_population, pics_stations_graphs and pics_stations_population. GIF animations are saved in folder docs.

##### CreateBokeh.ipynb
Create interactive Bokeh map visualization. Read stations_population, railways and stations data and creates bokeh map. Result is saved in folder docs with name StationsPopulation.html.