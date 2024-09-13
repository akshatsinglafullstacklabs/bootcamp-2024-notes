# Topics Covered

-   Generics
    -   Raw List
    -   Generic List Type
    -   Type Inference Java 7
-   Terminology for Generics:
    -   Method Argumet
    -   Method Definition
    -   Method Invocation
    -   Method Type
-   Non-Generic Box Class VS Generic Box Class
-   Generics with Limitation
-   Good Naming Conventions for Generics
-   Backward Compatibility with Generics

---

# Questions

-   Code LinkedList in Java
-   
-   


---


We must use generics for **type safety**

Collections never works with Primitives by desing. Only work with objects, that is why wrapper classes exist.

*Generics is a layer between the user and JAVA that ensures type safety. Java did not write Generics from scratch. Rather they built upon the existing collections code (Adding a layer of type checking to ensure type safety). Just like Typescript pre-processor for Javascript.*


---

#### Backwards Compatibility of Generics

Generics dont always mean that we ahve to give them some data type, we can also create Instances of that generic without specifying the data Types.

For e.g.

Box<E> 

I can all this as:
- Box< String > or Box< Integer >
  
Also i can do this

- Box objectName = new Box(new String("Mystring"));
But now we take away type safety from the code.


---

#### Terminology of Generics

**Generic Class / Interface:**
Instantiating with passing type argument we are doing generic type invocation.

Instantiating withOUT passing type argument we are doing RAW type instance for the Generic Type Class.

**Non - Generic Class / Interface:**
Non-Generic type instances because they do not provide generic DT rather allow specific Data Type.