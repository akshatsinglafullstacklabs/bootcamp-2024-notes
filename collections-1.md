## Topics Covered:
- List
- Stack
- Queue
- Set
- Deque
- ArrayBlockingQueue
- Interface Map _(Not in Detail)_
- toString() method overriding for Non_Primitives U.D. Classes
- HashCode() method overriding for Non_Primitives U.D. Classes
- IdentityHashCode() 
- .equals() method overriding for Non_Primitives U.D. Classes
- compareTo() method overriding for Non_Primitives U.D. Classes
- ==
- ArrayList
- Vector (Rarely Used)
- Common List Operations (CRUD methods)
- Internal Iteration (Using Streams)
  - Streams give us chained methods
- Coding Samples

#### Questions: 

- Is Map is a Collection?
- Name us the Java Collections
	- Maps do not fall under the category of Collections in Java
	- Because maps are key value pairs
		

#### **Collection**: 
-	Set (Sorted Set), List, Queue, Deque
#### **Map**: 
-	SortedMap


<br>

ADT (Abstract Data Type) is just a more generic word used in Computer Science.
Collections is more restricted towards Java and is the same as ADT.

Sets -> Eliminates Duplicates
Lists -> Keep Duplicates


## USAGES:
If 1D : Lists	
	If duplicated allowed : List
	If No Duplicates : Set
if FIFO structure : Queue
if LIFO : Stack

----------

# Object Equality

Hashcode gives us a Random Number generated from the VALUE Of the fields we have asked for (NOT MEMORY).
Hashcode generation is specific to the JVM. (2 Different JVM's can give same hashcode for different values).

_Hash based collections work on HashCodes._
.equals() compares the Hashcode.

_(**NOTE**: There is a remote possibility that the Hashcodes can Collide.)_

<br>

**_-	If 2 objects are equal their hashcode has to be same._**
**_-	If hashcodes are same, its not necessary that 2 two objects are equals._**


So, we would override .equals() method to property specify the requirements and usage of equating of objects at business level.


-> ALWAYS PROVIDE **equals()** AND **HashCode()** IMPLEMENTATION FOR THE OBEJCTS THAT WE CREATE (User Defined).
-> SAME FOR **toString()** and **toCompare()**

##### _NOTE: Avoid collections inside the toString();_


**identityHashCode()** is more like a _memory address Reference_ but not necessarily.
