# final-project-spider-man
final-project-spider-man created by GitHub Classroom

There are 2 overarching datasets. 
The first dataset is a collection of the LA Metro Bike Share data which is in the "BikeShare" folder.
The second dataset is the LA Metro Bus data that I attained from the LA Metro API ("LAMetro_bus_data.csv").

---

The Bike share data contains the following: 
  duration of the ride, the start and end time, the start and end longitude and latitude, etc.
The Bus data contains the following:
  grouped time (the time the set of buses was collected),
  actual time (the time the single bus was collected),
  last report (the last time the bus reported to the server in seconds),
  id (the bus's unique id),
  route (the bus's current route),
  latitude,
  longitude,
  run (the direction and destination of the bus)
  
---  
  
Running the API (LA Metro API.ipynb)
  Run the first code block which will import the libraries and initialize the variables.
  Then next code block will grab the data.
    The only code that needs to be adjusted is the time (t_end).
    It is in the format (seconds * minutes * hours) so adjust it accordingly.
    Once the desired time is set, run the code.
  The next block of code just shows the dtypes, so run it if you want.
  There now two blocks of code left.
    (1) The first block will save the df to a csv (LAMetro_bus_data).
          Run this if you want to create a csv file.
    (2) The second block will append the df to a csv ("").
          Run this if you have already created the csv file (the first block), and want to continue appending data.
  This is the end. Start from the beginning if you want to grab more data.
  It is necessary to start over so the df can be reset. Thus, redundant data will not be appended to the csv.
  
---
  
Running the Bike Station Visualizations (Bike Stations Visualizations.ipynb)
