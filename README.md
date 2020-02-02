Requirements
The following are the considerations that we had for selecting the language

**Comparing use cases**

    1.RESTful APIs. (Preferably with options to generate server code from Swagger spec)
    2.Consuming messages from one of the queues/streams like Kafka, SQS

**Working with following resources**

    1.MySQL
    2.Consuming and Producing messages from/to Kafka at high volume
    3.Consuming and Producing messages from/to SQS
    4.Redis
    5.DynamoDB
    6.Calling other internal and external RESTful APIs. Preferably option to generate client code from Swagger spec.
    7.SDK for other AWS services
**Performance**

    1.Latency for RESTful API services
    2.Throughput for stream consumer
    3.Memory footprint
**DevOps**

    1.Monitoring
    2.Dockerization
**Developer productivity**

    1.Language features
    2.Available talent pool and trainability
    3.IDE
    4.Formatting
    5.Static code analyzers
    6.Readability and maintainability of existing code
    7.Code-test cycle

# Go-Java
decider points to use go and java


**1. Developer productivity**:

Go language syntax very simple. This means that the Go syntax and its core concepts can be learnt pretty quickly.

Java has added huge number of features, syntactic sugar, concurrency libraries.
Hence, the complexity of learning the language has increased.Learning all the nitty-gritty of implementing concurrent processing right takes a lot of effort.
On top of these, other mostly defacto frameworks like Spring, Hibernate, SpringMVC/Jersey, Jetty/Tomcat, makes the learning go for a very long time.
On the other hand, once these frameworks/libraries/features are learnt, they provide a lot of productivity boost as they take care of a lot of complexities underneath.

**2. Performance**:

The memory footprint of Go is much much smaller than Java. In our Go based real-time notification server, some of the services are running with around 70 MB of memory per process in production.

With Java, pretty much nothing runs for less than 512 MB of memory. This is especially beneficial with docker allowing multiple services running on the same machine.
