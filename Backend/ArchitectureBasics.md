# Understanding Different Software Architectures - For Bootcamp Grads

I was not aware that there were different kinds of software architectures until I was working at one of my recent positions and some of the seniors were talking about "removing this monolithic (insert bad word here)." And I think most bootcamp grads might not learn about different software architectures. However, I think it's useful to understand that there are different approaches to building applications. 
Who knows, maybe you can also impress your interviewer by asking about the company's architectural style!

I didn't think it would make sense to include a lot of technical talk when I am just introducing the different styles. The goal of this article is to introduce software architectural styles in a simple and relatable fashion.

## Table of Contents

- [Monolithic Architecture](#monolithic-architecture)
  - [Example of a Monolithic Architecture](#example-of-a-monolithic-architecture)
- [Microservices Architecture](#microservices-architecture)
  - [Example of a Microservices Architecture](#example-of-a-microservices-architecture)
- [Service-Oriented Architecture (SOA)](#service-oriented-architecture-soa)
  - [Example of a Service-Oriented Architecture](#example-of-a-service-oriented-architecture)
- [Event-Driven Architecture (EDA)](#event-driven-architecture-eda)
  - [Example of an Event-Driven Architecture](#example-of-an-event-driven-architecture)
- [Layered Architecture](#layered-architecture)
  - [Example of a Layered Architecture](#example-of-a-layered-architecture)
- [Domain-Driven Design (DDD)](#domain-driven-design-ddd)
  - [Example of a Domain-Driven Design](#example-of-a-domain-driven-design)
- [Serverless Architecture](#serverless-architecture)
  - [Example of a Serverless Architecture](#example-of-a-serverless-architecture)

## Monolithic Architecture

In the realm of software architecture, Monolithic Architecture stands tall as a traditional powerhouse. It's like a mighty castle, housing the entire application within its solid walls. With simplicity and cost-effectiveness at its core, this architectural style is a go-to choice for smaller projects or when speed is of the essence. Developers can wield their skills to build the entire application as a single, self-contained unit, embracing the simplicity and efficiency that this architectural giant brings.

### Example of a Monolithic Architecture

One example of a company that has traditionally used a monolithic architecture is Microsoft with its Windows operating system. In earlier versions of Windows, the entire operating system was developed as a single, self-contained unit, tightly integrating various components and functionalities.

## Microservices Architecture

Prepare to enter a realm of distributed systems where agility and scalability reign supreme. The Microservices Architecture is like assembling a league of superheroes, each possessing unique abilities. By breaking down the application into smaller, autonomous services, developers unlock the power of scalability, fault isolation, and independent deployment. This architectural approach is the ultimate choice for constructing large, complex systems that demand adaptability and constant evolution.

### Example of a Microservices Architecture

Netflix is a prime example of a company that extensively utilizes microservices architecture. Its streaming platform is built on a vast network of independently deployable microservices, such as user authentication, content recommendation, billing, and video encoding. This modular approach allows Netflix to scale different services based on demand and enables continuous deployment and evolution.

## Service-Oriented Architecture (SOA)

Welcome to a modular universe where services take center stage, becoming the building blocks of innovation. The Service-Oriented Architecture (SOA) empowers developers to create loosely coupled and reusable services that transcend system boundaries. This architectural style fosters seamless interoperability, connecting different systems and technologies with ease. It's like building a universal language translator, enabling systems to communicate harmoniously across diverse domains.

### Example of a Service-Oriented Architecture

Salesforce, a leading customer relationship management (CRM) platform, adopts a service-oriented architecture. It provides a wide range of services, including sales management, marketing automation, and customer support, which can be accessed and integrated through a unified API. This architecture enables seamless interoperability and customization across various business systems.

## Event-Driven Architecture (EDA)

Prepare to be swept away into a world where components dance to the rhythm of events. The Event-Driven Architecture (EDA) is akin to orchestrating a grand symphony, where every event acts as a catalyst, setting off a chain reaction of actions. This reactive approach liberates systems from tight coupling, opening doors to scalability, real-time processing, and complex business workflows. EDA is the perfect fit for applications that thrive on events, paving the way for dynamic and eventful digital experiences.

### Example of an Event-Driven Architecture

Uber utilizes event-driven architecture in its ride-hailing platform. Events such as ride requests, driver availability, and trip updates trigger actions and workflows across different components. This architecture allows Uber to handle a massive volume of real-time events, ensuring scalability, responsiveness, and reliable coordination between users, drivers, and the system.

## Layered Architecture

Step into a well-organized kingdom, where different layers of power and responsibility reign supreme. The Layered Architecture is like a royal court, where each layer has its designated role to play. By separating components into logical layers such as presentation, business logic, and data access, developers unlock the power of separation of concerns, maintainability, and code reusability. This architectural style serves as the cornerstone for building robust and well-structured applications.

### Example of a Layered Architecture

The Java Enterprise Edition (Java EE) framework is built upon a layered architecture. It provides a set of standardized components and APIs for building enterprise applications. The architecture separates concerns into layers like presentation (e.g., JSF, JSP), business logic (e.g., EJB), and data access (e.g., JPA), promoting modularity, maintainability, and interoperability across various Java EE applications.

## Domain-Driven Design (DDD)

Embark on a quest to unveil the secrets of software development that align closely with the problem domain. Domain-Driven Design (DDD) is like a mystical journey, where domain experts and developers collaborate to uncover the very essence of the problem at hand. By modeling the application domain and its concepts with meticulous precision, developers create software solutions that are deeply rooted in the problem space. DDD empowers developers to bridge the gap between technical and business domains, breathing life into software that resonates with the needs of the domain.

### Example of a Domain-Driven Design

Domain-driven design finds application in companies like Airbnb. Airbnb utilizes DDD principles to model its domain, encompassing concepts such as property listings, bookings, and user profiles. By aligning their software closely with the problem domain, Airbnb can effectively address the needs of both hosts and guests, providing a seamless and intuitive user experience.

## Serverless Architecture

Prepare to step into a magical realm where developers can unleash their coding prowess without the burdens of infrastructure management. Serverless Architecture is like having a personal genie at your disposal, effortlessly handling the underlying infrastructure. This cloud-native approach offers scalability, cost optimization, and rapid development, providing developers with the freedom to focus solely on writing code. Whether you're embarking on event-driven workloads or building microservices, Serverless Architecture grants you the power to bring your innovative ideas to life with unparalleled agility.

### Example of a Serverless Architecture

AWS Lambda, a serverless computing service provided by Amazon Web Services, is a prime example of a company offering a serverless architecture. Developers can write code in various programming languages and have it executed on-demand without managing servers. This architecture enables rapid development and scalability, and many companies leverage AWS Lambda for building serverless applications and event-driven workloads.