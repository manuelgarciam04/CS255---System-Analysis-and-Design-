# CS255 - System Analysis and Design

Project Summary: DriverPass
The client for this project was Liam, the owner of DriverPass—a driving school struggling with administrative bottlenecks and a high student failure rate on DMV driving tests (around 65%). Liam and his internal IT specialist, Ian, needed a centralized, automated web and mobile management platform. The goal was to replace fragmented manual scheduling and record-keeping with an integrated system handling online lesson booking, instructor scheduling, vehicle tracking, secure payment processing across various service packages, and interactive DMV practice tests with automated scoring and analytics.

Areas of Strength
Translating broad, high-level business concerns into concrete, structured UML models was the strongest aspect of my deliverables. Specifically:

UML Activity & Sequence Modeling: In the System Design Document, mapping out the precise end-to-end interactions for lesson bookings and payment transactions clearly demonstrated how front-end requests communicate with business logic controllers and third-party APIs (such as payment gateways).

Requirements Traceability: The Business Requirements Document (BRD) clearly bridged Liam's operational pain points directly to functional requirements, ensuring every feature—from package tracking to automated test review—directly targeted student pass rates and administrative efficiency.

Areas for Revision & Improvement
If revising these documents, I would expand the error-handling and edge-case workflows within the architectural diagrams and class structures.

State Management for Incomplete Transactions: The initial sequence diagrams primarily modeled the "happy path" of booking and payments. Expanding the models to explicitly trace network timeouts, failed payment webhooks, or last-minute instructor cancellations would provide a more resilient blueprint for developers.

Database & Concurrency Constraints: I would refine the class diagram and database schemas to include explicit optimistic locking or concurrency handling to prevent double-booking instructors or vehicles during peak scheduling windows.

Interpreting User Needs & User-Centered Design
User needs were interpreted by decomposing Liam's high-level business goals into persona-based use cases (Students, Instructors, and Administrators):

Addressing the 65% Failure Rate: Rather than treating DriverPass purely as a logistical scheduling tool, the design prioritized an interactive practice test engine with immediate feedback, directly serving the student's need for test readiness.

Simplifying Instructor Logistics: Instructor availability and vehicle assignment workflows were designed to prevent overlaps automatically, eliminating administrative confusion.

Why User-Centered Design Matters:

Software that is technically sound but misaligned with actual user workflows results in low adoption, high error rates, and unresolved operational bottlenecks. Designing with the end user in mind ensures that business problems are solved at the root rather than just digitizing inefficient manual processes.

Future Software Design Approach & Strategies
Moving forward, my approach to systems analysis and design will center on an iterative, requirements-driven methodology:

Domain-Driven Decomposition: Break down complex systems into distinct bounded contexts (e.g., Identity/Auth, Scheduling, Billing, Assessment) before drafting architectural models.

Standardized Visual Modeling: Continue leveraging UML diagrams (Use Case, Activity, Sequence, and Class) in tools like Lucidchart to validate architectural logic before writing code, reducing costly structural refactoring downstream.

Traceability Matrices: Maintain clear alignment between user stories/functional requirements and technical components to ensure every architectural decision serves a verified stakeholder need.

Resilience & Edge-Case Modeling: Dedicate design phases specifically to non-functional requirements (NFRs)—focusing on concurrency, data integrity, security controls, and failure-recovery paths early in the system lifecycle.
