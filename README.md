## Micro Services Design Pattern — **AAA BBB CCC DES SSS** – (A3 B3 C3 DES S3)

* **API Gateway**: It acts as a single point of entry to a system.<br />
* **Ambassador**: A way to expose microservice architecture to outside world by using single gateway that proxies requests to individual microservices.<br />
* **Aggregator**: Allow to collect data from multiple sources and then aggregate it into a single result. Eg: Flipkart Search=rating+comments+feedback<br />
* **BFF -Backend For Frontend**: It allows to create separate backends for different frontends.<br />
* **Blue/Green Deployment**: It allows to deploy new versions of your application without any downtime. Blue - Prod version and Green - New version.<br />
* **Bulkhead**: Isolate different parts of application from each other to failure, performance & security Isolation and minimizing the impact of failures.<br />
* **Caching Pattern**: It storing and using a precomputed most frequently used value for expensive calculations again and again.<br />
* **CQRS-CMD & Query Responsibility Segregation**: Separates reading (query) and writing (Cmd) of an application's data model. Make things faster.<br />
* **Circuit breaker**: Make fault tolerance system, prevents continuous attempts to access a fail service. Improve performance by open/close circuit.<br />
* **DDD-Domain driven design**: Deal with large models by dividing them into different bounded context i.e. sales, order and payment processing.<br />
* **EDD-Event Driven Design**: It focuses on asynchronous communication between microservices through the use of events. i.e. Kafka, RabbitMQ.<br />
* **Saga**: A way to manage complex, long-running transactions or processes in a distributed system by breaking into smaller, more manageable steps.<br />
 * **1. Choreography**- All services of the distributed transaction, publish a new event after success or failure & inform to next (S) or previous(F) Saga.<br />
 * **2. Orchestration**- A single orchestrator (arranger) manages all transactions and directs services to execute local transactions.Eg Camel, Mulesoft<br />
* **Strangler**: A way to replace old (monolithic) system without disrupting existing system to a new microservice system in gradual approach. <br />
* **Sidecar**: Approach where separate sidecar service is paired with main application, handling supportive tasks like logging, security, communication.<br />
* **Service Discovery**: Allows you to dynamically discover the services at runtime and communicate with the services without hard coded URLs. i.e. Consul and Netflix Eureka.<br />
* **Database per Service**: Allow to create database for each microservices <br /><br />

**Deployment Strategies**: **Blue/Green**:Switching between the current production version and a new version, **Canary**:Deploy new version to small users(10%), **A/B Testing**: Deploys two versions & test(TogglZ), Shadow Deployment, Feature Toggle Deployment(Togglz library Spring Boot).
