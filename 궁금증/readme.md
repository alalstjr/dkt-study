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

오케스트레이션과 구성은 MSA(마이크로서비스 아키텍처)에서 마이크로서비스 간의 통신 및 조정을 관리하는 두 가지 접근 방식입니다.
오케스트레이션은 오케스트레이터라고 하는 단일 서비스가 다른 서비스 간의 상호 작용을 제어하고 조정하는 중앙 집중식 접근 방식을 나타냅니다. 오케스트레이터는 서비스 간의 요청 및 응답 흐름을 관리하고 서비스 간에 필요한 상호 작용이 올바른 순서로 발생하는지 확인하는 일을 담당합니다.
반면에 안무는 각 서비스가 다른 서비스와 상호 작용하는 방식을 결정하는 분산된 접근 방식입니다. 서비스는 서로 직접 통신하고 사용하는 프로토콜 및 메시지 형식에 대한 이해를 공유하여 작업을 조정합니다. 중앙 제어 또는 조정 지점이 없습니다.
오케스트레이션과 구성 모두 고유한 장점과 사용 사례가 있으며 둘 중 하나를 선택하는 것은 구축 중인 시스템의 특정 요구 사항에 따라 다릅니다.

## What is a Bounded Context?
A bounded context is a term used in Domain-Driven Design (DDD) to refer to a specific domain or area of the business in which a certain set of concepts and rules apply. It is a way to encapsulate and isolate the complexity of a domain, and to create a clear boundary between different parts of the system.
In a microservices architecture, a bounded context can be used to represent a single microservice, or a group of related microservices that together form a cohesive unit of functionality. Each microservice can have its own data model and business logic, and can be developed, deployed, and scaled independently of other microservices.
The idea behind bounded context is to align the subdomain with the team that is working on it, that way the team can focus on a specific set of problems and it will be easier for them to understand and communicate about it. By doing so, it allows the team to make changes in the subdomain without affecting the other parts of the system, and it will also make it easier to evolve the system over time.

제한된 컨텍스트는 DDD(Domain-Driven Design)에서 특정 개념 및 규칙 집합이 적용되는 특정 도메인 또는 비즈니스 영역을 나타내는 데 사용되는 용어입니다. 도메인의 복잡성을 캡슐화 및 격리하고 시스템의 다른 부분 간에 명확한 경계를 만드는 방법입니다.
마이크로 서비스 아키텍처에서 제한된 컨텍스트는 단일 마이크로 서비스 또는 결합된 기능 단위를 함께 형성하는 관련 마이크로 서비스 그룹을 나타내는 데 사용할 수 있습니다. 각 마이크로 서비스는 자체 데이터 모델 및 비즈니스 논리를 가질 수 있으며 다른 마이크로 서비스와 독립적으로 개발, 배포 및 확장될 수 있습니다.
제한된 컨텍스트의 이면에 있는 아이디어는 하위 도메인을 작업 중인 팀과 정렬하여 팀이 특정 문제 세트에 집중할 수 있고 팀이 더 쉽게 이해하고 소통할 수 있도록 하는 것입니다. 이렇게 하면 팀이 시스템의 다른 부분에 영향을 주지 않고 하위 도메인을 변경할 수 있으며 시간이 지남에 따라 시스템을 더 쉽게 발전시킬 수 있습니다.