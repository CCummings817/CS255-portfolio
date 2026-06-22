# CS 255 System Analysis and Design Portfolio

Carrie Cummings | Southern New Hampshire University

This repository contains artifacts from CS 255: System Analysis and Design. The two documents included here represent the full arc of the systems analyst role, from gathering and documenting what a client needs, to designing the system that meets those needs.

**Documents included:**
- Business Requirements Document (BRD) -- CS 255 Project One
- System Design Document (SDD) -- CS 255 Project Two

---

## Project Reflection

**Briefly summarize the DriverPass project. Who was the client? What type of system did they want you to design?**

The client was DriverPass, a company founded by Liam to address a real gap in driver education. Too many students were failing their DMV driving tests because they were relying on outdated practice tests rather than current, structured preparation. DriverPass wanted a cloud-based web application that would allow customers to create accounts, select training packages, take online classes and practice exams, and schedule behind-the-wheel driving lessons with professional drivers. The system also needed to support internal staff, including the owner, secretary, IT officer, and drivers, each with role-appropriate access and tools.

**What did you do particularly well?**

I think I did my strongest work on the functional and nonfunctional requirements in the BRD. I was thorough and precise about what the system needed to do and why, grounding each requirement in something the client actually said or implied during the interview. I was also intentional about using consistent "shall" language throughout, which kept the requirements actionable rather than vague. On the design side, the sequence diagram came together well. It clearly shows the two alternative flows for scheduling a lesson and illustrates how information moves between the customer, the system, the database, and the secretary.

**If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?**

I would go back and strengthen the written narrative in the system design document. Because the course scope focused heavily on the UML diagrams themselves, the written sections of the SDD ended up leaner than I would have liked. If I were revising it, I would add more context around each diagram, walking through a user story for each one, so that a developer picking this up cold could understand not just what the diagram shows but why the design decisions were made the way they were.

**How did you interpret the user's needs and implement them into your system design? Why is it so important to consider the user's needs when designing?**

I started with the client interview transcript and worked from there, pulling out explicit requirements but also reading between the lines for things Liam described as problems without framing them as features. For example, the concern about duplicate records across servers informed the decision to restrict offline data modification, even though Liam did not frame it as a technical requirement. That kind of interpretation is exactly why centering the user matters. A system that technically works but does not map to how real people use it will fail in practice no matter how clean the code is. The user's needs are not just input -- they are the standard against which the whole design should be evaluated.

**How do you approach designing software? What techniques or strategies would you use in the future to analyze and design a system?**

I approach design iteratively, starting broad with the problem space before narrowing into solutions. In this course, that looked like starting with the interview, moving into requirements documentation, and then using UML diagrams to model the system at different levels of abstraction. Going forward, I would lean more into use case and sequence diagrams early in the process because they force you to think about user interactions concretely before making structural decisions. I would also build in more explicit checkpoints for validating requirements with the client before moving into design, the kind of early feedback loop that catches misalignments before they become expensive to fix.
