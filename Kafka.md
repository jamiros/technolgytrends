* Kafka is a **distributed streaming platform that is used publish and subscribe to streams of records.** 
* Kafka is used for fault tolerant storage. 
* Kafka replicates topic log partitions to multiple servers. 
* Kafka is designed to allow your apps to process records as they occur
* Kafka itself is completely free and open source. Confluent is the for profit company by the creators of Kafka.
* Netflix embraces Apache Kafka® as the de-facto standard for its eventing, messaging, and stream processing needs. ... It provides us with the high durability and linearly scalable, multi-tenant architecture required for operating systems at Netflix.
* **topics in Kafka are retention based**: messages are retained for some configurable amount of time. ... It's worth noting that this is an **asynchronous process**, so a compacted topic may contain some superseded messages, which are waiting to be compacted away. Compacted topics let us make a couple of optimisations.
* AWS also offers Amazon MSK, the most compatible, available, and secure fully managed service for Apache Kafka, enabling customers to populate data lakes, stream changes to and from databases, and power machine learning and analytics applications.
* When you can lose messages in Kafka. Kafka is speedy and fault-tolerant distributed streaming platform. However, there are some situations when messages can disappear. It can happen due to misconfiguration or misunderstanding Kafka's internals.
* What happens when a Kafka broker goes down?
Kafka does not create a new replica when a broker goes down. ... If the offline broker was a follower, it will be marked a out of sync by the leader. When restarting the broker, it will try to get back in sync. Once done, whether it stays a follower or becomes the leader depends if it is the prefered replica.