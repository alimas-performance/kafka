# Kafka Project

### Scope

1. Generate Theory documentation about Kafka 
2. Generate Theory documentation about Performance Observations and Improvements when perf testing kafka
3. Deploy Kafka in Test Servers
4. Document how to deploy kafka locally 
5. Develop a basic consumer/ producer flow and setup kafka for that
6. Create JMeter script to test that
7. Create slides for Use Case Demo
8. Improve with Monitoring points using Grafana, Premethous and InflixDB

### Kafka Notes

**Broker**: Is the kafka server can be a VM, this contains **queues**

**Partition**: The **queue**. Ordered immutable sequence of messages that we append to a **log** file. Each Broker can have multiple partitions

**Topic**: A Logical way to **group** **partitions/queues**. You publish to and consume from topics in Kafka.

**Producers**: **Writes** messages to a **topics**.

**Consumers**: **Reads** messages from **topics**.

![image-20240815174051743](C:\Users\Angel\AppData\Roaming\Typora\typora-user-images\image-20240815174051743.png)

