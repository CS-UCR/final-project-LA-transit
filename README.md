# Phase 1
For the project, I plan map the LA Metro Bus system in "real-time" using publicly available data. I will also analyze the LA Metro Bike Share System and map trips to and from destinations. Through this hands-on project, I hope to get more experience with GIS and transit data.

# Phase 2

## Datasets
2 datasets being used in the project. 
- The first dataset is a collection of the LA Metro Bike Share data which is in the "BikeShare" folder. I took one portion of the data (from Q1 2020) and clean it into "2020 Q1 Cleaned Bike Data.csv". It has about 70,000 rows.
- The second dataset is the LA Metro Bus data that I attained from the LA Metro API ("LA Metro Bus Data.csv"). It is then cleaned. This set has about 500,000 rows.

---

## What the datasets contain
- The Bike share data contains the following: 
  - duration of the ride (in minute)
  - the start and end time
  - start and end longitude and latitude
  - start station and end station
  - bike type
- The Bus data contains the following:
  - grouped time (the time the set of buses was collected)
  - actual time (the time the single bus was collected)
  - last report (the last time the bus reported to the server in seconds)
  - id (the bus's unique id)
  - route (the bus's current route)
  - latitude
  - longitude
  - run (the direction and destination of the bus)
  
---  

## Bus: API, Cleaning, EDA, and Visualization
- (LA Metro API.ipynb, LA Metro Bus Cleaning.ipynb, LA Metro Bus EDA & Visualizaiton.ipynb)
- Running the API
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
  - *Note:* The csv is too big, so only a portion of the data has been uploaded to github
  
---

## Bikeshare: Cleaning, EDA, and Visualization
- LA Metro Bike Share - (LA Metro Bike Share Cleaning.ipynb, LA Metro Bike Share EDA & Visualization.ipynb)
  - Run the LA Metro Bike Share Cleaning.ipynb and follow the instructions.
    - Here I clean the data and prep it for EDA and Visualization
  - Then open LA Metro Bike Share EDA & Visualization and follow the instructions
    - In this section I show the arrival & departures and denisty maps for the LA Metro Bike Share System
    
---

# Phase 3
- Phase 3 is split between the LA Metro Bus EDA & Visualization and LA Metro Bike Share EDA & Visualization
- I used the LA Metro API and LA Metro Bike Share Dataset
- Questions about BikeShare:
  - How many people are riding the bikes?
  - What is the most common pass type?
  - Where are most bikers going?
  - What are the most popular stations?
- Questions about the bus system:
  - What are the most popular buses?
  - Where are most people going?
  - How does bus density change with the day or time?
