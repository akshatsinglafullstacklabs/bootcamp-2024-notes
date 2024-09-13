# Table of Contents:

- What is docker?
- Basic JDBC Architecture
  - JDBC Class Heirarchy
  - JDBC Drivers - 4 types
    - only 2 main
- Steps to work with database using jdbc
- Creating Database and Tables
  - Using Commandline
  - using Application
- Connecting to JDBC database from java applicaiton code
- Executing Statements from the code
  - Statement
  - Pepared Statement
  - Callable Statement
- Aspects to cover while executing Statements
  - Security - SQL injection
  - Performance
  - Parameter Binding
  - Code Readability and Mainenance
  - Hanlding complex queries
  - Batch Processing
  - Flexibility
- When to use Statement and when to use preparedStatement
- Statement VS Prepared Statement
- Callable Statement
- Permission Requirements
- Parsing Query Results
  - Result Set
  - Updateable result set
- Parsing Metadata
- Transactions
  - Using AutoCommit
  - <https://docs.oracle.com/javase/tutorial/jdbc/basics/transactions.html>
  - Connection Pooling
  - Transactions


# Questions:

-   Connection Pooling is Critical
    -   A lot of questions on this topic.
-   Left Outer Join, Right outer join
-   Propagation Levels
-   Isolation Levels
-   Locking mechanisms


---

- Regular Statement
- Prepared statement -> precompiled
  - Protects from SQL Injections



---

## Connection Pooling

- Object Pool Pattern
- Benefits of Connection Pools

---

## Transactions

Transactions must be complex to maintain Atomicity.
  - Does it keep a copy of everything that it's updating and then push the final version after last update 
  - Read about Isolation in Translation.
- Save points are not used at the Enterprise level we work with but are there if we are doing something of that need.
- ACID Features
  - Atomicity
  - Consistency
  - Isolatiuon
  - Durable