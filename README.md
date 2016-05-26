# Analysing_logs

Analyzing Logs Using certain open source tools for building any infrastructure for managing logs and for real time Analytics using tools. In this infrastructure we are using certain tools by which we can manage any live logs generated on any servers (i.e. website logs or system logs).

Any organization requires growing their business by means any media, that can be easily done by analyzing logs, such as click stream data or where are customers clicking on site or which particular browser they are using.
A log file is a file that records either event that occurs in an operating system or other software runs, or messages between different users of a communication software. 

Data constantly flows into your systems, but it can quickly grow to be fat and stale. As your data set grows larger, your analytics will slow up, resulting in sluggish insights. And this is likely to be a serious business problem. 

## Motivation

This Infrastructure is based on solving the basic needs for data flow at the backend in any organization. 


## Components 
 - [Elasticsearch](https://www.elastic.co/products/elasticsearch)
  Elasticsearch is a search server based on Lucene. It provides a distributed, multitenant-capable full-text search engine with an HTTP web interface and schema-free JSON documents. Elasticsearch is developed in Java and is released as open source under the terms of the Apache License

   - [More Elasticsearch](https://github.com/elastic/elasticsearch)

- [HDFS](hortonworks.com/apache/hdfs/) 
  HDFS is a Java-based file system that provides scalable and reliable data storage, and it was designed to span large clusters of commodity servers. HDFS has demonstrated production scalability of up to 200 PB of storage and a single cluster of 4500 servers, supporting close to a billion files and blocks.
    
   - [Mirror of Hadoop HDFS](https://github.com/apache/hadoop-hdfs)
   
- [Kafka](http://kafka.apache.org/)
  Apache Kafka is publish-subscribe messaging rethought as a distributed commit log.

- [Cassandra](http://cassandra.apache.org/) 
  Apache Cassandra is a free and open-source distributed database management system designed to handle large amounts of data across many commodity servers, providing high availability with no single point of failure.

- [Logstash](https://www.elastic.co/products/logstash)  
  Logstash is an open source tool for collecting, parsing, and storing logs for future use. Kibana 3 is a web interface that can be used to search and view the logs that Logstash has indexed. Both of these tools are based on Elasticsearch. Elasticsearch, Logstash, and Kibana, when used together is known as an ELK stack.

- [Logstash Forwarder](https://github.com/elastic/logstash-forwarder)
  Filebeat is a lightweight, open source shipper for logs. It replaces the Logstash Forwarder or Lumberjack. It can tail logs, manages log rotation and can send log data on to Logstash or even directly to Elasticsearch. Filebeat is part of a larger collection of data shipping tools called Beats.

- [Kibana](https://www.elastic.co/products/kibana)
  Kibana is an open source data visualization plugin for Elasticsearch. It provides visualization capabilities on top of the content indexed on an Elasticsearch cluster. Users can create bar, line and scatter plots, or pie charts and maps on top of large volumes of data.

## [Introduction to ELK Stack](https://www.elastic.co/webinars/introduction-elk-stack)
By combining the massively popular Elasticsearch, Logstash and Kibana, Elastic has created an end-to-end stack that delivers actionable insights in real time from almost any type of structured and unstructured data source. 

Built and supported by the engineers behind each of these open source products, the Elastic Stack makes searching and analyzing data easier than ever before. 

Thousands of organizations worldwide use these products for an endless variety of business critical functions.





## Integrating 

Logstash Forwarder agent (On servers) => Kafka => HDFS/ [Cassandra => Storm or Spark] => Logstash => Elasticsearch => Kibana 


## Visualizations

- [Working with Kibana](https://www.elastic.co/guide/en/kibana/current/getting-started.html)
- Some Visualizatons


![Sample Image Kibana](https://github.com/prateeknepaliya09/Analysing_logs/blob/master/images/images.png?raw=true)

![Sample Image Kibana](https://github.com/prateeknepaliya09/Analysing_logs/blob/master/images/setupkibana2.png?raw=true)
  
![Sample gif](https://github.com/prateeknepaliya09/Analysing_logs/blob/master/images/1-discover.gif?raw=true)

