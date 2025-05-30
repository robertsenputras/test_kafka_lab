
## Getting started
- Clone the starter code from this Git repository.
- The repository includes a python notebook for Kafka producer and consumer model.

## Connecting to Kafka server
1. Use SSH to create a tunnel to the Kafka server (find remote_server, user, and password on the Canvas entry for this lab):  
   `ssh -L <local_port>:localhost:<remote_port> <user>@<remote_server> -NTf`
2. Test the Kafka server connection to ensure it's operational.

## Implementing Producer-Consumer Mode
### 1. Producer Mode: Writes Data to Broker
Refer TODO sections in the script. Edit the bootstrap servers and add 2-3 cities of your choice. Run the code to write to Kafka stream.

### 2. Consumer Mode: Reads Data from Broker
Modify the TODO section by filling appropriate parameters/arguments in the starter code. Verify `Kafka_log.csv`.  

Ref:  
[KafkaProducer Documentation](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaProducer.html)  
[KafkaConsumer Documentation](https://kafka-python.readthedocs.io/en/master/apidoc/KafkaConsumer.html)

## Using Kafka’s CLI tools
`kcat` is a CLI (Command Line Interface). Previously known as kafkacat.  
Install with your package installer such as:
- macOS: `brew install kcat`
- Ubuntu: `apt-get install kcat`
- Note for Windows Users: Setting up kcat on Windows is complex. Please work in pairs with someone with mac/Ubuntu during recitation for this deliverable. The purpose is to understand CLI which will be helpful in the group project for using Kafka on Virtual machines (Linux based).

Using the kcat documentation, write a command that connects to the local Kafka broker, specifies a topic, and consumes messages from the earliest offset. 

Ref:\
  [kcat usage](https://docs.confluent.io/platform/current/app-development/kafkacat-usage.html)  
  [kcat GitHub](https://github.com/edenhill/kcat)   

## Additional resources
- [Kafka Introduction Video 1](https://www.youtube.com/watch?v=PzPXRmVHMxI) <- Recommended video for a quick 5-min introduction to Kafka
- [Kafka Introduction Video 2](https://www.youtube.com/watch?v=JalUUBKdcA0)
- [Apache Kafka](https://kafka.apache.org/)
- [Kafka for Beginners](https://www.cloudkarafka.com/blog/2016-11-30-part1-kafka-for-beginners-what-is-apache-kafka.html)
- [What is Apache Kafka? - TIBCO](https://www.tibco.com/reference-center/what-is-apache-kafka)
- [frequent bug list and solutions](./bug_list.md)


