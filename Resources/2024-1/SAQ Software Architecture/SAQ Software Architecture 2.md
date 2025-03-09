- Three Main topics in Software Engineering
	- Patterns:
		- Design patterns (GoF - GRASP)
		- Architectural Patterns (POSA)
		- Organizational Patterns (Coplien)
	- Heterodox Methods: XP (eXtreme Programming, Scrum, KANBAN, LEAN, Evo, DSDM, RUP, AM, Crystal, LD, ASD).
	- Software Application
-  Others:
	- Refactoring
	- Technologies: Functional Prog, AOP, SOA <small style="color:gray">Service oriented Architecture</small>, Cloud Computing, Mobile Apps, Software Product lines, Software Factory, ChatGPT/Github Copilot, Semantic Web, Web3, Blockchain.

> [!Note] SOA
> There's a common communication channel, like a tunnel, called ESB (Enterprise Service Bus). To this tunnel there are connected a lot of connectors called endpoints or ports. Web Services are connected to these ports, these web services communicate Process of a business.
> The bus orchestrate all those web services. OpenESB Studio


**HL7:** World wide used format for Health Sites.

**BPMN:**
- Business Process Model and Notation.

## Cloud Computing
There are different types of Clouds:
- Hybrids
- Community
- Public
- Private

**Cloud Layers:**
- SaaS <small>Software as a Service</small>
- PaaS <small>Platform as a Service</small>
- BaaS <small>Backend as a Service</small>
- IaaS <small>Infrastructure as a Service</small>
- XaaS <small>Anything as a Service</small>

**Cloud Native:**
- All what you do is oriented to using Cloud Services.

AWS -> PaaS


## Sematic Web
RDF: Search about RDF.

## Web3
- Dapps.


# Sofware Design
Process of applying several techniques and principles with the purpose of defining the application before coding.

Design phases:
- Physic
- Logic
- Data model

Design process:
- data
- architecture
- procedures
- interfaces

# Architecture
- What is a software architecture?
	There are not official definition
	- some people compare it with *abstraction of structures*
	- all what you need about the system that is not code.
A definition for us can be:
	is the fundamental organization of a system represented by its components, the relationships between them and the environment and the principles that guide its design and evolution

Software engineering model oriented 

**Structural Elements:**
- layers that support other layers inside the system:
- O/S Funcs.
- Language Standard Libraries.
- Third party Libs.
- The code of your.

**Connectors**

Case Tools
ADL -> Search definition

MEAN STACK
MERN STACKl

Project BOINC

Sync, Async, Peer to Peer, Event Broadcast

Shaw Philosophy 


## History
Dijkstra:
- Structure before programming
- It defines abstraction levels
- Conceptual Design

P.I. Sharp:
- Software Architecture
- Specifications: Functionality + Design + Shape

Structure Design:
- Software development models
- Cascading, evolutionary and cyclic models

David Parnas:
- Modules and hidden information
- software structures and program families
- Seeking of software quality
- Early Design Decisions

OOP:
- TADs, clases, smalltalk
- Theory: Model the domain of the problem and implement it in a OOP lang.

Perry & Wolf:
- Software architecture that is analogous to building construction.

Apogeo of SAs:
- Components
- Design patterns
- Architectural Styles ADLs
- Architectural views: Proposed models:
	-  4 +1
	- TOGAF
	- RM/ODP
	- IEEE 1461

MONO Project
Xamarin

Serverless -> Amazon lambda, Open FaaS, Fn Project|


### Software Architect
Desing Purporses

Quality Attributes

Primary Functionality

Architectural Concerns

Constrains


All before is for build architectural views


### SW vs Complexity
The more the system grows, the more the complexity augment

Design and implementation

In OO applications classes represent fine granularity units

How to avoid dependencies?: Microservices

Have system with low coupling 

### Algorithm to make an Architecture
1. Define architectural requirements

2. An initial effort To define candidate architecture
	1. refine enterprise architecture
3. Define a Reference architecture
4. Support project teams.

#### Steps
1. Creation of the business case (understand the business)
2. Understand requirements
3. Creation and selection of SW
4. Documentation and communication of the architecture
5. Analysis or evaluation of the chosen SW (ATAM strategy)
6. Implementation of the SW system.
7. Watch the implementation is equals to the architecture.


#### Defining an architecture
1. define main modules
2. define responsibility of each module
3. define interaction between modules:
	1. control and data flow
	2. information sequencing


### Difference between Architecture and Design

1.  level of abstraction:
	- SW: High level
	- Design: low level
2.  product
	- SW: subsystem, interfaces, horizontal services, frameworks, reusable components  
	- Design: component design, code specification
3. Focusing area:
	- SW: Tech selection (stack), QoS (NonFunctional requirements)
	- Design: Functional requirements


### Design Levels 
1. Architectonic Design
2. Interaction Design 
3. low level


### Implementation Process
1. Requirement Analysis, platform definition
2. Design by Models
3. Architecture definition
4. Development, pattern uses, frameworks (GRASP, GoF, PoSA, PoEAA, J2EE)
5. Component integration
6. system retrieving
7. Test and QoS Evaluation (Betas 1-2, release candidate 1-2), Jira (Bug tracking), Bugzilla.

### Development process component based
Architecture Stack
1. Enterprise Patterns
2. Architectural Patterns
3. Architectural Styles
4. Architectural Principles
5. Design Patterns
6. Design Principles
7. OOP
8. Programming Paradigms
9. Clean Code

### House like

The application
Patterns - Frameworks, libraries, technologies - Common sense and experience
Principles


## Principles
### Kiss
Keep it simple, stupid
Simple things do work better and are simple to maintain 
Advantages:
- Improves legibility and system comprehension 
- facilitates maintenance and decreases Technic doubt ...

**Recomendations:**
- Divide and Conquer
- Keept small methods (No more than 30-40 lines).
- Each method must resolve one problem and do not use cases

### DRY
Don't repeat yourself
- each piece of code should be unique, defined, have an unique objective

### YAGNI
you aren't gonna need it
Refers to do not code things that you won't use and erase the useless.


### SOLID
- Single Responsibility
- Open Close
- Liskov substitution
- Interface segregation (Facade pattern)
- Dependency inversion

## Important aspects of SW
- Select architectural View: C4(Content, Container, Components, Code), 4+1(UML)
- Select Architectural Style (Monolitic, SOA - Microservices, Layer architecture)
- Select on-premise or cloud
- Consider Authentication/ authorization and privacity.
- Define Communication protocols and security rules.
- define Charge balance (nginx), messaging (Kafka, RabiitMQ, jms)
- Make a general revision of any critic algorithm that control the service.
- Consider bottle necks and its solutions
- Select database
- What data need to be cached (Elasticsearch / Apache Solr).
- Select monitoring system (Prometeus / Grafana), logging (Logstash / Fluentd), how to manage exceptions and failures (Netflix Turbine / Hystrix).
- Define separation between public and restricted areas


### Component
- It's a block of modular building for software.
- It's changeable 
- Encapsulates 
- **Cohesion**:
	- Encapsulates only attributes and operations that are related between them.
	- A component should have a lot of cohesion.
- **Coupling**:
	- It's the qualitative measure of the grade of connection of a class with other.
	- there should be low coupling between classes.

#### Creation of Components
1. Identify all classes of the problem domain
2. all classes that belong to the infrastructure domain
3. Just make classes that aren't reused.
	1. Specify messages between classes that collaborate.
	2. identify interfaces
4. Describe persistent data sources.


### Architectonic Views
- It's a abstract representation of the structure and organization of the system from its architectonic perspective.
- It's centered in the main architectonic elements of the system, their relation and how they are connected to achieve functional requirements
- There are some views:
	- Logic view: analyst/designer - functionality - static diagrams - dynamic diagrams
	- process view
	- physical view
	- deploy view
	- use cases view


### UML General description



### Design guide in the architecture
- Name convention
- Interface notation and draw it at left side in the diagram
- Name Interfaces with the Prefix I
- Use Case tools
- Model dependencies from left to right
- Read UML documentation.

### Packages Diagram
- Arrows meaning package dependencies.

### Component Diagram
- Component types:
	- Distribution components
	- Work components
	- execution components
- Component interfaces:
	- Proportional interface
	- Required interface



BD <- DAO <- SER <- Controller