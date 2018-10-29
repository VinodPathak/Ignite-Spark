<b>1.  Create a SparkSession object using Pyspark</b>  
  
from pyspark.sql import SparkSession  
spark = SprakSession.builder.master("local").getOrCreate()
