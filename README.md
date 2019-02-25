# ProcessCsvFileUsingPySpark
Take advantage of spark DataFrame to filter a large .csv file.

This notebook does following - 

1. Read Events from a Big File using pySpark
2. Remove the unwanted events using Spark DataFrame APIs
3. Add new column to represent EPOCH time
4. ==> Following doesn't work now, proabably, as I have used spark 2.3 with java 11, So use Spark itself to write the out file
     # (Convert filtered list to a pandas dataframe => Spark dataframe.write.csv write operation writes segmented files. So, let us use pandas.)
     # 5. Write the padas dataframe to the .csv file=> This will be a smaller file in comparison to the raw file and will be used for further processing.
