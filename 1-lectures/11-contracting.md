## 11 Contracting

###### 21 June - 27 June

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=597843)

---

### 1. Motivation

#### 1.1 Why is Contracting important?

##### Questions need to be answered

* What are expected deliverables?
* What is the schedule?
* What about the money?
* What are the responsibilities of the contractor and the client?
* What about change management?

##### Important!

* A contract defines the **basic requirements** of a project \(deliverables, time, money\)
* A contract defines the **basic rules of collaboration**
* However: It does not dictate how to deal with uncertainties \(requirements, innovation, change\)

#### 1.2 Contracting in the Project Lifecycle

##### How does contracting work?

* Part of the project preparation \(pre-development\)
* Procurement, Acquisition and Bidding Procedures

###### Acquisition and Bidding

* Can be very formal
  * e.g. rigorous evaluation and selection processes in the public sector
* Don't underestimate the effort

###### Critical

* Price-Performance Ratio
* Good Estimations
* Good Calculations

##### Contracting: Interaction

###### Decision Gate

* Milestones and Quality Gate
* Requires completed work products to determine project progress
* A project plan is a sequence of decision gates

###### Client Project

* Get a system 
* Often Waterfall like

###### Contractor Project

* Build a system
* Flexible approach

###### =&gt; The formal contracting flow

| **Client** |  | Contractor |
| :--- | :---: | :--- |
| 1. Request for Proposals | =&gt; |  |
|  | &lt;= \(Offer\) | 2. Submit Offer |
| 3. Contract Awarded | &lt;= \(Contract\) =&gt; | 3. Contract Awarded |
| 4. Iteration scheduled |  | 4. Iteration scheduled |
| 5. Acceptance Completed | &lt;= \(Software\) =&gt; | 5. Acceptance completed |
|  | &lt;= \(Final Project Report\) | 6. Project Completed |
| 7. Project Completed |  |  |

##### Contracting: Roles

Procurement, acquisition and bidding require 'project roles' \(Client, Contractor\). A contract defines responsibilities, deliverables, schedules, procedure for BOTH of them

* **Client** \(also Customer, Purchaser, Contracting Enitity\)
  * Define initial requirements
  * Request proposal\(s\)
  * Monitor \(proposal\) projects
  * Acceptance testing
* **Contractor** \(also Supplier\)
  * Submits offers \(bidding\)
  * Ships results \(software, concrete deliverable, services, ...\)

It gets more tricky, if it is an internal project **without** a contract

* Who is the client? Who is the contractor?
* How to define the agreement?
  * Informal Agreement
  * Formal Agreement
  * Cross-Unit-Collaboration

### 2. Influence Factors

Projects have different influence factors. These are also relevant for the contracting procedures.

###### Main Influence Facors

* Goals
* Business Case
* Initial esitimations
* Legal restrictions

###### Context Variables

* Every project has a variety of context variables, which
  * need to be considered in the contract
  * and have to be addressed properly, while leaving some flexibility
* Context variables and formal legal requirements need to be balanced in order to create a suitable environment for the project

##### Contract Content

* **Services and Responsibilities**
  * Functional Requirements
  * Deadlines \(procedures for delays\)
  * Quality Requirements \(non-functional requirements\)
  * Price and Payment Schedule
  * Acceptance
* **Warranty and Liability**
* **Provisions**
* **Copyrights**
* **Regulations, Standards, Compliance**

### 3. Basic Procedures

#### 3.1 Overview

A project usually starts with a dialog and need preparation \(regardless of acquisition strategy\)

##### Project Acquisition Strategies

1. Pro-Active
2. Re-Active
3. Client request for an offer
4. Call for bids/submissions

##### Preparation in Practice

* Plan the offer's development as a project
  * \[1\] Prepare the Offer
  * \[2\] Develop / Submit the Offer
  * ... \(System is developed\)
  * \[3\] Acceptance of the System under Development
* A contract is **always** concluded based on the accepted offer.
* Sum of this makes contracting very demanding.

#### 3.2 Prepare the Offer

**Experience and Observation** are important for the offer preparation. Particular procedure may vary from company to company.

**Input:** Project Idea  
**Output:** Project Proposal \(Draft\)

###### Steps

1. Collect and complete information
   regarding the client
2. Evaluate business value
3. Conduct feasibility study
4. Develop offer and sales strategy
5. Estimate cost and effort
6. Check resource availability
7. Initial project planning
   1. Cost Plan
   2. Resource Plan
   3. Risk Analysis
   4. Scheduling \(initial\)
8. Create proposal

#### 3.3 Develop the Offer

**Input:** Project Proposal \(Draft\)  
**Output:** Project Proposal

###### Steps

1. Build proposal development team
2. Develop proposal development strategy
3. Develop and continuously improve proposal parts
   1. Sales Parts
   2. Economic Parts
   3. Solution Parts
   4. Contract Parts
4. Develop initial project plan
   1. Project Plan
   2. Effort and Cost
   3. Resources

#### 3.3 Prepare Acceptance

The acceptance procedure should define

* **Contractor:** Shipping, including preparation
* **Client:** Acceptance Test, including
  * Who is authorized to accept?
  * Formal or silent acceptance?
  * Partial Delivery
  * Reporting

**Important:** Already in the contract the procedure for the system's acceptance have to be defined. Acceptance means always a **reversal of the burden of proof**.

* delivery dates
* acceptance procedures

##### Acceptance Tasks

* Check for **completeness**: “Was everything shipped as expected?”
  * Basis: the contract
  * Further artifacts: additional agreements, change requests, management decisions
* **Verification** of the project results: “Was the software developed right?”
* **Validation** of the project results: “Was the right software developed?”

##### Problems in the acceptance phase

* Errors and bugs
* Acceptance delays
* Acceptance refusal
* Acceptance with conditions

### 4. Legal Aspects

_"A contract is really just a set of written playing rules"_

##### Content, responsibility, trust, and risk

* How is a contract **structured**?
* What are the **basic rules** for delivering scope and invoicing revenue?
* How is **risk** and **reward** shared between customer and contractor?
* How are **changing requirements** handled?
* What **relationship model** between contractor and client is implemented? 

##### Contract Types

| **Fixed Price** | Time & Material |
| :--- | :--- |
| **Subject:** A system | **Subject:** Resources and time |
| **Price:** fixed | **Price:** based on effort |
| **Progress Definition:** Milestone based, payment schedule | **Progress Definition:** Feature based, not necessarily congruent with payment schedule |
| **Disadvantage:** Low flexibility regarding changes \(changes request, changes are expensive\) | **Advantage:** Open for change requests, as long as the client pays |
| **Project Risk:** Transferred to the contractor | **Project Risk:** Transferred to the client |
| **Prerequisites:** Fully specified system | **Prerequisite:** Requirements can be under-specified |

###### Relationship Model: Fixed Price

**Client**

* negotiation and contracting procedures are well known
* client sticks to waterfall process
* client provides extra description of product \(fully specified system\)
* contract ensures that client gets product as specified \(but not necessarily what they want\)
* low budget reliability
* high cost risk
* **Risk:** max\(system\) for min\(price\)

**Contractor**

* realized project exactly as stated in the requirements specification
* has better perspective on project than customer
* scope and status can be determined based on requirements
* fixed price project are not meant for change
  * changes have impact on archtitecture / functionality
  * many contractors have adopted this as business model \(risk compensation\)
* **Risk:** min\(System\) for max\(Price\)

###### Relationship Model: Time & Material

**Client**

* Goal: maximise value and get a meaningful solutions
* Allocate resources as needed
* Responsible for project success by
  * providing feedback
  * taking part in the project
* The idea: one can exchange the contractor during the project \(prevent vendor dependencies\)
* **Risk:** Contractor might increase effort \(and cost\) unnecessarily
* **Risk:** Contractor has no duty to ship a product

**Contractor**

* Yield supplies as stated in contract \(only requested resources are delivered\)
* Invoice as many person-days as possible \(to make the project more expensive\)
* Make yourself irreplaceable
* **Risk:** Client might refuse the price increase

##### Relationship Model Behavior

* In projects parties have **interests**
* Interests are reflected in the behavior and interaction strategy
  * **competitive** \(my win is your loss\)
  * **cooperative** \(win-win\)
  * **indifferent** \(I don't care - you lose\)
  * **dependent** \(heads: I win - tails: you lose\)
* Contract should be signed with a **win-win** interaction strategy
  * fair contract 
  * allows open atmosphere during project

### 5. Practices

##### Why do we need different process models \(alternatives\)?

* Significant increase of agile methods \(absolute and relative\)
* Relative growth of rich processes \(e.g. V-Model XT\)
* **Consequence:** The classic approaches have to evolve

#### Contracting Practices

##### Overview

Several practices exist to make contract more flexible to adopt agile methods.

1. Maximum Price
2. Change for Free
3. Exit Point / Money for Nothing

**Note:** All these practices have currently no clear legal basis. They are based on agreements that clients and contractors make. There are no legal definitions of how to apply them.

##### Overview
##### 1. Maximum Price

**Idea:** Work according to **Time & Material** but set a limit.

* Define and estimate the system
* Define the max price for the system
* Define the cost per unit (e.g. cost per story point)

##### 2. Change for Free

**Idea:** Client is participating in the project (on-site client), give continuously feedback and has a learning curve

* Allow the client to add features
* Identify other features that can be removed / stalled
* Update the contract accordingly

##### 3. Exit Points / Money for Nothing

**Idea:** Define an approach where a project can be stopped, but good performance is awarded.

* Define exit points (under which conditions to stop the project)
* Define payments to compensate, or award early termination

##### 4. Combined Practices

##### How to handle failure?

_ As soon as lawyers start talking, the project is a failure._

* Contract-relevant **failure** in a project can occur for many reasons
* It is important to be prepared, for this:
    * Define **Warranty**: when do liability and damage compensation start?
    * Define **Ownership**: who owns the project results?
    * Define **Copyright**: who is authorized to publish and use project results?
    * Define **Escalation**: don’t go to court immediately; give mediation a chance

### 6. Summary

Contracts define the **basic rules of collaboration** – they set the stage…

##### They define

* Functionality/deliverables and their respective quality
* Responsibilities
* Time/Schedule
* Money

##### Two basic types \(defined and legally solid\)

* Fixed Prices
* Time & Material

Several** additional practices** exist to adopt flexibility and to reflect actual software development business \(changing requirements, technology, etc...\)

##### What are contracts for? \(And for what not ...\)

* Contracts **define rules** =&gt; It is not the goals to outrun the partner
* Contracts **need balance** =&gt; risk share
* Contracts **need to be fair** =&gt; all participating parties have rights and duties

* It is good to have a contract, but in projects ...

  * talk about the system, not paragraphs
  * an open atmosphere is better than a legal skirmish
  * you should name escalation authorities that are NOT lawyers

* **Remember:** A court case may give you justice, but no working software ...



