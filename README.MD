# Software Design

This is a collection of notes on software design. It is a work in progress and will be updated as I learn more.

# why Design?
* To make software easier to understand and maintain
* To create a solution that is flexible and can be extended
* Tackle Complexity: The more complex the problem, the more important design becomes
# Tackle Complexity
* BUFD: Big Up Front Design
* Diagrams: UML, Sequence, Class, State, Activity, Component, Deployment, etc.
* Writing Documentation
* Writing Tests

# Separation of Concerns
* you need to separate the concerns of your application into different layers
* The layers should be independent of each other
* The layers should be loosely coupled
* The layers should be easy to test
* The layers should be easy to extend
* The layers should be easy to maintain
# Lower Coupling and Higher Cohesion
* Coupling: How much a class knows about other classes
* Cohesion: How much a class does
* High Cohesion: A class should do one thing
* Low Coupling: A class should know as little as possible about other classes
its all about separation of concerns and making your code easy to understand and maintain
# The Four Rules Of Good Separation Of Concerns
1 - Separate the business logic from Presentation, in other words, separate the UI from the business logic of your application 
what this means is that you should have a layer that is responsible for the UI and a layer that is responsible for the business logic
what is the benefit of this? well, if you want to change the UI, you don't have to change the business logic and vice versa
and if you want to test the business logic, you don't have to test the UI
and if you want to extend the business logic, you don't have to extend the UI
you well save a lot of time and effort in the long run
keep the business logi in the business layer and the UI in the UI layer

2 - Create Clear business entry points to your businsess logic: This means that you should have a clear entry point to your business logic
for example, if you have a class that is responsible for creating a user, you should have a method called createUser and the endpoint should be called api/user/create
this way, you can easily understand what the endpoint does and you can easily test it
you can also easily extend it, for sure you will have to add more endpoints to your application, so you should have a clear entry point to your business logic

3 - Separate your stuff from infrastructure: This means that you should have a layer that is responsible for the infrastructure
for example, if you are using a database, you should have a layer that is responsible for the database
a big example is the repository pattern: you have a repository that is responsible for the database and you have a service that is responsible for the business logic
the service should not know anything about the database, it should only know about the repository
Example: 
 Hexagonal Architecture

4 - Avoid Tutorialware: This means that you should avoid writing code that is written in tutorials, you should write code that is easy to understand and maintain

# Architecture Through our short history of software development, we have seen many different architectures
* Monolithic Architecture
* Layered Architecture
* Microservices Architecture
* Hexagonal Architecture
* Event Driven Architecture
* Serverless Architecture

- Architecture is blocks and arrows
- Architecture is about cost of change
- Architecture is about reducing const of change
