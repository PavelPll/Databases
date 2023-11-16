# OBJECTIVE: Create AWS S3 bucket and use it for ETL Spark project.
## Create AWS S3 bucket
AWS S3 bucket can be created directly using AWS account. Another option, I am using [here](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Scala_ETL/toS3bucket.scala) (or see **toS3bucket.scala**), is the creation of the bucket directly from the code using the class [AmazonS3Client](https://docs.aws.amazon.com/AWSJavaSDK/latest/javadoc/com/amazonaws/services/s3/AmazonS3Client.html). In order to get the required AWS_ACCESS_KEY and AWS_SECRET_KEY one has to create new IAM (Identity and Access Management) user in AWS account. Choose "Attach policies directly" then "AmazonS3FullAccess" then press "Create user". After user is created go to his "Security Credentials" and press "Create access key" for "Applications running outside AWS". Two libraries aws-java-sdk-bundle and hadoop-aws need to be added (to build.sbt file  and to spark-shell/spark-submit after "--packages"). Check if all hadoop-* libraries have the same version (3.3.1 in my case) to avoid multple ClassNotFoundException etc. 





The file **SQL_server_installation.txt** describes the installation procedure. I used this postreSQL server for
* Extract Transfer Load (ETL) Spark pipeline (for details see [toSQL.scala](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Scala_ETL/toSQL.scala)).  
* For Spark streaming (for details see [toSQLstreaming.scala](https://github.com/PavelPll/Spark-ETL-ML/blob/main/Streaming/src/main/scala/toSQLstreaming.scala)).
> [!NOTE]
> For Hadoop Hive project I used Derby database. It is also possible to use postreSQL instead of Derby for this purpose. I put the corresponding notes in (8) in [hive_installation.txt](https://github.com/PavelPll/Hadoop-Hive/blob/main/hive_installation.txt).
