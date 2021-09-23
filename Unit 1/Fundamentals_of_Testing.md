## 1) Fundamentals of Testing

## 1.1) What is Testing?

Software Test is a way to assess quality of the software, reducing the risks and failures in operation. 

The test process includes activities such as:

Test planning,
analyzing, 
designing and implementing tests,
reporting test progress and results, 
evaluating the quality of a test object,
verification of requirements, user stories or other specifications,
validation

1.1.1) Typical Objectives of Testing

The objectives of testing can vary, depending upon the context of the component or system being tested,
the test level, and the software development lifecycle model. These differences may include, for example:

During COMPONENT TESTING, one objective may be to find as many FAILURES as possible so that the underlying DEFECTS are identified and fixed early. Failures are caused by defects!

Another objective may be to increase code coverage of the component tests.

During acceptance testing, one objective may be to confirm that the system works as expected and satisfies requirements OR may be to give information to stakeholders about the risk of releasing the system at a given time.

But all tests are included objective such as:

To find defects and failures thus reduce the level of risk of inadequate software quality

To provide sufficient information to stakeholders to allow them to make informed decisions, especially regarding the level of quality of the test object

To comply with contractual, legal, or regulatory requirements or standards, and/or to verify the
test object’s compliance with such requirements or standards

1.1.2) Testing and Debugging

Debugging is an activity to find, analyze and fix defects. 
Normally developers do the debbuging, associated component and component test.
In Agile development and in some other software development lifecycles, testers may be involved in debugging
and component testing.


## 1.2 Why is Testing Necessary?

1.2.1) Testing’s Contributions to Success

Using appropriate test techniques can reduce the frequency of problematic deliveries, when are applied with the appropriate level of test expertise, in the appropriate test levels, and at the appropriate points in the software development lifecycle.


Examples:

- Testers involved in requirements reviews or user story refinement
- Testers working closely with system designers - while it is increasing
- Testers working closely with developers, understanding the code and testing it
- Testers verify and validate the software prior


1.2.2 Quality Assurance and Testing

Quality assurance and testing are not the same, but they are related by Quality Management.
Quality management includes all activities that direct and control an organization with regard to quality.

Quality Assurance: It is focused in PROCESS, to provide levels of quality will be achieved.

Testing: Test activities are part of overall software development or maintenance process.
Testing contributes to the achievement of quality in a variety of ways.


1.2.3 Errors, Defects, and Failures

A person can make an error (mistake), which can lead to a defect (fault or bug) in the software. 
If a defect is executed, it MAY cause a failure, but not necessarily in all circumstances!

Errors, defects and failures are differents!

Errors reasons: time pressure, human fallibility, insufficiently skilled, miscommunication, complexity of the code, complexity of design or architecture or technologies, misunderstanding about intra-system and inter-system interface

Failure can also be caused by environmental conditions, changing hardware. Ex: pollution.

Failure can be false negative or false positive.


1.2.4 Defects, Root Causes and Effects

The root causes defects are the first reason to create a defect!
Defect can be analyzed to identify their root causes.
All this make an effect!

Example: Product owner made an ambiguity at user story payment, so the code calculated it in a wrong way.
The client complainted about it!

Product owner mistake is the root cause -> it caused a defect in the code -> it caused an effect, which is customer complaint


## 1.3 Seven Testing Principles 

1) Testing shows the presence of defects, not their absence
It can show that defects are present, but cannot prove that there are no defects.

2) Exhaustive testing is impossible
Testing everything (all combinations of inputs and preconditions) is impossible!
It is necessary using techcniques to test efforts is better.

3) Early testing saves time and money
Find defects in static or dynamic test as early as possible helps to reduce or eliminate costly changes

4) Defects cluster together
A small number of modules usually contains most of the defects discovered during pre-release testing, or
is responsible for most of the operational failures.
Important to focus in the test effort!

5) Beware of the pesticide paradox
The same tests don't find any new defects.

6) Testing is context dependent
It is done differently in different contexts. 
For example: testing in an Agile project is done differently than testing in a sequential software development lifecycle project.

7) Absence-of-errors is a fallacy
It is impossible to find all possible defects - look principles 2 and 1, respectively.


## 1.4 Test Process

There is no universal software test process, but there are some common sets very important to achieve the success process.



## 1.4.1 Test Process in Context

There are included, but not limited to:

- Software development lifecycle and methodologies
- Test levels and test types
- Product and project risks
- Business domain
- Operational constraints, including but not limited to:
	o Budgets and resources
	o Timescales
	o Complexity
	o Contractual and regulatory requirements
- Organizational policies and practices
- Required internal and external standards


## 1.4.2 Test Activities and Tasks

A test process consists of the following main groups of activities:

- TEST PLANNING:
	Activities that define the objectives of testing and the approach for meeting test.

- TEST MONITORING AND CONTROL:
	It is a on-going comparison of actual progress against planned progress using any test monitoring metrics defined in the test plan. Test quality and results.

- TEST ANALYSIS:
	
During this part, the test basis is analyzed to identify testable resources and define a test conditions. Determines "what to test".

The major activities:
	Requirement specifications, such as business requirements, functional requirements, etc
	Design and implementation information, such as system or software architecture diagrams or documents, etc
	The implementation of the component or system itself, including code, database, interface
	Risk analysis reports, which may consider functional, non-functional, and structural aspects of the component or system

It can be useful to find defects such as:

	Ambiguities
	Omissions
	Inconsistencies
	Inaccuracies
	Contradictions
	Superfluous statements


Test techniques useful:
	black-box, 
	white-box,
	experience-based

to define more precise and accurate test conditions.

The identification of defects during test analysis is an important potential benefit, especially where no other review process is being used.
For example, techniques such as behavior driven development (BDD) and acceptance test driven development (ATDD)

- TEST DESIGN:

In this part, the test conditions are elaborated into high-level test cases and other testware. Defines "how to test".

Includes the following major activities:
• Designing and prioritizing test cases and sets of test cases
• Identifying necessary test data to support test conditions and test cases
• Designing the test environment, infrastructure and tools
• Capturing bi-directional traceability between the test basis, test conditions, and test cases

Good to find defects! It also uses techniques.

- TEST IMPLEMENTATION:

The testware necessary for test execution is created and/or completed.
Test design answers the question  “how to test?” "do we have everything for it?"

Includes the following major activities:
• Developing and prioritizing test procedures, and, potentially, creating automated test scripts
• Creating test suites from the test procedures and (if any) automated test scripts
• Arranging the test suites within a test execution schedule in a way that results in efficient test
execution 
• Building the test environment (including, potentially, test harnesses, service virtualization,
simulators, and other infrastructure items) and verifying that everything needed has been set up
correctly
• Preparing test data and ensuring it is properly loaded in the test environment
• Verifying and updating bi-directional traceability between the test basis, test conditions, test cases (until now same as design) + test procedures, and test suites

Test implementation and test design are often combined!

- Test execution:

Test suites are run in accordance with the test execution schedule.

includes the following major activities:

Recording the IDs and versions of the test item(s)
Executing tests either manually or by using test execution tools
Comparing actual results with expected results
Reporting defects based on the failures observed

- Test completion:

Collect data from completed test activities to consolidate experience, testware, and any other relevant information.

includes the following major activities:
• Checking whether all defect reports are closed, entering change requests or product backlog
items for any defects that remain unresolved at the end of test execution
• Creating a test summary report to be communicated to stakeholders
• Finalizing and archiving the test environment, the test data, the test infrastructure, and other
testware for later reuse

These activities look sequencial, but they can be implemented interatively.
Example: Agile development involves small iterations of software design and test that happen on a continuous basis, supported by on-going planning.


## 1.4.3 Test Work Products

Test work products are created as part of the test process. Just as there is significant variation in the way
that organizations implement the test process, there is also significant variation in the types of work
products, like names, organization and how they are managed.

Basically they are almost the same!


Differences between than:

Test planning work products:
typically include one or more test plans.



Test monitoring and control work products: 

Test monitoring and control work products typically include various types of test reports, including test
progress reports produced on an ongoing and/or a regular basis, and test summary reports
Test monitoring and control work products should also address project management concerns



Test analysis work products:

Test analysis work products include defined and prioritized test conditions, each of which is ideally bi-
directionally traceable to the specific element(s) of the test basis it covers.

## 1.5.1 Human Psychology and Testing

Testers and test managers need to have good interpersonal skills to be able to communicate effectively
about defects, failures, test results, test progress, and risks, and to build positive relationships with
colleagues.2.1 Software Development Lifecycle Models

ex: For the organization, defects found and fixed during testing will save time and money and reduce overall risk to product quality.
This is a benefit for testing.
Start with collaboration rather than battles. Remind everyone of the common goal of better quality
systems.


## 1.5.2 Tester’s and Developer’s Mindsets

Tester: A tester’s mindset should include curiosity, professional pessimism, a critical eye, attention to detail, and a motivation for good and positive communications and relationships.

Developer: Can have some elements of tester, but successful developers are often more interested in designing and building solutions than in contemplating what might be wrong with those solutions. It is hard to see their own mistakes.
