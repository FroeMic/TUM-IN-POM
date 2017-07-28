## 09 Kanban

###### 14 June - 20 June

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=592440)

---

### 1. Motivation

#### 1.1 Challenges of Day-to-Day IT Project Work

##### Software Project Mananger

* Have a hard time setting clear priorities and making corresponding decisions
* They do not understand how their team works an why it 'does not work' the way they want it to.
* They are frustrated because the team does not manage to 'work according to plan'

##### Project Team

* Members are overwhelmed and stressed.
* The development takes longer than planned because the team members continuously have to justify their actions to management and are interrupted.
* The quality of the finished software is insufficient.
* They do not understand why the management makes such significant changes to the direction of the work and wants something different every day.

### 2. Origin: Toyota Production System

###### Motivation: Toyota

* Storage Capacity extremely expensive
* Production 'from stock' not financially feasible
* How can we optimize vehicle production so that we need as little storage capacity as possible?

##### Lean Production

* organize the flow of material similar to a supermarket
* consumer can pick and item, only then it is restocked
* lead to development of Toyota Production System

#### 2.1 Toyota Production System \(TPS\)

##### Production only On-Demand

* Only produce what will be consumed
* 'Pull' mechanism forms the basis of Kanban
* Event-based \(not clocked\) system
* Challenge: Keep the pipeline filled.

##### Product Management using Cards

* Cards \(Jap. Kanban\)signal tasks to do
  * Handed over from station to station when a task is finished
  * Number of tasks **limited** for each station
* **Pull:** Only when a worker has nothing more to do, he will 'pull' the next task from the pipeline
* Challenge: Keep the pipeline going \(everyone is busy\)

##### Special Challenges

* **Lead Time:** Time between receiving a receipt and delivery of the product. \(should be as short as possible\)
* **Just in Time:** The production process should be designed as efficient and effective as possible in order to save costs. \(storage costs, pipeline stall costs\)
* **Optimization:** Minimize production effort while maximizing product quality.

#### 2.1 Optimization of the TPS using Kaizen

* Kaizen is evolution, not revolution!
* Perfection is achieved not when there is nothing more to add, but when there Is nothing
  left to take away.

##### 3 Steps

1. Recognize Potential \(= eliminate redundancy\)
2. Change the Process
3. Measurement and Analysis

##### Muda, Mura, Muri

* **Muda:** every activity / process that does not add value to the production \(=&gt; tailoring\)
* **Mura:** waste resulting from inhomogeneity and inconsistency
* **Muri:** waste resulting from misused resources \(machines / workers\)

###### Muda

* Activities / Processes without added value
* Potential improvement in the following areas:
  * **Transport:** The movement of the product between different production plants and production steps
  * **Warehouse Stock:** Items currently WIP, material and finished products within the company
  * **Movement:** Physical movement of people and machines during operation
  * **Wait Time:** When people / machines are ready for operation, but have to wait
  * **Overproduction:** Producing more than the customer ordered
  * **Overworking:** Doing more than the customer needs
  * **Defects:** Rejects and Defect Elimination during the production process

###### Mura

* Waste resulting from inhomogeneity and inconsistency
* Goal would be consistent, need-based capacity utilization

###### Muri

* Waste resulting from overload
* Potential improvement in the following areas:
  * Employees perform tasks they have not been trained to do
  * Non-ergonomic work spaces
  * Dirty and messy work spaces
  * Work instructions that are not clear
  * Insufficient tool support and kits
  * Insufficient maintenance and servicing
  * Tools and processes that are not allowed
  * Insufficient communication and insufficient feedback to the manager

### 3. Transfer: Kanban in IT

The **Development Process** in software development projects can be seen as the **Production Process**. Further, the **Requirements** represent the **Material** and the final **Software** the resulting **Product.**

#### 3.1 Overview

##### Transparency: Management and Team share a common perspective

| **Management** | Team |
| :--- | :--- |
| - Leadership instead of micromagement | - Considers the 'big picture', not just niches |
| - Makes the best possible decision | - **Kaizen:** continuous optimization of work methods / capacities in regard to cost, time and quality |
| - Communicates clear tasks prioritization | - Improvement without side effects, such as 'passive aggressiveness' |
| - Accepts the team's current work capacity and bases expectations on it | - Ability to make clear statements on capacity and performance |

##### Core Principles of Kanban

1. Start with an existing process
2. Agree to pursue incremental, evolutionary change
3. Respect the current process, roles, responsibilities and titles
4. Leadership at all levels

#### 3.2 Core Practices

1. Visualize the current workflow
2. Limit the work in progress \(WIP\)
3. Measure and optimize the flow
4. Make process policies explicit
5. Implement feedback mechanisms
6. Improve Collaboratively, Evolve Experimentally \(Kaizen\)

##### 1. Visualize the current workflow

* A Kanban board should reflect what the team actually does
  * Backlog
  * Do
  * Develop \(Ongoing / Done\)
  * Deploy
  * Live

##### 2. Limit the work in progress \(WIP\)

* Each column has a WIP limit
* The WIP Limit defines the allowed parallel work in progress in a specific process step
  * Development is ONE process step
  * It does not matter, whether a card is _done_, or _ongoing_, as long as it is in the process step, it counts towards the WIP limit.
* Only if the WIP limit is not yet reached new cards can be pulled in

###### Project Management is Process Controlling and Optimization

* **Flow Theory**
  * Cycle Time: Time needed for entire production process 
* **Little's Law**
  * Throughput = WIP / Cycle Time
  * To increase the Throughput
    * **Reduce **WIP while **improving cycle time**
    * Traditional management would do it the other way around, which creates a downward spiral
* **Lean:** Problems MUST be solved
  * Implicit escalation enforces communication
  * **Slack Time** \(= being blocked?\) is wanted and used to solve problems, so they do not reoccur

##### 3. Measure and optimize the flow

* **Lead Time:** Time from Request being made to Delivery
* **Cycle Time:** Time from Work Begins to Delivery

=&gt; Kanban leads to predictability

##### 4. Make process policies explicit

* **DOD**: Definition of Done
  * defines criteria, when a work item is ready for the next process step
  * agreed among team, customer and stakeholders
* DOD enables **Pull-Principle**

##### 5. Implement feedback mechanisms

* Kanban Cadences \(regular meetings for example\)
  * \[1\] Standup Meeting
  * \[2\] Retrospective Meeting
  * \[3\] Replenishment Meeting
  * \[4\] Operations Reviews

##### 6. Improve Collaboratively, Evolve Experimentally \(Kaizen\)

* e.g. Process Tailoring: Change the process steps under 'Development' to adhere to test-driven development

#### 3.3 Kanban vs Scrum

##### Scrum is REVOLUTIONARY

##### Kanban is EVOLUTIONARY

* Small optimizations minimize the J-Curve effect

![](/assets/scrum_vs_kanban.png)

### 4. Summary

#### 4.1 Properties of Kanaban

##### Kanban \(method\) stands for

* Transparency
* Optimization
* Personal responsibility

##### Kanban does not solve problems, but it makes them visible

##### Kanban begins with the current state and process of a system

* Current system development
* job titles and process is respected

##### Kanban is evolution NOT revolution

* Kaizen
* Kanban always considers the overall picture

##### Kanban requires to rethink traditional management

* Multitasking: =&gt; Stop Starting and Start Finishing
* Push without limits: =&gt; Pull with limits
* 100% capacity utilization: =&gt; 'Slack Time' is wanted

##### Kanban focuses on people, not mechanics

* Kanban is team sport

##### Kanban does not favor a specific management approach

##### Kanban can be combined with different approaches

* **Traditional:** Waterfall Model, V-Model XT, Spiral Model, Unified Process, ...
* **Agile:** Scrum =&gt; Scrum-ban

##### Kanban enables

* Incremental Process Tailoring \(at runtime throughout the process\)
* Process Change / Improvement Management

#### 4.2 Principles and Core Practices of Kanban

##### 4 Basic Principles

1. Start with an existing process 
2. Agree to pursue incremental, evolutionary change
3. Respect the current process, roles, responsibilities and titles
4. Leadership at all levels

##### 6 Core Practices

1. Visualize the current workflow
2. Limit the work in progress \(WIP\)
3. Measure and optimize the flow
4. Make process policies explicit
5. Implement feedback mechanisms
6. Improve Collaboratively, Evolve Experimentally \(Kaizen\)



