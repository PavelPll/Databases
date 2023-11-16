# OBJECTIVE: Create AWS S3 bucket and use it for ETL Spark project.
## Create AWS S3 bucket
AWS S3 bucket can be created directly using AWS account. Another option, I am using here, is the creation of the bucket directly from the code using the class [AmazonS3Client](https://docs.aws.amazon.com/AWSJavaSDK/latest/javadoc/com/amazonaws/services/s3/AmazonS3Client.html). In order to get the required AWS_ACCESS_KEY and AWS_SECRET_KEY one has to create new IAM (Identity and Access Management) user in AWS account. 



The file **SQL_server_installation.txt** describes the installation procedure. I used this postreSQL server for
* Extract Transfer Load (ETL) Spark pipeline (for details see [toSQL.scala](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Scala_ETL/toSQL.scala)).  
* For Spark streaming (for details see [toSQLstreaming.scala](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Streaming/src/main/scala/toSQLstreaming.scala)).
> [!NOTE]
> For Hadoop Hive project I used Derby database. It is also possible to use postreSQL instead of Derby for this purpose. I put the corresponding notes in (8) in [hive_installation.txt](https://github.com/PavelPll/Hadoop-Hive/blob/main/hive_installation.txt).
