# OBJECTIVE: Create AWS S3 bucket and use it for ETL Spark project.
AWS S3 bucket can be created directly using AWS console. 
The file **SQL_server_installation.txt** describes the installation procedure. I used this postreSQL server for
* Extract Transfer Load (ETL) Spark pipeline (for details see [toSQL.scala](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Scala_ETL/toSQL.scala)).  
* For Spark streaming (for details see [toSQLstreaming.scala](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Streaming/src/main/scala/toSQLstreaming.scala)).
> [!NOTE]
> For Hadoop Hive project I used Derby database. It is also possible to use postreSQL instead of Derby for this purpose. I put the corresponding notes in (8) in [hive_installation.txt](https://github.com/PavelPll/Hadoop-Hive/blob/main/hive_installation.txt).
