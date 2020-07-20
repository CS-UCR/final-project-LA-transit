# Phase 2

## Datasets
There are 2 overarching datasets. 
The first dataset is a collection of the LA Metro Bike Share data which is in the "BikeShare" folder. I take one portion of the data and clean it into "2020 Q1 Cleaned Bike Data.csv".
The second dataset is the LA Metro Bus data that I attained from the LA Metro API ("LAMetro_bus_data.csv").

---

## What the datasets contain
- The Bike share data contains the following: 
  - duration of the ride, the start and end time, the start and end longitude and latitude, etc.
- The Bus data contains the following:
  - grouped time (the time the set of buses was collected),
  - actual time (the time the single bus was collected),
  - last report (the last time the bus reported to the server in seconds),
  - id (the bus's unique id),
  - route (the bus's current route),
  - latitude,
  - longitude,
  - run (the direction and destination of the bus)
  
---  

## Bus Data and API
- Running the API - (LA Metro API.ipynb)
  - Run the first code block which will import the libraries and initialize the variables.
  - Then next code block will grab the data.
    - The only code that needs to be adjusted is the time (t_end).
    - It is in the format (seconds * minutes * hours) so adjust it accordingly.
    - Once the desired time is set, run the code.
  - The next block of code just shows the dtypes, so run it if you want.
  - There now two blocks of code left.
    - (1) The first block will save the df to a csv (LAMetro_bus_data). Run this if you want to create a csv file.
    - (2) The second block will append the df to the csv (LAMetro_bus_data). Run this if you have already created the csv file (the first block), and want to continue appending data.
  - This is the end. Start from the beginning if you want to grab more data.
  - It is necessary to start over so the df can be reset. Thus, redundant data will not be appended to the csv.
  - Instructions for this are also in the notebook
  
---

## Bikeshare: Cleaning, EDA, and Visualization
- LA Metro Bike Share - (LA Metro Bike Share Cleaning.ipynb, LA Metro Bike Share EDA.ipynb, LA Metro Bike Share Visualizaiton.ipynb)
  - Run the LA Metro Bike Share Cleaning.ipynb and follow the instructions.
    - Here I clean the data and prep it for the visualization
  - Then open LA Metro Bike Share EDA and follow the instructions
    - After, I quickly go over the EDA before the visualization portion
  - Lastly, open the LA Metro Bike Share Visualization and follow the instructions.
    - In this section I show the arrival and departures for the LA Metro Bike Share System
