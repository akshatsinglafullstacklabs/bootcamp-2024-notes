# Topics Covered:

-   What is Exception
-   The Call Stack
-   catch-specify
-   


---


# Questions:

-   Why Use Exceptions and not If-else blocks?
    -   Unreadable
    -   Not Portable
    -   Non Scalable
    -   Concept of OOPS are used in Exceptions
        -   Every Catch is basically a sub class of exception
        -   All Exceptions can be caught using one super Exception class
    -   Exceptions are consistent across language
  
-   Why Do Exception Handling and not use Error Codes
    -   Same answer as above
-   what is different between Error and Runtime Exception?
    -   Error is at a JVM level, runtime exceptions are mostly because of the programmer logic mistake.
-   Can I catch error or Runtime Exception in Java
    -   Yes, Everything in java is catchable, but can we really do anything about it?
        -   No
-   ##### Swallowing an Error/Exception and Killing JVM till death
    -   Inteview Question
    -   Never swallow an Exception. Even the exceptionTrace wont spit in some cases of Error Catches, so its a big big no.
-   What is the difference between throws and throw
    -   Throws is the generator of the question and we dont need a catcher for this
    -   but if in a class I am throwing without that class being the producer with throws, then it needs to be enclosed within the catch block.
-   


---


Benefits of Using try{}catch(){}


If no methods in the call stack have available exception handling the program will crash.

<br><br>
_Try-Specify is not for Errors in Java. There is nothing we can do when we catch errors in Java._

All Things in exceptions are checked exceptions (managed under try and catch blocks) other than Runtime Exception.

_**so Runtime Exceptions and Errors are exempt from try-catch block.**_ _(You may swallow an Error/exception)_.
Then what is different between Error and Runtime Exception.?


---

Checked exception are thrown mostly to signal the user input mistakes and allow them to recover the app flow and stop it from crashing. 
They (Checked Exceptions) are the only ones who are a candidate of try and catch.


<br><br>

- **Checked Exceptions**: Cause because of the user input mistake and allows the program to recover allowing the user to try again.
- **Runtime Exceptions**: When the programmer makes a logic mistake in the code and we are not expected to recover from it. usually let the program crash.
- **Error**: the state where the JVM goes unhealthy.

---

#### Catch or Specify

Consider this like abstract classes. If a class extending an abstract class does not implement its abstract methods then I have to declare the class abstract.

If classA throws someException: it need not catch someException when it is thrown within this class.

If in classB i am using throw someException, then either I need to catch it or this class needs to say throws someException within its class declaration. 
Same for methods.

