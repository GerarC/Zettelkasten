## Software Architecture (SfA) in Practice
#### Definitions
1. **Software architecture:** Is the *set of structures* that are essential for understanding and managing the system, including software elements, relations among them and properties of both.
2.  **Software Structure**: Set of *elements* (components or modules) held together by a relation. There are three types:
	1. **Module decomposition**: each module have specific responsibilities, Like database, business rules, interface, etc... You can aggregate it in layers. This type of structures is static. The focus is how the system's functionality and the team are divided.
	2. **Component-and-Connector (C&C):** this is a runtime structure, where the system is built as a set of services. Those services, their relations, synchronization and the infrastructure they interact are called *C&C*. *Components* are always a runtime entity.
	3. **Allocation:** describes the mapping from structure elements to the system's organizational,  environment. Like *Modules* are assigned to Teams, and to places in a directory structure. *Components* are deployed onto hardware.
3. **Abstraction:** a *SfA* is an *Abstraction* because omits information that isn't important for understanding the system. How *Elements* interact (through *interfaces*), how are composed, their relevant properties, etc...
4. **Views**: it's a representation of a structure elements and their relations. Not the whole software structure, there can be different views from the same SfA.
5. **Architectural Patterns:** are the way that elements are composed to solve particular problems.

<div style="page-break-after: always;"></div>

### Why use SfA?
Structures provide **insight**. Each structure provides and leverages different perspective of the system

![[Types of Structures - SfA.png]]

<div style="page-break-after: always;"></div>

## Several Terms
- *Mime types:* Standard to represent different data can be used and transferred in web.
- *Pub/Sub:* A pattern used to send data to client without its petitions, It's very useful with micro services.
- *DevOPS:* It's a combination of culture, philosophy, practice and tools that seek deliver application and services at high speed. Makes use of IaC (Infrastructure as Code) and Pipelines to automatize Developer IT Operations.
- *JQuery:* A JavaScript library associated to *AJAX* <small>Asynchronous JavaScript and XML</small>
- *Container:* Its a standard unit of software that packages all the needed dependencies for an application.
- *Docker:* A container manager.
- *Kubernetes:* Container orchestrator, manages connections between containers.
- *EJB:* Enterprise Java Beans, a *Bean* is a reusable object in java.
- *HL7:* A world wide format used for heath sites.
- *BPMN:* Business Process Model and Notation.

<div style="page-break-after: always;"></div>

## Databases
![[TriangleCAP.png]]
- A DB system just can have 2 of the three characteristics of CAP
- **ACID:** Atomicity, Consistency, Isolation and Durability. Are properties a DB Must have.

## IDL <small style="color:gray;">Interface definition language</small>
It's a language that allows to an application made with a programming language to communicate with another application made with another lang.
<div style="page-break-after: always;"></div>

## WEB Services
- Each Web service has a contract language, an IDL.
- *SOAP:*
	- Simple Object Access Protocol <small style="color:gray;">W3C: Whom Standardize all the Web</small>.
	- It's associated *IDL* is **WSDL** <small style="color:gray;">Web Service Description Language, it's an XMl Schema</small>
	- UDDI <small style="color:gray;">Universal Description, Definition and Integration</small>. It's based of SOAP and defines a way to publish and find information 
	- Has QoS: It means that is Secure and it's fiable.
- *RESTful:*
	- Created by Roy Fielding, HTTP Creator.It isn't an Standard, Based a on HTTP, defines a way to interact through HTTP. 
	- Resources -> An URI
	- Method: To manipulate resources <small style="color:gray;"><small>GET, POST, PUT, DELETE, CONNECT, TRACE, HEAD</small></small>
- *gRPC:* Was created by google. Call to Remote Procedures and it's used to define APIs. It's so fast to transmit data because is binary codification. Use it when you are using thousands services. Has an IDL called Protocol Buffers or Proto3.
- *GRAPHQL:* it's a consult language based on graphs. specialized to the Frontend. It has an IDL called Schema. A lightest 

## Cloud Computing
- **Types:**
	- *Hybrids:* a mix of interconnected, private and public, clouds
	- *Community:* It's a collaboration where infrastructure is shared between several organizations and/or communities.
	- *Public:* An Infrastructure available to all people or a large sector.
	- *Private:* A Cloud infrastructure dedicated to one organization.
- **Layers:**
	- *SaaS* <small>Software as a Service</small>
	- *PaaS* <small>Platform as a Service</small>
	- *BaaS* <small>Backend as a Service</small>
	- *IaaS* <small>Infrastructure as a Service</small>
	- *XaaS* <small>Anything as a Service</small>
- **Cloud Native:** When application is oriented to using cloud services.

## Software engineering
- ***Three Main Topics:***
	1. **Patterns:** Are toolkit of solutions to common problems, There are three: Design Patterns such as *GoF* or *GRASP*, Architectural Patterns like *POSA*, and organizational Patterns like *Coplien*
	2. **Heterodox Methods:** Ways teams have to work such as XP (eXtreme Programming), Scrum, Kanban,  Lean, Evo, DSDM and so forth.
	3. **Software applications:** Final product
- ***Other Topics:***
	- **Refactoring**
	- **Technologies:** Software and tool that are used to create new software. Examples, AOP, SOA, Cloud Computing, Web3, Blockchain and so on.
> [!Note] SOA
> There's a common communication channel, like a tunnel, called ESB (Enterprise Service Bus). To this tunnel there are connected a lot of connectors called endpoints or ports. Web Services are connected to these ports, these web services communicate Process of a business.
> The bus orchestrate all those web services. OpenESB Studio

# Software Desing
Process of applying several techniques and principles with the purpose of defining an application before coding.
- **Design Phases:**
	1. *Physic* 
	2. *Logic* 
	3. *Data Model* 
- **Design Process:**
	1. *Data*
	2. *Architecture*
	3. *Procedures*
	4. *Interfaces*
<div style="page-break-after: always;"></div>

# Architecture
Is the fundamental organization of a system represented by its components, the relationships between them and the environment and the principles that guide its design and evolution.
- **Structural Elements:** Layers that support other layers inside the system: O/S Functions, Language Standard Libraries, Third party libraries or your own code.
- **Connectors:**
	- *Case tools*
	- *ADL:* Architecture Description Language.
	- *Stacks:* such as *MEAN* or *MERN*.
	- *BOINC:* Berkeley Open Infrastructure for Network Computing.

The more the system grows, the more complexity there's. So it's needed Design and implementation.

In OOP applications classes represent fine granularity units.

A system must have low coupling.

## History
1. **Dijkstra:** Proposes make the structure before programming, defines abstraction levels and a conceptual design.
2. **P.I. Sharp:** Says that Software architecture is different to Software Engineering and established Specifications -> *Functionality*, *Design* and *Shape*.
3. **Structure Design:** Software development models -> Cascading, evolutionary and cyclic models.
4. **David Parnas:** Proposes modules, hidden information software structures and program families. Seeking of software quality and early design decisions.
5. **OOP:** introduces ADTs (Abstract Data Types), classes, smalltalk and the theory of Modeling domain of the problem and implementing it in an OOP Language.
6. **Perry & Wolf:** Suggest Software architecture is analogous to building construction and that is composed by three components -> *Elements*, *Form* and *Reason*.
7. **Apogee of SAs:** Use of Components, Design patterns, Architectural Styles and ADLs
	- *Architectural views*: 4 + 1, TOGAF, RM/ODP, IEEE 1461.
## Software Architect Profile
It's the person in charge of establish design purposes, quality attributes, primary functionality, architectural concerns, constrains. And using those things, builds architectural views.

## Algorithm to make an Architecture
1. Define architectural requirements.
2. An initial effort to define candidate architecture and refine enterprise architecture.
3. Define the reference architecture.
4. Support project teams.

### Steps
1. Creation of business case (Understanding the business).
2. Understand requirements.
3. Creation and selection of Software.
4. Documentation and communication the architecture.
5. Analysis or evaluation of the chosen software Architecture (Atam Strategy).
6. Implementing Software Architecture.
7. Watch the implementation is equal to the architecture.

### Defining an Architecture
1. Define Main Modules.
2. Define Responsibility of each module.
3. Define interaction between modules:
	1. Control and data flow.
	2. information sequencing.

## Design Levels
1. Architectonic Design
2. Interaction Design
3. Low Level

## Implementation Process
1. Requirement Analysis, platform definition.
2. Design by models
3. Architecture definition
4. Development, pattern uses, frameworks (GRASP, GoF,PoSA, PoEEA, J2EE)
5. Component integration
6. System retrieving
7. Test and QoS Evaluation <small style="color:gray">Betas 1-2, Release candidate 1-2</small>, Jira <small style="color:gray">Bug tracking</small>, Bugzilla.

## Development Process Component Based
1. Architecture Stack
2. Enterprise Patterns
3. Architectural Styles
4. Architectural Principles
5. Design Patterns
6. Design Principles
7. OOP
8. Programming Paradigms 
9. Clean Code

## House analogue 
***The application***
**Patterns - Frameworks, Libraries, Technologies - Common sense and Experience**
*Principles*

<div style="page-break-after: always;"></div>

## Important Aspects of Software Architecture
1. Select an architectural view: *C4* (Content, Container, Components and Code), *4 + 1* (UML) or so forth.
2. Select an architectural Style: *Monolithic*, *SOA - Microservices*, *Layer Architecture*.
3. Select *on-premise* or *cloud*.
4. Consider Authentication/Authorization and Privacity.
5. Define communication protocols and security rules.
6. Define charge balance (Nginx), Messaging (Kafka, RabbitMQ, JMS).
7. Make a general revision of any critic algorithm that controls services.
8. Consider bottle necks and its solutions.
9. Select a database.
10. Think on what data can be cached (ElasticSearch / Apache Solr).
11. Select monitoring system (Prometheus / Grafana), logging (Logstash / Fluentd).
12. Select exceptions and failures managing (Netflix turbine / Hystrix).
13. Define segregation between public and restricted areas.

## Component
A *component* is a block of modular building piece for software, is changeable and encapsulates attributes and functionalities. These components have the next properties:
- **Cohesion:** A component encapsulates elements which only attributes and operations that are related between them.
- **Coupling:** It's a qualitative measure of grade of class' connection with another. There should be low coupling between anything.

### Creation of Components
1. Identify all clases of domain problem.
2. All classes belonging to infrastructure domain.
3. Make unique classes:
	1. Specify messages between classes that collaborate.
	2. Identify Interfaces (connections)
4. Describe persistent data sources.

## Architectonic Views
It's an abstract representation of the structure and organization of the system from its architectonic perspective. Centered in the main architectonic elements of the system, their relations and how they are connected to achieve functional requirements. There are several types of view:
- *Logic view:* Analyst/Designer, functionality, static diagrams, dynamic diagrams.
- *Process view*
- *Physical view*
- *Deploy view*
- *Use Cases view*

<div style="page-break-after: always;"></div>

# Principles
- ## Kiss <small style="font-weight:400;font-size:14;">Keep it simple, stupid</small>
	Simple things do work better and are simple to maintain. Follow this principle improves legibility and system comprehension, facilitates maintenance and decreases Technic doubt.
	##### **Recommendations:**
	- Divide and Conquer.
	- Keep small methods (No more than 30-40 lines).
	- Each method must resolve one problem and don't use cases.
- ## DRY <small style="font-weight:400;font-size:14;">Don't repeat yourself</small>
	Each piece of code  should be unique, defined, have an unique objective.
	##### **Recommendations:**
	- Make use of templates
- ## YAGNI <small style="font-weight:400;font-size:14;">You aren't gonna need it</small>
	Refers to don't code things that you won't use and erase useless things.
- ## SOLID
	The name is an acronym of five principles:
	- *Single Responsibility:* A class should do one thing and a single reason to change.
	- *Open-Cloose:* A class should be open to extension and closed to modifications.
	- *Liskov Substitution:* Any subclass should be substitutable by its parent class with out break nothing
	- *Interface Segregration:* Keeping things separated, means that it's better have various specific interfaces than only a general purpose one.
	- *Dependency Inversion:* States that a Class should depend on interfaces or abstract classes instead of specific implementations.
	
<div style="page-break-after: always;"></div>

# UML Guide
## Design guide in the architecture
- Name convention
- Interface notation and draw it at left side of the diagram.
- Name interfaces with I prefix (deprecated).
- Use Case tools
- Model dependencies from left to right
- Read UML documentation

## Packages Diagram
- Arrows meaning package dependencies.

## Component Diagram
- *Component types:* Distribution, work and execution components
- *Component interfaces:* Proportional and Required interfaces.

~~~ mermaid
flowchart TD;
Con[Controller] -->|Uses| Ser[Service]
Ser -->|Uses| DAO[DAO]
DAO -->|Uses| DB[Database]
~~~

## Deployment Diagram
Show the physical localization of the components, the used elements are:
- *Components*
- *Node:* A cube that represents a piece of hardware in the system (Where the component is).
- *Association:* A line that link nodes.

**Stereotypes:**
- `<<Device>>`: a node that represent a physical device like a computer, a mobile or servers and more
- `<<Deployment>>`: It's a dependency relation that describes a artifact location. Can be associated to one or more artifacts
- `<<Artifact>>`: a classifier that represents a physical system like a source, a library, executable script or Web Archive.

> **Pros:**
> -  Show a set of nodes and their relations. 
> - Used to describe the static deployment view.

> **Cons:**
> - Possible hardware failing because of the modeling.

<div style="page-break-after: always;"></div>

# Software Patterns
- **Creational:** Abstraction of the object creation process, like *Builder*, *Singleton* or *Prototype*-
- **Structural:**: Centered in class relations, some examples are *Facade*, *Bridge* or *Decorator*.
- **Behavioral:** Inheritance and distribution of behavior between classes, such as *Interpreter*, *Observer* or *Strategy*.

# POSA <small style="color:gray;font-size:16">Pattern Oriented Software Architecture</small>
First book that did a pattern classification. They are shown from High to low detail
~~~ mermaid
graph LR;
	Arch[<small><h3>Architectural Patterns</h3>Affect to the global structure of the system<br/>Suggests global architecture the app should follow <br/>An example could be <i>MVC pattern</i></small>]
	Desig[<small><h3>Design Patterns</h3>Define micro-architectures in subsystem of components<br/>Explain how to solve a particular design problem <br>For example, <i>DAO pattern</i> allows to abstract and to encapsulate the access to a Database</small>]
	Idio[<small><h3>Idioms</h3>Details of the structure and behavior of the components<br/>Allows to resolve a problem with a particular implementation of a specific language<br/>For example, in java to compare an object you use <code>equals</code> and <code>hashCode</code></small>]
~~~

## Architectural Styles
