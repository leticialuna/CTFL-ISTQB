## 2 Testing Throughout the Software Development Lifecycle

## 2.1 Software Development Lifecycle Models

Lifecycle model describes the types of activity in each stage during the software development project and how the activities are related to one another.


## 2.1.1 Software Development and Software Testing

No matter which software development lifecycle model is chosen, test activities should start in the early
stages of the lifecycle, adhering to the testing principle of early testing.


There are 2 types:

- Sequential development models:

A sequential development model describes the software development process as a linear and sequential. It means the next phase should start when the previous is completed. typically require months or years for delivery to stakeholders and users.

Ex: Waterfall - requirements analysis, design, coding, testing
The V-model - integrates the test process throughout the development process, implementing the principle of early testing.
In this model, the execution of tests associated with each test level proceeds sequentially, but in some cases overlapping can happen.



- Iterative and incremental development models:

Incremental development: Involves changes that test a system in pieces, and then they are grow incrementally.
The size of these feature increments varies, with some methods having larger pieces and some smaller pieces

Iterative development models: occurs when groups of features are specified, designed, built, and tested together in a series of cycles, often of a fixed duration.


• Rational Unified Process: Each iteration tends to be relatively long (e.g., two to three months),
and the feature increments are correspondingly large, such as two or three groups of related
features

• Scrum: Each iteration tends to be relatively short (e.g., hours, days, or a few weeks), and the
feature increments are correspondingly small, such as a few enhancements and/or two or three
new features

• Kanban: Implemented with or without fixed-length iterations, which can deliver either a single
enhancement or feature upon completion, or can group features together to release at once

• Spiral: Involves creating experimental increments, some of which may be heavily re-worked or
even abandoned in subsequent development work

iterative and incremental models may deliver usable software in weeks or even days, but the complete requirement may be in months or year.


* Regression testing is increasingly important as the system grows.



## 2.1.2 Software Development Lifecycle Models in Context

Must be selected and adapted to the context of project and product, based on the project goal, the type of product, business priorities and risks.

ex: testing of a minor internal administrative system should be different from the development and testing of a safety-critical system.

Safaty-critical system: failure may result in death or serious injury to persons or serious damage to equipment

Foftware development lifecycle models themselves may be combined. 
For example, a V- model may be used for the development and testing of the backend systems and their integrations, while an Agile development model may be used to develop and test the front-end user interface (UI) and functionality.


why software development models must be adapted to the context:
- Difference in product risks of systems (complex or simple project)
- Many business units can be part of a project or program (combination of sequential and agile development)
- Short time to deliver a product to the market (merge of test levels and/or integration of test types in test levels)



## 2.2 Test Levels

Test levels are groups of test activities that are organized and managed together. Each test level is an instance of the test process

Test levels:

- Component testing
- Integration testing
- System testing
- Acceptance testing

Test levels are characterized by the following attributes:
• Specific objectives
• Test basis, referenced to derive test cases
• Test object (i.e., what is being tested)
• Typical defects and failures
• Specific approaches and responsibilities


Every test level is necessary an environment. 
Ex: Acceptance testing - production-like test environment
component testing - own development environment



COMPONENT TESTING:

Component testing (also known as unit or module testing) focuses on components that are separately testable.

Objective: reducing risks, find or prevent defects

Test basis
Examples of work products that can be used as a test basis for component testing include:
• Detailed design
• Code
• Data model
• Component specifications

Test objects
Typical test objects for component testing include:
• Components, units or modules
• Code and data structures
• Classes
• Database modules

Typical defects and failures
Examples of typical defects and failures for component testing include:
• Incorrect functionality (e.g., not as described in design specifications)
• Data flow problems
• Incorrect code and logic 


Component testing is usually performed by the developer who wrote the code. 

Often use the TDD technique.

TDD: Test driven development is highly iterative and is based on cycles of developing automated test cases, then building and integrating small pieces of code, then executing the component tests, correcting any issues, and re-factoring the code. This process
continues until the component has been completely built and all component tests are passing.




INTEGRATION TESTING:

Integration testing focuses on interactions between components or systems.

Test basis
Examples of work products that can be used as a test basis for integration testing include:
• Software and system design
• Sequence diagrams
• Interface and communication protocol specifications
• Use cases
• Architecture at component or system level
• Workflows
• External interface definitions

Test objects
Typical test objects for integration testing include:
• Subsystems
• Databases
• Infrastructure
• Interfaces
• APIs
• Microservices

Typical defects and failures
Examples of typical defects and failures for component integration testing include:
• Incorrect data, missing data, or incorrect data encoding
• Incorrect sequencing or timing of interface calls
• Interface mismatch
• Failures in communication between components or system
• Unhandled or improperly handled communication failures between components or system
• Incorrect assumptions about the meaning, units, or boundaries of the data being passed between components or system


Functional, non-functional, and structural test types are applicable.
Test make by developers
Such continuous integration often includes automated regression testing


SYSTEM TESTING

Focuses on the behavior and capabilities of a whole system or product
Often considering the end-to-end tasks the system can perform and the non-functional behaviors
Focus on fuctional and non-functional behaviour system
Validating that the system is complete and will work as expected.

System testing often produces information that is used by stakeholders to make release decisions. 
System testing may also satisfy legal or regulatory requirements or standards.


Test basis
Examples of work products that can be used as a test basis for system testing include:
• System and software requirement specifications (functional and non-functional)
• Risk analysis reports
• Use cases
• Epics and user stories
• Models of system behavior
• State diagrams
• System and user manuals

Test objects
Typical test objects for system testing include:
• Applications
• Hardware/software systems
• Operating systems
• System under test (SUT)
• System configuration and configuration data
Typical defects and failures

Examples of typical defects and failures for system testing include:
• Incorrect calculations
• Incorrect or unexpected system functional or non-functional behavior
• Incorrect control and/or data flows within the system
• Failure to properly and completely carry out end-to-end functional tasks
• Failure of the system to work properly in the system environment(s)
• Failure of the system to work as described in system and user manuals




ACCEPTANCE TESTING

The main objective of operational acceptance testing is building confidence that the operators or system
administrators can keep the system working properly for the users in the operational environment, even
under exceptional or difficult conditions.
Focuses on the behavior and capabilities of a whole system or product.

Objectives:
confidence in the quality of the system
Validating that the system is complete and will work as expected
Verifying that functional and non-functional behaviors of the system are as specified

It's not an objective to find defects at this part. Find many defects can be considered a risk for a product.


The activities:

- User acceptance testing: build confidence that the users can use the system to meet their needs and perform business processes with minimum difficulty, cost, and risk.

- Operational acceptance testing: The tests focus on operational aspects, like Testing of backup and restore, Installing, uninstalling and upgrading, Checks for security vulnerabilities, Performance testing

- Contractual and regulatory acceptance testing: Contractual acceptance testing is performed against a contract’s acceptance criteria for producing custom-developed software. The main objective of contractual and regulatory acceptance testing is building confidence that
contractual or regulatory compliance has been achieved.

- Alpha and beta testing: Alpha testing is performed at the developing organization’s site, not by the development team, but by potential or existing customers, and/or operators or an independent test team.
Beta testing is performed by potential or existing customers, and/or operators at their own locations.
Don't need alpha first to do.


Objective: See if everything is working as expected.


Test basis
Examples of work products that can be used as a test basis for any form of acceptance testing include:
• Business processes
• User or business requirements
• Regulations, legal contracts and standards
• Use cases and/or user stories
• System requirements
• System or user documentation
• Installation procedures
• Risk analysis reports



Typical test objects
Typical test objects for any form of acceptance testing include:
• System under test
• System configuration and configuration data
• Business processes for a fully integrated system
• Recovery systems and hot sites (for business continuity and disaster recovery testing)
• Operational and maintenance processes
• Forms
• Reports
• Existing and converted production data


Typical defects and failures
Examples of typical defects for any form of acceptance testing include:
• System workflows do not meet business or user requirements
• Business rules are not implemented correctly
• System does not satisfy contractual or regulatory requirements
• Non-functional failures such as security vulnerabilities, inadequate performance efficiency under
high loads, or improper operation on a supported platform


Acceptance testing is often the responsibility of the customers, business users, product owners, or operators of a system, and other stakeholders may be involved as well.



## 2.3 Test Types

FUNCTIONAL TESTING:

Functional testing of a system involves tests that evaluate functions that the system should perform.
The functions are “what” the system should do. Functional testing considers the behavior of the software.

-  Functional tests should be performed at all test levels

Technique: black-box


NON-FUNCTIONAL TESTING:

Non-functional testing of a system evaluates characteristics of systems and software such as usability, performance efficiency or security.

- should be performed at all test levels, and done as early as possible.

Technique: black-box
Ex: boundary value analysis for performance tests.


WHITE BOX TESTING:

Tests based on the system’s internal structure or implementation. 
Internal structure may include code, architecture, work flows, and/or data flows within the system.

When to use: At the component integration level
ex: white-box testing may be based on the architecture of the system, such as interfaces between components

Also check the code coverage.


CHANGE-RELATED TESTING:

When changes are made to a system, either to correct a defect or because of new or changing functionality, testing should be done to confirm that the changes have corrected the defect or implemented the functionality correctly.

There are 2 tests:

Confirmation testing: After a defect is fixed, the software may be tested with all test cases that failed due to the defect, which should be re-executed on the new software version. The purpose of a confirmation test is to confirm whether the original defect has been
successfully fixed.



Regression testing: It is possible that a change made in one part of the code, whether a fix or another type of change, may accidentally affect the behavior of other parts of the code. Regression testing involves running tests to detect these kind of defects.


* Confirmation testing and regression testing are performed at all test levels.
* regression testing is a strong candidate for automation. Automation of these tests should start early in the project


## 2.4 Maintence Testing

Maintenance is needed to preserve or improve non-functional quality characteristics of the component or system over its lifetime, especially performance efficiency, compatibility, reliability, security and portability.


The scope of maintenance testing depends on:

• The degree of risk of the change, for example, the degree to which the changed area of software
communicates with other components or systems
• The size of the existing system
• The size of the change

We can classify the triggers for maintenance as follows:

- Modification
- Migration

Impact analysis may be done before a change is made, to help decide if the change should be made, based on the potential consequences in other areas of the system.
It can use regression test.

Impact analysis can be difficult if:
• Specifications (e.g., business requirements, user stories, architecture) are out of date or missing
• Test cases are not documented or are out of date
• Tool support is weak or non-existent
