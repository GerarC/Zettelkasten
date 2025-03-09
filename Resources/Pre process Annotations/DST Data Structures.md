# 3 List, Stacks, and Queues

## 3.1 Abstract Data Types (ADTs)
An abstract data type (ADT) is a set of objects together with a set of operations. Abstract data types are mathematical abstractions; nowhere in an ADT’s definition is there any mention of how the set of operations is implemented. Objects such as lists, sets, and graphs, along with their operations, can be viewed as ADTs. For the set ADT, we might have such operations as add, remove, size, and contains. Alternatively, we might only want the two operations union and find, which would define a different ADT on the set.

There is no rule telling us which operations must be supported for each ADT; this is a design decision. Error handling and tie breaking (where appropriate) are also generally up to the program designer.

## 3.2 The List ADT
### 3.2.2 Simple Linked Lists
The linked list consists of a series of nodes, which are not necessarily adjacent in memory. Each node contains the element and a link to a node containing its successor. We call this the next link. The last cell’s next link points to nullptr.

The remove method can be executed in one next pointer change. Figure 3.2 shows the result of deleting the third element in the original list. The insert method requires obtaining a new node from the system by using a new call and then executing two next pointer maneuvers. The general idea is shown in Figure 3.3. The dashed line represents the old pointer. ^parrafo1


[[#^parrafo1]]