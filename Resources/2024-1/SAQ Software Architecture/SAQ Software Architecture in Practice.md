# Software Architecture (SfA) in Practice
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