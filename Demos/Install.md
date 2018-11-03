### Installed jre 1.8 64 bit  
JAVA_HOME : C:\Java\jre1.8.0_191;  
Path:- "%JAVA_HOME%\bin"  
_JAVA_OPTIONS = -Xms2048m -Xmx4096m -XX:MaxPermSize=1024m  

### Setup Winutils and Env  
HADOOP_HOME = C:\hadoop  
Path = %HADOOP_HOME%\bin  

### Links  
https://stackoverflow.com/questions/33734210/system-cannot-find-the-path-specified-in-spark-shell  
https://jaceklaskowski.gitbooks.io/mastering-apache-spark/spark-tips-and-tricks-running-spark-windows.html  



### Read Data:  
df = spark.read.options(header=True, inferSchema=True, delimiter= ',').csv("F:\\Analytics\\Datasets\\hacker-news-corpus\\hacker_news_sample.csv")  

### Spark Memory Issues:  
https://github.com/rstudio/sparklyr/issues/321  
https://stackoverflow.com/questions/27152429/spark-installation-memory-issues  
