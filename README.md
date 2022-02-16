# SPA
This repositary contains case study for smart process analysis as part of final assignment.

## About Logs:
* Processing the log file from Dutch municipalities released in 2015.
* In Netherland, a permit is required when citizens wish to do anything with their land like constructing a new building or demolishing building, cutting a tree etc.
* This process from requesting for a permit to receiving the permit is recorded in the log file.
* Data analysis is performed using Disco and Celonis tools


## Steps followed to process Log:
* Data Analysis: 
  * Converted log file format from XES to csv using python
  * Log file consists of Log file consists of 52217 Events, 811 cases and 289 activities
* Filters log data:
  * Performance: Maximum duration 80 days, covered 81% of cases.
  * EndPoints:
    * Start event values: Register submission date request
    * End event values: Enter send date acknowledgement
 
This process finally produce .pnml file which is then fed as an input to python code which attempts to predict the probability of next event.
