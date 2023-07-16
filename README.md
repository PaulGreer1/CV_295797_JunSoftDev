# Curriculum Vitae 295797_JunSoftDev_16-07-2023

This CV is much easier to read at GitHub, and all the demonstration files are there too:

https://github.com/PaulGreer1/CV

This CV demonstrates the following skills:

- Clean architectures using variations of MVC, MVVM, OOP, etc.. Loose coupling of components for easier development, maintenance and testing. Registration of event handlers for notification of events of interest for controller event handlers. Storage of input and output data with the same object used for registration/notification, to enable easy access by various components of the system.

- Test-driven development (TDD): specification and implementation. The identification of conditions which form the basis for unit tests, and the declaration of these conditions as tautologies in order to drive the first set of reasoned pseudocode blocks which bring about the conditions before implementation using programming languages.

- Automated test suites: ensuring all code works as expected before deployment. Organisation of unit tests according to classes. Using JUnit so that tests are performed as part of the compilation process.

- Continuous deployment environment: Automated CICD pipelining with Git

- Programming languages: Java, Python, PHP

- Full stack development of web applications

- RESTful APIs

- Relational databases (MySQL) and SQL

Part 1 of this CV includes projects which demonstrate these skills. I give links to any code available at GitHub, so you can download and run it in your IDE.

Part 2 is a summary of my education. This includes a BSc Degree in Computer Science, Mathematics and Systems Analysis.

## Part 1: Projects and demonstrations









### Project: TheGardenersWeb 2022 - 2023

This project demonstrates the following skills:

- Programming languages: Java

https://github.com/PaulGreer1/TheGardenersWeb/tree/main/src/main/java/com/strongcoffee/tgw

- Relational databases: theory and practice: SQL, MySQL

https://github.com/PaulGreer1/TheGardenersWeb/blob/main/database/StatementOfDataRequirements.md

- Test automation techniques and tooling: Test-driven development, JUnit

https://github.com/PaulGreer1/TheGardenersWeb/tree/main/src/test/java/com/strongcoffee/tgw

#### Overview

This is the server component of the TheGardenersWeb system. It is deployed to an AWS Lambda compute service from where it provides database read/write services to clients. This app uses a Registrar object to provide an event and handler registration/callback facility. The Registrar also provides an input and output data storage and retrieval facility for other components in the system.

The Gateway class simulates the reception of HTTP requests from clients, and invokes the handleRequest() method defined in the Handler class. The Gateway object also creates the Handler object, which creates other components such as a Registrar which stores request and response data for use by various components throughout the process. The Registrar also manages the notification of event handlers as user interface (UI) events occur. The Controller manages the registration of its event handlers for UI events.

![](https://github.com/PaulGreer1/TheGardenersWeb/blob/main/REQUEST_RESPONSE_SEQUENCE_DIAGRAM.png)














## Part 2: Education

BSc Degree in Computer Science, Mathematics and Systems Analysis from a UK university.

### Computer science

#### Relational databases: theory and practice

Data requirements analysis ~ Relational theory ~ Entity relationship modelling ~ Logical schema creation ~ Referential integrity ~ Normal forms ~ Database design and implementation ~ SQL ~ Constraints

#### Modelling computer processes

Finite automata ~ Automata with memory ~ Language and grammar creation ~ Reasoned programming ~ Object interaction ~ Concepts of concurrency ~ Programming concurrency ~ Threads

#### Computing: an object oriented approach

Classes and objects ~ Inheritance ~ Modelling, designing and implementing software systems ~ Structural models ~ Invariants ~ Computing and networks

#### Building blocks of software

Data types ~ Sets ~ Binary trees ~ Formal logic ~ Pre-, mid- and post-conditions ~ Rules of inference ~ Recursion ~ Algorithm efficiency ~ Mathematical induction ~ Recurrence systems

### Mathematics

#### Exploring mathematics

Sequences ~ Conics ~ Matrix transformations ~ Calculus ~ Taylor polynomials ~ Complex numbers ~ Number theory ~ Groups ~ Proof and reasoning

#### Using mathematics

Functions ~ Modelling with sequences, matrices and vectors ~ Differential equations ~ Growth and decay ~ Chance ~ Variation ~ Estimating

### Systems analysis

#### Understanding system complexity

Mess analysis ~ Cause and effect ~ Positive feedback loops ~ Dynamic equilibrium ~ Chaos ~ Lag ~ Control loops ~ System dynamics ~ Stock and flow ~ Software simulation (NetLogo)
