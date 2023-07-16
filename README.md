Dear Sir/Madam.

Thank you very much for this opportunity to show you my CV.

Please note that I use the pseudonym 'Paul Greer' in order to comply with your anonymity rules.

This CV is much easier to read at GitHub, and all the demonstration files are there too:

https://github.com/PaulGreer1/CV_295797_JunSoftDev

Kind regards,

Paul Greer

# Curriculum Vitae - 295797 - Junior software developer

This CV demonstrates the following skills:

- Clean architectures using variations of MVC, MVVM, OOP, etc..
    - Loose coupling of components for easier development, maintenance and testing.
    - Registration of controller event handlers for notification of events of interest.
    - In-memory storage of input and output data using the same object as that used for registration/notification, to enable easy access by various components of the system.
    - Dependency injection.

- Test-driven development (TDD)
    - Specification and implementation.
    - The identification of conditions which form the basis for unit tests, and the declaration of these conditions as tautologies in order to drive the first set of reasoned pseudocode blocks which bring about post-conditions before implementation in programming language.

https://github.com/PaulGreer1/TheGardenersWeb/blob/main/database/MethodSpec-getNewId.md

https://github.com/PaulGreer1/cinema-tickets/blob/main/specification/cinema-tickets-ui.txt

- Automated test suites
    - Ensuring all code works as expected before deployment.
    - Organisation of unit tests according to classes.
    - Using JUnit to perform unit testing as part of the compilation process.

- Continuous deployment environment
    - Automated CICD pipelining with AWS Microservices and Git.

- Programming languages
    - Java
    - Python
    - PHP, CSS, HTML

- Full stack development of web applications

- RESTful APIs

- Relational databases (MySQL) and SQL

Part 1 of this CV includes projects which demonstrate these skills. I give links to any code available at GitHub, so you can download and run it in your IDE.

Part 2 is a summary of my education. This includes a BSc Degree in Computer Science, Mathematics and Systems Analysis.

# Part 1: Projects and demonstrations

### Project: TheGardenersWeb 2022 - 2023

This project demonstrates the following skills:

- Programming languages: Java

https://github.com/PaulGreer1/TheGardenersWeb

https://github.com/PaulGreer1/TheGardenersWeb/tree/main/src/main/java/com/strongcoffee/tgw

- Clean architectures

- Registration of event handlers for notification of events of interest

- In-memory storage of input and output data for use by various components

- Relational databases: theory and practice: SQL, MySQL. The following demonstrates how I designed the schema and implemented the database for the TheGardenersWeb database:

https://github.com/PaulGreer1/TheGardenersWeb/blob/main/database/StatementOfDataRequirements.md

- RESTful APIs

#### Overview

This is the server component of the TheGardenersWeb system. It is deployed to an AWS Lambda compute service from where it provides database read/write services to clients. This app uses a Registrar object to provide an event and handler registration/callback facility. The Registrar also provides an input and output data storage and retrieval facility for other components in the system.

The Gateway class simulates the reception of HTTP requests from clients, and invokes the handleRequest() method defined in the Handler class. The Gateway object also creates the Handler object, which creates other components such as a Registrar which stores request and response data for use by various components throughout the process. The Registrar also manages the notification of event handlers as user interface (UI) events occur. The Controller manages the registration of its event handlers for UI events.

Please download and inspect the source code from:

https://github.com/PaulGreer1/TheGardenersWeb

![](https://github.com/PaulGreer1/TheGardenersWeb/blob/main/REQUEST_RESPONSE_SEQUENCE_DIAGRAM.png)

### Project: AwsCicdAutoPipeline 2022 - 2023

This project demonstrates the following skills:

- Automated CICD pipelining: AWS CodePipeline, CodeCommit, CodeBuild, CloudFormation, Amazon CloudWatch, S3

https://github.com/PaulGreer1/AwsCicdAutoPipeline

#### Overview

Our software development and delivery system includes an automated pipeline which compiles, packages and deploys software artefacts, and is central to the continual integration and continuous deployment (CICD) of our Java server.

An AWS CodePipeline service provides the stages, transitions and executions for a 'source-compile-package-deploy' sequence. From a Git push in the local development environment, to the final remote deployment by the AWS CloudFormation service, I use AWS microservices to manage and automate the procedure. I have ensured that changes in the CodeCommit repository are detected from source push, not from CodeBuild polling.

Please read all the details at GitHub:

https://github.com/PaulGreer1/AwsCicdAutoPipeline

The following link shows the overall development and delivery system:

https://github.com/PaulGreer1/TheGardenersWeb/blob/main/CICD.png

The following diagram shows the automated pipeline:

![](https://github.com/PaulGreer1/AwsCicdAutoPipeline/blob/main/AwsCicdAutoPipelineInSdds.png)

### Project: Ripples 2019 - 2020

This project demonstrates the following skills:

- Programming languages: Python

#### Overview

Animated model of raindrops landing on a gently flowing river. An initial investigation into game theory using Python's Turtles module. After this I moved on to Java/LibGDX so that I could create more powerful multi-agent software simulations of real-world phenomena.

https://github.com/PaulGreer1/Ripples

![](https://github.com/PaulGreer1/Ripples/blob/main/PYTHON_RIPPLES_00001.png)

### Project: WebsiteLamp 2018 - 2022

This project demonstrates the following skills:

- Programming languages: PHP, SQL
- Front-end web technologies: HTML, CSS
- Full stack development of web applications

https://github.com/PaulGreer1/WebsiteLamp

#### Overview

This is a powerful Linux-Apache-MySQL-PHP (LAMP) website with tools for membership, customer relationship management (CRM), brochure, financials, etc.. I use my own proprietary PHP-based model-view-controller (MVC) system. Take it, install it, enjoy it!

This repository will start you off with the following website:

https://www.ukappcoder.com/index.php

The HTML output from any particular app is generated by the app's Content.php file. The output is styled by the three CSS files in the root directory.
The site is powered by a set of PHP/MySQL web apps. Each app has an MVC structure, and includes the following mimimal set of files:

- Config.php
- Content.php
- controller.php

Use the top level Config.php file to configure the system for your server, then copy this file to all the other app directories.

Read all the details and get all the source code at GitHub:

https://github.com/PaulGreer1/WebsiteLamp

![](https://github.com/PaulGreer1/WebsiteLamp/blob/main/UKAPPCODER_002.png)

# Part 2: Education

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
