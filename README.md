# Home-Sales

In this project, I was tasked to use SparkSQL to determine key metrics about a home sales data set. 

I used Spark to create a temporary view from which I could run the SQL queries needed to extract information from the data set.

I also attempted various ways of running the SQL queries, measuring run time of running the query from the temporary view alone and from a cached version of the temporary view. I also partitioned the data set by writing the dataframe to parquet format and running the query from that file as well.

The quickest run time was the cached version of the temporary view at 0.12479305267333984 seconds. The next quickest was from the original temporary view with a run time of 0.17152905464172363. Finally the parquet read query ran the slowest at 0.26303720474243164 seconds. Comparing these strategies and run times help outline the most efficient process for running the query and returning the desired information.