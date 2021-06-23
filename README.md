## 1) Fundamentals of Testing

## 1.1) What is Testing?

Software Test is a way to assess quality of the software, reducing the risks and failures in operation. 



The test process includes activities such as:

Test planning,
analyzing, 
designing and implementing tests,
reporting test progress and results, 
evaluating the quality of a test object,
verification of requirements, 
user stories or other specifications,
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



