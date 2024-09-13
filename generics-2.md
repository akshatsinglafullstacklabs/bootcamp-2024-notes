# Topics Covered

-   Compile Time Type Safety / Static Type Checking
-   Parametrized Type VS Raw Type
-   Generic Methods 
    -   Terminology
    -   In Class Examples
-   Generic Bounds
-   Multiple Bounds
-   


Questions:

-   Discuss the before and after of generics? Or Explain the elimination of type casting in collections using Generics.
-   Raw Type, Type Parameter, Type Argument, Type Invocation
-   What did generics help with?
    -   Compile Time Type Safety
    -   Elimination of Type Casting
    -   DRY (Dont Repeat Yourself)
-   Writing Generic methods from Normal Methods
-   Relation between Generics

---

After Type invocation with type arguments, we create a **Parameterized type** of generic type (class/interface).


---

### Generic Methods

- Generic Methods only have generic behaviour
- Generic Class have generic state as well as generic behaviour.

---

### Multiple bounds

Cannot have more than 1 class in the generic Type parameter but can extend more than 1 interface.

Multiple inheritance and Multiple bounds are very much related.

---

### Relationship between Generics.

Type arguments in a relationship does not necessarily mean that their generics are in a relationship.

As Long as the internals (Type arguments) are same the generics are connected. Keep in mind the concept of Inheritance. The subclasses need to be extending the parents. But at the same time their Type arguments needs to be in consideration.

Eg. Collection< String > -> List< String > -> ArrayList< String >
