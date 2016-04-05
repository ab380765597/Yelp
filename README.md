
# YelpDataAnalysis-
Use hadoop to analysis yelp customer data
This is a project to read the original data from Yelp in JSON and ELT data using MR.

The process to run this project:
go to the file in console

mvn clean
mvn package
hadoop -dir /user/cloudera/Yelp/input/1
hadoop -put Yelp_training_set_data.json /user/cloudera/Yelp/input/1
hadoop -dir /user/cloudera/Yelp/output/1
hadoop jar target/YelpProject-0.0.1-SNAPSHOT.jar MapReduce.Demo /user/cloudera/YelpProject/input/3 /user/cloudera/YelpProject/output/26
hadoop fs -cat /user/cloudera/Yelp/output/1/*


