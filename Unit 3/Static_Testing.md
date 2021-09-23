## 3 Static Testing

## 3.1 Static Testing Basics

static testing assess the code or other work product being tested without actually executing the code or work product being tested.

It does static analysis and review.

static analysis is an important part of security testing. 
Static analysis is also often incorporated into automated software and distribution tools, for example in Agile development, continuous delivery, and continuous deployment.


Almost any work product can be examined using static testing (reviews and/or static analysis), for
example:

• Specifications, including business requirements, functional requirements, and security
requirements
• Epics, user stories, and acceptance criteria
• Architecture and design specifications
• Code
• Testware


## 3.1.2 Benefits of Static Testing

enables the early detection of defects before dynamic testing is performed
ex:  requirements or design specifications reviews

It is also cheaper to find defects before dynamic testing



## 3.1.3 Differences between Static and Dynamic Testing

They have the same objectives - assess the quality of product work and find defects as soon as possible. They complete each other, but they find different types of defects.

Static testing find defects directly, instead of identify failures caused by defects while the software is running. 
Static testing may be able to find the defect with much less effort.
static testing can be used to improve the consistency and internal quality of work products, while dynamic testing typically focuses on externally visible behaviors.


Ex using static testing:

Requirement defects - ambiguites or contradition
Design defects -inefficient algorithms or database structures
Coding defects - variables with undefined values, variables that are declared but never used
Incorrect interface specifications
Security vulnerabilities - buffer overflow

** most types of maintainability defects can only be found by static testing



## 3.2 Review Process

Reviews vary from informal to formal.

Informal: reviews are characterized by not following a defined process and not having formal document
Formal: reviews are characterized by team participation, documented results of the review, and documented procedures for conducting the review.


Formality: 
	life cycle
	maturity of development process
	complexity of work product
	legal or regulatory requirements
	need for audit trail
	
	
## 3.2.1 Work Product Review Process	

Planning
Initiate review
Individual review
Issue communication and analysis
Fixing and reporting


## 3.2.2 Roles and responsibilities in a formal review

Author
• Creates the work product under review
• Fixes defects in the work product under review (if necessary)

Management
• Is responsible for review planning
• Decides on the execution of reviews
• Monitors ongoing cost-effectiveness

Facilitator (often called moderator)
• Is often the person the success of the review depends
• Ensures effective running of review meetings
• Mediates, if necessary, between the various points of view

Review leader
• Takes overall responsibility for the review
• Decides who will be involved and organizes when and where it will take place

Reviewers
• May be subject matter experts, persons working on the project, stakeholders with an interest in
the work product, and/or individuals with specific technical or business backgrounds
• Identify potential defects in the work product under review
• May represent different perspectives (e.g., tester, developer, user, operator, business analyst,
usability expert, etc.)

Scribe (or recorder)
• Collates potential defects found during the individual review activity
• Records new potential defects, open points, and decisions from the review meeting


** In some review types, one person may play more than one role
** Due the tools advance, sometimes there is no need for a records


## 3.2.3 Review Types

one of the main objectives is to uncover defects. 
All review types can aid in defect detection, and the review type should be based on the project.


Types:

Informal review: 
	Main purpose: detecting potential defects



Walkthrough:
	Main purposes: find defects, improve the software product, consider alternative implementations, evaluate 		conformance to standards and specifications
	Can be formal or informal
	Scribe is mandatory



Technical review:
	Main purposes: gaining consensus, detecting potential defects
	Individual preparation before the review meeting is required
	Potential defect logs and review reports are produced
	Scribe is mandatory

	
Inspection: 
	Main purposes: detecting potential defects, evaluating quality and building confidence in the work
product, preventing future similar defects through author learning and root cause analysis
	Metrics are collected and used to improve the entire software development process
	Scribe is mandatory
	led by a trained facilitator



## 3.2.4 Applying Review Techniques

Examples of different individual review techniques

1) Ad hoc
	reviewers are provided with little or no guidance on how this task should be performed.
	
2) Checklist-based
	A review checklist consists of a set of questions based on potential defects, which may be derived from experience.
	
3) Scenarios and dry runs
	A scenario-based review supports reviewers in performing “dry runs” on the work product based on expected usage of the work product.
	

4) Perspective-based ** the most effective technique
	In perspective-based reading, similar to a role-based review, reviewers take on different stakeholder viewpoints in individual reviewing.
	ex: end user, marketing, designer, tester, or operations.
	ex: tester would do acceptance tests to see the performing a perspective-based reading on a requirements
	
A key success factor is including different stakeholder viewpoints appropriately, based on risks

5) Role-based
	evaluate the work product from the perspective of individual stakeholder roles. 
	Typical roles include specific end user types (experienced, inexperienced, senior, child, etc.)
	Specific roles in the organization (user administrator, system administrator, performance tester, etc.)
	The same principles apply as in perspective-based
	
## 3.2.5 Success Factors for Reviews

People-related success factors for reviews include:

• The right people are involved to meet the review objectives
	for example, people with different skill sets or perspectives, who may use the document as a work input
• Testers are seen as valued reviewers who contribute to the review and learn about the work product, which enables them to prepare more effective tests, and to prepare those tests earlier
• Participants dedicate adequate time and attention to detail
