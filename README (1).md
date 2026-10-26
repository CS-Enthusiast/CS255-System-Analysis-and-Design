# CS 255: Systems Analysis and Design
**Ehigie Ekata | Southern New Hampshire University**

This portfolio presents the analysis and proposed design for DriverPass, a driver-training business. It contains design documents rather than an implemented application.

## Portfolio documents

- [Project One: Business Requirements Document](CS255_Project_One_Business_Requirements_Ekata.docx)
- [Project Two: System Design Document](CS255_Project_Two_System_Design_Ekata.docx)

## Briefly summarize the DriverPass project. Who was the client? What type of system did they want you to design?

The client was DriverPass, a business that wanted to help students prepare for their driving exams through training packages, driving lessons, online classes, and practice tests. The project involved analyzing those needs and designing a web-based system that customers and staff could access from computers and mobile devices. Customers needed to manage their training and schedule lessons, while staff needed tools to manage reservations, accounts, and progress reports. The business requirements document identifies what the client needs, and the system design document translates those needs into UML diagrams and technical requirements.

## What did you do particularly well?

One strength of my design was considering what could go wrong during a booking instead of describing only a successful reservation. The activity and sequence diagrams include eligibility checks, scheduling conflicts, and failed database updates. The design requires the reservation, reserved hours, and audit entry to be saved together before the customer receives confirmation. It also distinguishes the customer receiving a lesson from the staff member who books it. These details make the design more useful to developers because they explain how to protect accurate schedules and records.

## If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?

I would improve the connection between individual business requirements and the system design by adding a requirements traceability table. Each requirement would receive an identifier and link to the relevant use case, diagram, and acceptance check. For example, preventing double bookings would connect to the scheduling activity diagram, the reservation sequence, and a test involving two simultaneous requests for the same driver or vehicle. I would also identify which items are confirmed client requirements and which are proposed choices awaiting approval. This would make omissions and the effects of requirement changes easier to identify.

## How did you interpret the user's needs and implement them into your system design? Why is it so important to consider the user's needs when designing?

I translated the client's requested tasks into user roles, workflows, and data relationships. For example, allowing a secretary to book for a customer led to separate customer and acting-user records, while package-specific training access led to enrollment records that preserve purchased hours and access rights. The design also connects progress reporting to practice-test attempts and lesson records. These needs were incorporated into the design rather than implemented in working software. Considering users is important because a technically correct system can still fail if it does not support their actual responsibilities, permissions, or everyday tasks.

## How do you approach designing software? What techniques or strategies would you use in the future to analyze and design a system?

I approach design by identifying the problem, the people involved, and the tasks the system must support before choosing technologies. I then use complementary models: use cases describe user goals, activity diagrams describe workflows and decisions, sequence diagrams describe communication, and class diagrams describe data and relationships. In future projects, I would combine stakeholder interviews with observation, prototype reviews, and written confirmation of requirements. I would review failure paths, accessibility, security, and acceptance criteria early. Keeping requirements, diagrams, and tests aligned would help the team evaluate changes and verify that the final implementation meets the client's needs.

