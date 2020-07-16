# spark_streaming_with_twitter_and_kafka_TFIDF_sentiment_analysis
spark streaming with twitter and kafka producing TFIDF sentiment analysis

# Purpose:
- use twitter as producer to ingest tweets to be used by spark streaming 
- create object class to be the producer for kafka using spark.
- train a TFIDF algorithm using Virgin Airlines tweets for sentiment analysis and use in spark streaming for predictions.
- push the sentiment analysis to kafka as consumer.

# Requirements:
- Spark installed
- Kafka library installled

# Objective :
- use twitter as producer to generate input data to be consumed be spark streaming.
- implement some logic inside the spark to consume data from twitter, process data, and send results to kafka.
- use object class in spark to be the engine to send results back to kakfa.

# To run Spark :
- start-dfs.sh      # start the hadoop daemons
- start-master.sh   # start the spark cluster master 
- start-slaves.sh   # start the spark cluster slaves
- spark-shell --master spark://spkm:7077 --jars KfkProducer/target/scala-2.11/kfk-producer_2.11-1.0.0.jar   # have the kfk-producer compiled to be used as producer to kafka