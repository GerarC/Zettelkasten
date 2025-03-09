## Deployment diagram
- Show localization of the components
- Used element are:
	- components: the same component
	- Node (Where the component is): a cube that represents a piece of hardware in the system
	- Association: A line that link nodes
- Uses:
	- Embebed systems
	- Client-Server systems
- Pros:
	- Show a node set and its relations
	- Used to describe the static deployment view
- Cons:
	- Possible hardware failing because of the modeling
- Stereotypes:
	- `<<Device>>`: a node that represent a physical device like a computer, a mobile or servers and more
	- `<<Deployment>>`: It's a dependency relation that describes a artifact location. Can be associated to one or more artifacts
	- `<<Artifact>>`: a classifier that represents a physical system like a source, a library, executable script or Web Archive.
- Node Hierarchy
- Execution Environment
- Manifest

<br/>

> [!note] Note about a deployment diagram
> ~~~ mermaid
> graph TD;
> ECommerce[E-Commerce] --> MCommerce[M-Commerce]
> ECommerce --> TCommerce[T-Commerce]
> ~~~

<br/>
<p style="margin: 10em; background-color: red;"></p>

## Software Pattern
**Pattern**
- Creational
- Structural 
- Behavioral 


### POSA (Pattern Oriented Software Architecture)
- Architecture definition
- POSA Book
- Dataflow Based
- Data-Centric systems (Repositories)
- Implicit invocation
- Layered
- Object oriented
- Microkernel
- MVC
- Message Queues and Streams
- Distributed systems (Brokers): 
	- Middlewares
- Service Oriented
- Filter-Pipe: implemented in pipe terminal

### Broker
- Definition
- Technologies: 
	- Message
	- RPC
	- Distributed objects

### Ports
- Well known ports: 0-1023
- Registered ports: 1024-49151
- Dynamic ports: 49152-65536

### CORBA
- Means: Common Object Request Broker Architecture
- It works because IDLs
- createds an Stub and a Skeleton

### gRPC
- Remote Process Control of google
- uses and idl called proto3

## Models
 - Client server
 - Model with intermediary:
	 -  Proxy/cache
	 - Multilevel
- Peer-to-peer

## Architectural Style
- Refers to the overall design and organization of a software system.
- Some styles:
	- Micro-services
	- Event-Driven
	- Layered
	- Service-Oriented
	- Domain-driven
	- Data-Centric
	- Component-based
 
### POSA Pattern
- MicroKernel

### Brute Terminal
a monitor and keyboard


## Evolution for C/S
- Monolitic
- C/S: Desktops productivity apps
- C/S three layered: On premise enterprise apps e.g. CRM, ERP 
- C/S N layers: APS Hosted enterprise apps
- SOA: SaaS
- MS / Serverless


## Services
- Server Process: Provider
- Client process: consumer
- A clair separation.
- Asymmetric Protocols
- Transparency of locality 
- Platform independency
- Communication based on messages
- Growing
- Security

### Middleware


## REST


## Codification codes
ASCII
EBCD
xmlns -> xml name space



High cohesion low coupling

### ROA architecture
**HATEOAS**

### Idioms
## EJB (Enterprise Java Beans)

- Stateful:
- Stateless:
- Message Driven Bean:
	- Send messages between layers
- Timer Session Bean:
- Singleton
--------
- ### WebRTC

### HTTP
- HTTP/1.1:
	- Petition redundace
	- HOL o HOLB
	- Latency on resource charging
	- security breaches
	- Unique connection over TCP
- HTTP/2:
	-  header compression
	- Binary data in headers
	- Connection multiplexing

# Web Sockets
- Derived on HTTP
- It's a standard for web communication 
- Bidirectional protocol
- Full-duplex
- Web sockets are standardize by W3C in RTC6455
- Better than Ajax and Comet
- Websocket API:
	- 

### Polling
- It's near to real time 
- Browser searches http requests in regular intervals of time.
- event can occur between browser searches

