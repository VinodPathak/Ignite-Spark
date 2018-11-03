### Installed jre 1.8 64 bit  
JAVA_HOME : C:\Java\jre1.8.0_191;  
Path:- "%JAVA_HOME%\bin"  
_JAVA_OPTIONS = -Xms2048m -Xmx4096m  

Setup Winutils  
winutils - https://github.com/steveloughran/winutils/blob/master/hadoop-2.6.0/bin/winutils.exe  
HADOOP_HOME = C:\hadoop  
Path = %HADOOP_HOME%\bin  

### Links:  
* https://stackoverflow.com/questions/33734210/system-cannot-find-the-path-specified-in-spark-shell  
* https://jaceklaskowski.gitbooks.io/mastering-apache-spark/spark-tips-and-tricks-running-spark-windows.html  


### Run Pyspark with configurations  
pyspark --master local[8]    

### Read Data:  
df = spark.read.options(header=True, inferSchema=True, delimiter= ',').csv("F:\\Analytics\\Datasets\\hacker-news-corpus\\hacker_news_sample.csv")  
df = spark.read.options(header=True, inferSchema=True, delimiter= ',').csv("F:\\Analytics\\Datasets\\consumercomplaints\\consumer_complaints.csv")  
df = spark.read.options(header=True, inferSchema=True, delimiter= ',').csv("F:\\Analytics\\Datasets\\acquire value shoppers challenge\\transactions.csv")  
df = spark.read.options(header=True, schema=myschema, delimiter= ',').csv("F:\\Analytics\\Datasets\\acquire value shoppers challenge\\transactions.csv")  

### Spark Memory Issues   
https://github.com/rstudio/sparklyr/issues/321  
https://stackoverflow.com/questions/27152429/spark-installation-memory-issues  

### import methods
from pyspark.sql.types import StructType, StructField, StringType, FloatType, IntegerType  

### Define Schema
myschema = StructType([\  
StructField("id",StringType(),True),\  
StructField("chain",StringType(),True),\  
StructField("dept",StringType(),True),\  
StructField("category",StringType(),True),\  
StructField("company",StringType(),True),\  
StructField("brand",StringType(),True),\  
StructField("date",StringType(),True),\  
StructField("productsize",StringType(),True),\  
StructField("productmeasure",StringType(),True),\  
StructField("purchasequantity",IntegerType(),True),\  
StructField("purchaseamount",IntegerType(),True)])  



(2.1 + ex) = 0.6 * heap
