---
{"dg-publish":true,"permalink":"/1-mw-coe-420/w4-ch3/"}
---

# Chapter 3 – Agile Software Development

#software-engineering #agile #scrum #XP #methodology

---

> [!question] Why is rapid development crucial today? 
> Businesses operate in **fast-changing environments**. It's practically impossible to produce a stable, complete set of software requirements upfront.

## What is Agile Development?

Agile development flips the traditional model on its head. Instead of completing each phase sequentially, agile **interleaves** specification, design, and implementation.

> [!abstract] Core Characteristics of Agile
> 
> - **Incremental versions** — The system is developed as a series of releases
> - **Stakeholder involvement** — Customers participate in version specification and evaluation
> - **Frequent delivery** — New versions are delivered regularly for feedback
> - **Tool support** — Extensive use of automated testing tools
> - **Minimal documentation** — Focus on working code, not paperwork

---

## Plan-Driven vs Agile Development

| Aspect        | Plan-Driven                              | Agile                                                              |
| ------------- | ---------------------------------------- | ------------------------------------------------------------------ |
| **Planning**  | Outputs planned in advance at each stage | Outputs decided through negotiation during development             |
| **Iteration** | Occurs _within_ activities               | Occurs _across_ specification, design, implementation, and testing |
| **Model**     | Waterfall                                | Inherently incremental<br>Ex. Scrum, XP                            |
![image-9.png|400x304](/img/user/1%20-%20MW%20COE420/img/image-9.png)

> [!note] Important Distinction Plan-driven doesn't automatically mean waterfall. You can do plan-driven incremental development where iteration happens within individual activities.

---

## The Five Principles of Agile Methods

1. Customer involvement
2. Incremental delivery
3. Team develop own ways of working
4. Embrace change
5. Maintain simplicity 

---

## Agile Development Techniques

### Extreme Programming (XP)

> [!example] What is XP? 
> **Extreme Programming** is a highly influential agile method from the late 1990s. It takes an "extreme" approach to iterative development.

How extreme? Consider these practices:

|Practice|Frequency|
|---|---|
|New builds|Several times **per day**|
|Customer deliveries|Every **2 weeks**|
|Test runs|**Every single build**|

> [!warning] Build Acceptance Rule A build is **only accepted** if all tests run successfully. No exceptions.

---

### User Stories for Requirements

In XP, a customer or user is **part of the team** and makes decisions on requirements.

> [!abstract] How User Stories Work
> 
> 1. Requirements are expressed as **user stories** or scenarios
> 2. Stories are written on **cards**
> 3. The development team breaks them into **implementation tasks**
> 4. Tasks become the basis for **schedule and cost estimates**
> 5. Customer chooses stories for the next release based on **priorities** and **estimates**

> [!example] Example: Prescribing Medication Story 
> A user story describes _what_ the user needs to do (e.g., "prescribe medication for a patient"). Task cards then break this down into specific implementation work. Test cases verify the functionality works correctly.

![WIN_20260202_13_07_39_Pro.jpg|400x225](/img/user/1%20-%20MW%20COE420/img/WIN_20260202_13_07_39_Pro.jpg)

---

### Pair Programming

> [!tip] What is Pair Programming? 
> Two programmers work together at the **same computer**, developing code as a team.

**Why does this work?**

| Benefit                    | Explanation                                  |
| -------------------------- | -------------------------------------------- |
| **Common ownership**       | Code belongs to the team, not individuals    |
| **Knowledge spreading**    | Information flows across the whole team      |
| **Informal review**        | Every line of code gets seen by 2+ people    |
| **Encourages refactoring** | Whole team benefits from system improvements |

> [!note] Efficiency 
> Myth Busted 
> Pair programming is **not necessarily inefficient**. Evidence suggests a pair working together can be _more_ efficient than two programmers working separately.

> [!success] Risk Reduction 
> The knowledge sharing in pair programming **reduces project risk** when team members leave. No one person holds all the critical information.

---

## Scrum

> [!abstract] What is Scrum? 
> Scrum is an agile method focused on **managing iterative development** rather than specific technical practices.

### The Three Phases of Scrum

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  Initial Phase  │ ──▶ │  Sprint Cycles  │ ──▶ │ Project Closure │
│  (Planning)     │     │  (Development)  │     │ (Wrap-up)       │
└─────────────────┘     └─────────────────┘     └─────────────────┘
```

1. **Initial Phase** — Establish general objectives and design software architecture
2. **Sprint Cycles** — Series of iterations, each producing a system increment
3. **Project Closure** — Complete documentation, user manuals, and lessons learned

![image-10.png|400x176](/img/user/1%20-%20MW%20COE420/img/image-10.png)
> Main difference is backlog and "sprint" instead of "iteration"

---

### Scrum Terminology

> [!info]+ Development Team 
> A **self-organizing group** of software developers (no more than 7 people). Responsible for developing software and essential project documents.

> [!info]+ Product Backlog ⭐ 
> A **"to do" list** for the Scrum team. May include:
> - Feature definitions
> - Software requirements
> - User stories
> - Supplementary tasks (architecture, documentation)

> [!info]+ Product Owner 
> The person who:
> - Identifies product features/requirements
> - Prioritizes items for development
> - Continuously reviews the backlog
> - Ensures the project meets critical business needs
> 
> _Could be a customer, product manager, or stakeholder representative._

> [!info]+ Sprint 
> A **development iteration**, usually 2–4 weeks long.

> [!info]+ Scrum (Daily Meeting) 
> A **daily meeting** that reviews progress and prioritizes work. Should be:
> - Short
> - Face-to-face
> - Include the whole team

> [!info]+ ScrumMaster
> Ensures the Scrum process is followed. Responsibilities:
> - Guide the team in effective Scrum use
>     
> - Interface with the rest of the company
>     
> - Protect the team from outside interference

> [!info]+ Potentially Shippable Product Increment
> The deliverable from each sprint. Ideally in a **finished state**—no additional testing needed to incorporate it into the final product.
> 
> _In practice, this isn't always achievable._

> [!info]+ Velocity
> An estimate of how much **backlog effort** a team can cover in one sprint. Used to:
> 
> - Estimate sprint capacity
> - Measure improving performance

---

### The Scrum Sprint Cycle

> [!example] How a Sprint Works
> 
> 1. **Starting point:** The product backlog (list of work to do)
> 2. **Selection phase:** Whole team + customer select features/functionality for the sprint
> 3. **Sprint duration:** Fixed length, normally 2–4 weeks
> 4. **Output:** Potentially shippable product increment

---

## When to Use Agile? Key Considerations

### System Issues

> [!question]+ How large is the system? 
> Agile works best with **small, co-located teams** who can communicate informally.
> If large ⇒ waterfall/plan-driven

> [!question]+ What type of system is being developed? 
> Systems requiring **extensive analysis** before implementation need fairly detailed design. (Waterfall)

> [!question]+ What is the expected system lifetime? 
> **Long-lifetime systems** need documentation to communicate developers' intentions to the support team. (Waterfall method if long lifetime since lots of documentation and longspan)

> [!question]+ Is the system subject to external regulation?
> Regulated systems often **require detailed documentation** as part of the system safety case. (Waterfall method)

---

### People and Teams

> [!question]+ How skilled is the development team?
> Some argue agile requires **higher skill levels** than plan-based approaches, where programmers simply translate detailed designs into code.

> [!question]+ How is the team organized? **Distributed teams** may need design documents to coordinate effectively.

> [!question]+ What tools are available? **IDE support** for visualization and program analysis becomes essential when design documentation is minimal.

---

## Summary

> [!success] Key Takeaways
> 
> - Agile emerged to address the need for **rapid, adaptive software development**
> - Core principles: customer involvement, incremental delivery, people over process, embrace change, maintain simplicity
> - **XP** pushes iterative development to the extreme with frequent builds and pair programming
> - **Scrum** provides a framework for managing iterative development through sprints
> - Agile isn't one-size-fits-all—consider system size, type, lifetime, regulation, team skills, and organization

---

_Source: Chapter 3 – Agile Software Development_



In exam, I will give you scenario like this. Midterm 1 has theory (midterm 2, final no theory).
Scenario:
![image-11.png|400x333](/img/user/1%20-%20MW%20COE420/img/image-11.png)
> [!success]- What are the keywords?
> Why is this waterfall
> 500 page documentation
> 21 months from start to finish.
> "sequential phases"
> strict regulatory requirements
> errors cannot be tolerated
> requiring formal approval before proceeding



