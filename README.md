# Kafka-Producer-Consumer-Spring-Boot-Microservices

# Command to Start Kafka Server: 
Cluster ID: <"Generated UUID">
C:\kafka\bin>windows\kafka-storage.bat random-uuid

.\bin\windows\kafka-storage.bat format --standalone -t <"Generated UUID"> -c config\server.properties

# Start a Kafka Server
.\bin\windows\kafka-server-start.bat .\config\server.properties

# Create a topic:
.\bin\windows\kafka-topics.bat --create --topic test-topic --bootstrap-server localhost:9092

# List the topics:
.\bin\windows\kafka-topics.bat --list --bootstrap-server localhost:9092

# Start a console consumer:
.\bin\windows\kafka-console-consumer.bat --topic test-topic --from-beginning --bootstrap-server localhost:9092

# Start a console producer:
.\bin\windows\kafka-console-producer.bat --topic test-topic --bootstrap-server localhost:9092

# Press Ctrl + C inorder to stop the above processes

# To Test a Producer:
.\bin\windows\kafka-console-consumer.bat --topic location-update-topic --from-beginning --bootstrap-server localhost:9092
