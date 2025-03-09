# Software Architecture

How to integrate all the components to make some of quality.

- Models based on Architectural styles (?).

- What is a software component?
- Who is a Software Architect?
- Modern architectonic style...
- Architectonic Patterns.
- Web Services (REST like).
- Team Work around a software project.


Content:
- Software architecture
- component
- architectonic Pattern
- Frameworks
- Architectural Patterns
- Quality Factors
- Domain-specific software architecture

Evaluation:
- Laboratories, works and expositions
- Theoretical and practical partial exams
- used SW tools
- Proposed Architecture (explain it generally)}


Empresarial Architectures:
- TOGAF 
- DODAF


Terms:
- TOGAF
- DODAF
- Spring
- JavaEE
- RESTful / SOAP
- SQL
- NoSQL: DML
- JBoss
- Docker
- Angular
- Matriz Zachman
- PUB/SUB
- API GRAPHQl
- Git
- NodeJs
- Xml / Json
- XML - RPC
- JPA
- ORM \[Objet-Relational Mapping\]
- Bootstrap
- Azure DevOps
- Pipelines
- LAMP
- Jquery
- VueJs
- SOLID
- KISS
- DRY
- PL/SQL
- Kubernetes
- JSF
- REACT
- Hibernate
- WADL

**CAP Triangle**
![[TriangleCAP.png]]

**DATABASES:**
- ACID: Characteristics 
- SQL
- NoSQL
- InMemory: Uses Cached memory for increase speed.
- NewSql: Combine SQL and NoSQL.

**JSON:**
- Key - Value
- Arrays

**WEB Services:**
- Each Web service has a contract language, an IDL <small style="color:gray;">(Interface definition language)</small>
- *SOAP:*
	- Simple Object Access Protocol <small style="color:gray;">W3C: Whom Standardize all the Web</small>.
	- Use a lot of XML.
	- WSDL <small style="color:gray;">Web Service Description Language, it's an XMl Schema</small>.
	- UDDI <small style="color:gray;">Universal Description, Definition and Integration</small>.
	- Has QoS: It means that is Secure and it's fiable.
- *RESTful:*
	- Created by Roy Fielding, HTTP Creator.
	- It isn't an Standard, and yes this is a problem
	- Based a lot on HTTP
	- Resources -> An URI
	- Method: To manipulate resources <small style="color:gray;"><small>GET, POST, PUT, DELETE, CONNECT, TRACE, HEAD</small></small>
- *gRPC:*
	- Created by google.
	- CAll to Remote Procedures.
	- Used to define APIs and it's so fast to transmit data because is binary codification.
	- Use it when you are using thousands services.
	- Has an IDL called Protocol Buffers or Proto3.
- *GRAPHQL:*
	- Consult Language Based on Graphs.
	- More to the Frontend.
	- Has an IDL called Schema.
	- A lightest 
	
**MIME Types:** Standard types to represent data.

**PUB/SUB:**
- Send data to a client without client's petitions.
- Micro services fav.

**DevOPS:**
- Dev -> Developer.
- OPS -> Infrastructure.
- It's a Culture
- DevOPS Cicle:
	 ![[Pasted image 20240208170051.png]]
- Can make environment and the application pass through them just as it was a **pipeline**
- Pipeline: Has the responsibility of automatize the operations of the DevOPS cicle.
- IaC: Infrastructure as Code

**JQuery:**
- It's a JavaScript Library.
- Associated with AJAX <small style="color:gray;">Asynchronous Javascript and XML</small>

**Docker:**
- It's a container manager.
- Has no hypervisors 

**Kubernetes:**
- It's used as Orchestrator to manage the connection between containers.

**EJB:**
- Means Enterprise Java Beans.
- Used in JavaE or JakartaE.