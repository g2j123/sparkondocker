# sparkondocker


docker build --rm -t sparkondocker/spark:1.6.0 .

docker run -it -p 8088:8088 -p 8042:8042 -p 4040:4040 -h sandbox sparkondocker/spark:1.6.0 bash





--running spark
 spark-submit --class org.apache.spark.examples.SparkPi --files $SPARK_HOME/conf/metrics.properties --master yarn-cluster --driver-memory 1g --executor-memory 1g --executor-cores 1 $SPARK_HOME/lib/spark-examples-1.6.0-hadoop2.6.0.jar
