## 02 Software Lifecycle Models I

###### 10 May - 16 May

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=577450)

---

### 1. Software development as Application Domain

**Methodologies:** provide general principles and strategies for selecting **methods** and **tools** in a given **project environment** when errors occur.

#### 1.1 Introduction

##### Inherent Problems with Software Development

* Requirements are constantly changing / not known in advance
* Frequent changes are difficult to manage \(checkpoints for estimation & planning are difficult to identify\)
* Several Systems of different maturity need to be considered

##### Why do we need Software Lifecycle Models?

* Development of large systems requires _organized approach_
* Software Management can be seen as complex system
* Methods to model systems \(e.g. UML\) can be used to model Software Management

**Software Lifecycle:** \(also Software Process\)  
Set of activities and their relationships to each other to support the development of a software system.

**Software Lifecycle Model:** \(also Software Process Model\)  
An abstraction that represents a software lifecycle for the purpose of understanding, monitoring, or controlling the development of a software system.

#### 1.2 Modeling

* **Advantages**
  * enable developers to deal with complexity
  * make implicit knowledge about the system explicit
  * formalize knowledge and make it 'shareable'
* **Disadvantages**
  * models can themselves become very complex

##### Where do we need Models?

* **\[A\] Communication:** Models provide a common vocabulary. Informal models can be used to communicate an idea.
* **\[B\] Analysis / Design:** Models enable developers to reason about a future system.
* **\[C\] Archival:** Compact representation of the design and rational of a system \(documentation\).

###### \[A\] Models that support Communication

* called _Communication Models_
* purpose: communicate and idea to another **person** \(support communication!\)
* used in early phases of the project, during informal meetings
* does NOT need to be consistent, complete or have correct notation
* e.g. napkin model, whiteboard, mockup

###### \[B\] Models that support Analysis / Design

* called Specification_ Models_
* purpose: provide a representation to reason about the system
* used to communicate an idea to a **tool**
* needs to be consistent and complete
* needs to have correct notation, so it can be entered into CASE tool
* UML is the preferred notation for specification models

#### 1.3 Managerial Challenges of Modeling

###### Formalizing Knowledge is expensive

* takes time and efforts from developers
* **Antipattern:** Analysis Paralysis
* requires validation and consensus

###### Models introduce redundancy

* If the system is changed, the model needs to be changed
* If several models \(different aspects\) exist, several models need to be changed
* If a model is out of sync, it looses it's value

###### Models become complex

* With growing complexity, models use their value. If the model is similarly complex as the system, why use it?

##### Typical Software Lifecycle Questions

* Which **activities** should we select for the software project?
* What are the **dependencies between activities**?
* How should we **schedule the activities**?

###### Software Development Activities \(Examples\)

* **Requirement Anlysis:** What is the problem?
* **System Design:** What is the solution?
* **Detailed Design:** What are the best mechanisms to implement the solution?
* **Program Implementation:** How is the solution constructed?
* **Testing:** Is the problem solved?
* **Delivery:** Can the customer use the solution?
* **Maintenance:** Are enhancements needed? 

### 2. Modeling the software lifecycle

#### 2.1 Tailoring

There is no “one size fits all” software lifecycle model that works for all possible software engineering projects

**Tailoring**: Adjusting a lifecycle model to fit a project

* **Naming**: Adjusting the naming of activities \(e.g. Detailed Design -&gt; Object Design\)
* **Cutting**: Removing activities not need in the project \(e.g. Maintenance not needed\)
* **Ordering**: Defining the order the activities take place in \(e.g. Testing before Implementation\)

#### 2.2 Modeling a Software Lifecycle

* **Functional Model of a Software Lifecycle**
  * Scenarios
  * User Stories
  * Use Cases
* **Structural model of a software lifecycle**
  * Object Identification
  * Class Diagrams
* **Dynamic model of a software lifecycle**
  * Sequence diagrams
  * State chart
  * Activity diagrams

![](/assets/typical_software_development_activities_and_artifacts.png)

#### 2.3 Major Views of Software Lifecycles

**1\) Activity Centered**: Software development consists of a set of development activities.  
**2\) Entity Centered:** Software development consists of a set of deliverables

#### ![](/assets/views_on_software_lifecycles.png)2.4 IEEE Std 1074: Standard for Software Lifecycle Activities

**Process Group: ** consists of a set of processes \(e.g. _Development\)_  
**Process:** consists of activities \(e.g. _System Design_\)  
**Activity:** consists of sub-activities and tasks \(e.g. _Persistent Data Managment_\)

![](/assets/IEEE_1074.png)

### 3. Overview of Software Lifecycle Models

##### Types of software lifecycle models

**Sequential**: Waterfall Model, V-Model \(if changes are not to be expected\)  
**Iterative**: Spiral Model, V-Model XT, Unified Process \(if changes are infrequent\)  
**Agile**: Extreme Programming, Kanban, Scrum \(if changes are frequent\)

###### The Waterfall Model

* Activity oriented
* Only once an activity is finished the next can start. \(sequential\)
* Assumption: software development can be scheduled as a step-by-step process that transforms user needs into code
* Once you are done with an activity, all issues covered in that activity are closed and cannot be reopened
* Activities:
  * Concept Exploration
  * System Allocation
  * Requirements Elicitation
  * Design
  * Implementation
  * Verification & Validation
  * Installation
  * Operation & Support

###### V-Model

* activity oriented
* sequential
* separation between development and testing
* mapping between development and testing activities
* Activities:
  ```
  * Requirements Engineering - - - - - - - - - Acceptance Testing
  * - - - Requirements Analysis - - - - - - -System Testing
  * - - - - - - - - System Design - - - - Integration Testing
  * - - - - - - - - - Object Design - - Unit Testing 
  * - - - - - - - - - - - - - - Implementation
  ```

**Validation:** Assurance that a product, service, or system meets the needs of the customer and other  
identified stakeholders \(often involves acceptance and suitability with **external** customers\)  
**Verification:** Evaluation whether or not a product, service, or system complies with a regulation, requirement, specification, or imposed condition \(often an **internal** process\)

###### Spiral Model

* iterative 
* 6 invariants of the spiral model
  * 1\) Define artifacts concurrently
  * 2\) Perform four basic activities in every cycle
  * 3\) Risk determines level of effort
  * 4\) Risk determines degree of details
  * 5\) Use anchor point milestones
  * 6\) Focus on the system and its lifecycle

###### V-Model XT

* successor of V-Model
* standard for German government contracts
* allows **tailoring** and **iterations**
* incorporates duties of the client
* Goals:
  * Minimization of project risk
  * Improvement and guarantee of quality
  * Reduction of cost
  * Improvement of communication
* Focus on products instead of activities
  * No defined chronology of activities

###### Unified Process

* Transition from engineering stage to production stages
* Each of the following stages defines

  * Objectives
  * Activities
  * Evaluation Criteria

    ```
    [1] - - - - [2]  [1] Inception
     |           |   [2] Inception
     |           |   [3] Transition 
    [3] - - - - [4]  [4] Construction
    ```

###### \Extreme Programming \(XP\)

* initially released in 1987
* initial excitement, followed by lots of problems
* mostly performance problems

###### Kanban

* 4 Basic Principles
  * 1\) Start with the existing process
  * 2\) Agree to pursue incremental, evolutionary change
  * 3\) Respect the current process,roles, responsibilities and titles
  * 4\) Leadership at all levels

###### Scrum

* Management and control process
* Focus on early risk management 
* Deliver working software, incrementally and empirically
* Simple framework for effective team collaboration

### 4. Summary

* A software lifecycle model \(also software process model\) represents a software lifecycle \(concrete instance of a project\)
* A software lifecycle model has the purpose to **understand**, **monitor**, or **control** the development of a software system
* A software lifecycle model consists of **activities and their relationship**
* We use **UML activity diagrams **to model software lifecycles
* Different types of software lifecycle models:
  * **Sequential**: Waterfall Model, V-Model
  * **Iterative**: Spiral Model, V-Model XT, Unified Process
  * **Agile**: Extreme Programming, Kanban, Scrum



