# MSA

## MSA 의 SOAP 인터페이스와 WSDL 이란?

MSA (Microsoft Specific Architecture) 의 SOAP (Simple Object Access Protocol) 인터페이스는 웹 서비스를 위한 통신 프로토콜로, XML 기반으로 데이터를 주고받는 것을 지원합니다.
WSDL (Web Services Description Language) 는 SOAP 을 사용하는 웹 서비스를 설명하는 언어로, 서비스에 대한 메소드, 파라미터, 입/출력 등을 정의하고 서비스의 위치를 명시하는데 사용됩니다.

## MSA 의 자바 RMI 와 RPC 메커니즘 이란?

MSA (Microsoft Specific Architecture) 의 RMI (Remote Method Invocation) 은 자바 플랫폼에서 사용되는 분산 객체 기술로, 객체간의 메소드 호출을 원격에서 수행할 수 있도록 합니다. RMI 는 자바 객체를 원격에서 사용할 수 있도록 하며, 이를 위해 자바 RMI 인터페이스를 제공합니다.
RPC (Remote Procedure Call) 메커니즘은 원격 컴퓨터에서 프로시저를 실행하는 기술로, 원격에 있는 프로시저를 호출하는 것과 마찬가지로 로컬에 있는 프로시저를 호출하는 것처럼 사용할 수 있도록 합니다. 이를 위해 프로토콜을 사용하여 통신하며, 이를 이용해 원격에 있는 서비스를 사용할 수 있습니다.

## What is Orchestration and Choreography in MSA?

Orchestration and choreography are two different approaches to managing communication and coordination between microservices in a microservice architecture (MSA).
Orchestration refers to a centralized approach where a single service, called the orchestrator, controls and coordinates the interactions between other services. The orchestrator is responsible for managing the flow of requests and responses between services, and for ensuring that the necessary interactions between services take place in the correct order.
Choreography, on the other hand, is a decentralized approach where each service is responsible for determining how it interacts with other services. Services communicate directly with each other and coordinate their actions through a shared understanding of the protocols and message formats that they use. There is no central control or coordination point.
Both orchestration and choreography have their own advantages and use cases, and the choice between them depends on the specific requirements of the system being built.

## What is a Bounded Context?
A bounded context is a term used in Domain-Driven Design (DDD) to refer to a specific domain or area of the business in which a certain set of concepts and rules apply. It is a way to encapsulate and isolate the complexity of a domain, and to create a clear boundary between different parts of the system.
In a microservices architecture, a bounded context can be used to represent a single microservice, or a group of related microservices that together form a cohesive unit of functionality. Each microservice can have its own data model and business logic, and can be developed, deployed, and scaled independently of other microservices.
The idea behind bounded context is to align the subdomain with the team that is working on it, that way the team can focus on a specific set of problems and it will be easier for them to understand and communicate about it. By doing so, it allows the team to make changes in the subdomain without affecting the other parts of the system, and it will also make it easier to evolve the system over time.