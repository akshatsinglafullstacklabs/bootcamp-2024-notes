# Topics Covered:

-   Wildcards
    -   Heirarchy
-   PECS
-   Type Erasure

# Questions:


-   When to use T vs when to use '?'
    - if we are just consuming from the producer we use '?'
    - otherwise T is fine   
    - Usually ? is used in the generic methods and T is used in generic classes



---

Passing a **final class** in Generic bounds is not technically adding any value.


Extends also means implements in Generics.

Generics is all about assignments and who can work with whom.

---
### Wildcards

Wildcards are mostly used in Collection (Maps Included :-)).

#### PECS (Producer Extends, Consumer Super)
_concept only for wildcards_

we have 2 types of Variables 'in' and 'out'

in - this is what we pass in - producer of info - producer extends
out - this is what we get out - consumer of info - consumer super

write into the consumer and read from the producer

we as devs consume from producer
we as devs produce into consumer

Producer:

- for producer data structures we use extends (Upper Bounds) - Data Structure produces and we consume (we can read only from these)
- *no writes allowed*, only reads. (Only consuming is allowed, since I as a developer am consuming the data and the list itself is the producer (producer data structure))

Consumer:

-  we use lower bounds (super)
-  read is allowed in super. anything writable is read also.
-  write- able and read-as-objects        
-  


---

# Typer Erasure

