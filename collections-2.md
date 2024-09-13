# Topics Covered

- Wrapper Classes
- AutoBoxing and Unboxing
  
_Java 4 in 2004 and Java 8 in 2014_

- Code Samples for Autoboxing and Unboxing with ArrayList 
- Other code samples of **ArrayList**
- Sys.out calling toString()
- Raw Maps
- InstanceOf
- Typecasting with maps and collections
- HashSet<>()
- TreeSet<>() Maps (All trees does sorting for us.)
- EntrySet
- created compareTo, toString
- Stack
- Queue
- Concurrent HashMap (**IMPORTANT**)
- 


---

### Questions:
- What Java version do you use?
- What features from this Java Version do you use frequently?
- How do you get a stack over flow error in Java?
  - _One way is because of **circular reference** when we are **using/Overriding toString() method**. If we call parent from the child and the parent is calling in the child then its a never ending loop and this leads to a StackOverFlowError_
- Difference between internal and external foreach loop?
  - _Internal:_
    -  _Less Control_
    -  _More Optimized as it delegates the task to the JVM, Allowing parallelism_
  - _External:_ 
    - _More Control over the Incremental Logic, termination Logic_
    - _Not the best usage of the JVM HW power._
- Stack Implementation (Brackets Question, Palindrome)
- **Code LinkedList** (_IMPORTANT_)

<br>

---

**Collections is a Utility class** with a number of static methods.


_NOTE : sout calls the toString for non-primitive date types. and if we do not write the toString method, then the java default implementation for toString for the non-primitive data types is called which prints the hashCode of the object._

<br>
<br>

Using Builders for User Defined classes is always good :-)


*ArrayList thread safe version is Vector.*

---
## MAPS

Map is not a collection
n rows and 2 columns
Key, Value Pair (_Key is Unique, Override of value happens for repeating Keys_)

<br>

Maps with Generics are Type Safe.
Maps without generics are not tye safe. (Dont throw compile time errors but are practically Useless).

Maps size gives the number of Key Value pair

**Collections are supposed to be Type Safe and that is why we always use them with Generics.**


***HashTable** O(1) are thread safe version of HashMaps.*

<br>
<br>

_**NOTE:**_
People write pre-processors. Dont come up with new processors all along.
_Typescript is a pre-processor for Javascript. It just fixes what Javascript has issues with and then converts the pre-processed written code into Javascript for browsers to run._


---

## SETS

TreeSets<> - always use super type for variable declaration i.e. Set< Type > 
Same for all other sets.


**HashSets** - eliminates the duplicates based on the equals and hashcode method implements

**TreeSets** - sorts the elements based on the compareTo method implementation, and also throws away the duplicates based on the same compareTo implementation.

- _TreeSets cannot have null value by default because nulls are not comparable. Since they are not comparable, tree set cannot organize them and keep a sorted collection._
- _Same with Tree Maps._

**NullPointerException** is thrown.

---

## STACK

LIFO
Bracket Matching Program uses Stack.

Makes a good candidate for interview.

---
## QUEUE

FIFO
Linked Lists (Non Thread Safe)
**Array Blocking is also a Queue** (and Threadsafe)
**Consumer Producer Pattern** is done with Array Blocking Queue.

---

## DEQUE 

Double Ended Queue
Both add and remove allowed from both ends of the pipe.

---

Concurrent version of Collections are better than Synchronized version of collections.
- **Sync. version** only allows just 1 thread to access the method at one time. Very SLOW.
- **Concurrent Versions** actually fight the real war and make the performance a lot better than Sync. Version. So usually we use Concurrent version of collections if we want to ensure thread safety.

