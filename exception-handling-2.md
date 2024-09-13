# Topics Covered:
-   finally block
-   converting checked exceptions to unchecked exceptions
    -   Done by Spring framework
-   User Created exception classes and error classes
-   Catching more than 1 exception with 1 exception handler
-   encapsulating checked/user created exceptions with runtimeExceptions
    -   Exception Translation / Exception Chaining
-   Reading Exception stack traces
-   closable and autoclosable
-   



---


# Questions: 

-   3 Types of exceptions that occur in Java?
    -   Error,  Checked Exception, Runtime Exception
-   When to throw Unchecked Exception VS Checked Exception?
-   What is Catch-Specify Requirement?
-   Which exception type falls under catch-specify requirements?
-   When do we use which exception?
-   Can we catch Error or Runtime Exception?



---

We normally would use only clean up stuff in finally whihc is supposed to execue anyhow.


---

Try - catch - **finally** block:
-   We will reach finally in Exceptions
-   May or may not hit finally in Error depending if the JVM is alive or not
-   


#### Try-with-resource

We use try-with-resource implementing an interface autoclosable, this saves resources if the developer forgets to close the connection in the finally block.

sometimes the developer would forget to add a finally block that is why we now only use try with resource in the industry like a mandate.

Prevents **resource-leak**