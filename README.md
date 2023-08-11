# GDELT Data Analysis in DataBricks

Explore empathetic comments' origins using GDELT data from GDELT Project via DataBricks. Importing a substantial GCP dataset, we employed Spark and Python for data cleaning. Visualized geographical insights with scatter plots of latitudes and longitudes, optimizing performance with caching. Proficiency in Spark and big data demonstrated while handling large datasets up to several gigabytes.

## Cluster Setting:
Multi Node, No Isolation Shared
Runtime: 11.0
Worker/Driver Type: e2-highmem-2
(Min Workers: 1, Max Workers: 6 with autoscaling)

## Code Optimization:
Efficiency measures included specifying executor and driver memory at two gigabytes. Utilized cache() function on the RDD. Employed reduceByKey() over groupByKey() where feasible.

## Objectives:
Leveraged the event database to identify likely event occurrences. Visualized event frequency by location and time, identifying common event types in specific regions.

## Input Data:
Inputs read from GCP bucket: "GDELT.MASTERREDUCEDV2.TXT"
Website origin of data: https://www.gdeltproject.org/

## Key Code Snippets:

Data parsing and transformation using Python and Spark RDDs.
Utilized functions for column retrieval, timestamp conversion, and data type conversion.
For detailed code and visualizations, refer to the notebook.
