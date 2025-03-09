# Webhook
Using webhooks, server usually inits the conversation between it and the client, also is known as inverse API or push API

Client subscribe its url to the server and the server makes post to the client, it's usually used to send notifications

- advantages:
	- automation
	- real time information
	- easy configuring
	- improve network and informatics security
- disadvantages:
	- less functionality than an API
	- data loosing
	- potentially overcharge
	- External servers are necessary

# BFF

(Back-end from front-end)
it creates a custom back-end for each front-end, i.e., web, mobile, etc...

# MVVM
Model View ViewModel
- Applications with graphical interface
### View
it's in charge to define how the application is showed

# Clean Architecture
Main purpose of clean architecture is to separation of responsibilities 
- Layers:
	- Domain (Business logic):
		- Business rules:  Restrictions and politic definitions that must be applied in the business.
		- Entities: objects that encapsulates data and business rules.
	- Use Cases:
		- use case rules: implements logic of the business, its rules and entities. Technic limitations of the application.
	- Adapter:
		- its a communication bridge between domain and implementation details.
	- External:
		- Implementation  details and infrastructure.

- Framework independence:
	- The application architecture must be framework application.
- User interface independence:
	- Logic must be isolated from user interface.
- Database independence:
	- Logic must be independent from the database you're using.

Promotes a high no coupling.

# SOFEA
Service Oriented Front-End Architecture  

Basically like micro-services like the back-end   

### SOA
Service oriented architecture
- Born to be more flexible in a time that every application must be personalized 
- Tries flexible coupling
- interoperability  and specific contract.

# Space-Based Architecture
It's a distributed system, composed by a central middleware that coordinates all the different processing units.

### Processing Unit
- Its business logic
- Data that will be used by the unit (in memory database)
- A Data replication engine

### Virtualized Middleware
- Messaging grid: 
- Data grid: synchronizes data changes.
- Processing grid: In charge to coordinate dependency between units
- Deployment manager: deploy and escalates processing units.