# References:

### Concepts

- [General concepts explanation](https://youtu.be/DU8o-OTeoCc)
- [Zookeeper Navigator](https://zoonavigator.elkozmon.com/en/docs-pre-v1/quickstart.html)
- [Zookeeper Docker Samples](https://hub.docker.com/r/bitnami/kafka/)
- [Kafka UI](https://docs.kafka-ui.provectus.io/overview/getting-started)
- [Kafka Repo Doc](https://github.com/bitnami/containers/blob/main/bitnami/kafka/README.md)
- [Auth documentation 1](https://github.com/wurstmeister/kafka-docker/issues/532)
- [Script to create the JKS and PEM files](https://github.com/jaehyeon-kim/kafka-pocs/blob/main/kafka-dev-with-docker/part-10/generate.sh)
- [Article about Kafka Auth](https://jaehyeon.me/blog/2023-07-13-kafka-development-with-docker-part-10/) and also [this article series](https://jaehyeon.me/series/kafka-development-with-docker/) 
- [Generate JKS for kafka](https://docs.cloudera.com/runtime/7.2.0/kafka-securing/topics/kafka-secure-create-ca.html) 
- [Plain auth kafka configuration](https://codeforgeek.com/how-to-set-up-authentication-in-kafka-cluster/)

# Deploy

It was used the file named `kafka-and-ui.yaml` which contains a kafka server and a kafka server ui to administrate it. 



### Configuration

To configure the Kafka cluster in the web ui, it was used the following information:

- local IP host where the apache server was created
- default port used when installing kafka (9092)

### Certificate Setup

- Get into a Linux System like Ubuntu
- Install or make sure it is installed JRE 21+
  - `sudo apt install openjdk-21-jre-headless`
- Install or make sure it is installed the OpenSSL tools
- Copy the script located in this [Link](https://github.com/jaehyeon-kim/kafka-pocs/blob/main/kafka-dev-with-docker/part-10/generate.sh) in the Linux machine
- make the script file *.sh executable
  - `chmod +x generate.sh`
- create a file named kafka-hosts.txt and make sure to have the IP of the kafka server there
- Execute the generate.sh script
  - `./generate.sh`



[^Note]: localhost hostname doesn't work





