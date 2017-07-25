## 04 Software Lifecycle Models II

###### 17 May - 23 May

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=582868)

---

### 1. Sequential Software Lifecycle Models

##### Properties of sequential models

###### Managers love sequential models

* nice milestones
* no need to look back \(linear model\)
* always one activity at one time
* easy to check progress during development \(e.g. 90% coded, 20% tested\)

###### However, Software Development is non-linear

* **During Design:** problems with requirements are identified
* **During Implementation:** design and requirement problems are found
* **During Testing:** coding errors, design errors and requirement errors are found

##### Validation vs Verification

| **Validation** | Verification |
| :--- | :--- |
| - Assurance that a product, service or system meets the need of the customer and other identified stakeholders | - Evaluation whether or not a product, service or system complies with a regulation, requirement or imposed condition |
| - Often involves acceptance and suitability with **external** customers | - Often an **internal** process |
| **Informally:** _Are you building the right thing?_ | **Informally:** _Are you building it right?_ |

#### 1.1 Waterfall Model

![](/assets/waterfall_model.png)

* An activity centered lifecycle model tat prescribes a sequential execution of activities
  * Assumption: Software Development can be scheduled as a linear, step-by-step process, transforming user needs to code
  * Goal: Never turn back, once an activity was completed
* Key Feature: **Verification Step** at the end of each activity
  * ensure that the activity does not introduce unwanted requirements or deletes mandatory ones
* Provides a simplistic view on Software development that measures progress by the number of tasks completed

#### 1.2 V-Model

![](/assets/v_model.png)

* The horizontal object flow denotes the information flow between activities on the same **abstraction level**
* **Higher Levels** of abstraction deal with the requirements in terms of elicitation and operation. 
  * The Client Acceptance Activity validates the understanding of the user against the requirements
* The **middle part** of focuses on mapping the understanding of the problem into a software architecture
  * Component Integration and Test verifies functional components against the preliminary design
* **Lower Levels** focus on details such as the assembly and coding of software components
  * Unit Test Activity verifies units against their description in the detailed design

### 2. Iterative Software Lifecycle Models

##### Iterative vs Incremental

| **Iterative** | Incremental |
| :--- | :--- |
| - means to 're-do' or 're-work' | - means to 'add onto something' |
| - helps to improve product | - helps to improve process |
| **Iterative Development:** A strategy in which time is set aside to revise and improve parts of the system. | **Incremental Development:** A strategy where various parts of the system are developed at different times or rates and integrated as they are completed. |

###### Increments can cause iterations

* a **product iteration** can result from **incremental addition** of functionality that had not been anticipated in previous iterations
* a **product iteration** can also result from **restructuring**

##### Limitations of Linear and Iterative Models

* Linear and iterative models do not deal well with frequent change
  * the Waterfall model assumes that once done with an activity, all issues are covered and will stay so
  * the Spiral model can deal with changes between activities, but not within and activity
* For more frequent changes use
  * Unified Process
  * V-Model XT
  * Agile Methods

##### Prototypes

Important: Don't use the term **rapid prototyping**

* confuses prototyping with rapid development
  * prototyping = technical issue
  * rapid development = management issue
* prototyping can go forever, if not restricted \(time-boxed prototyping\)

###### Types

1. **Illustrative Prototype**
   1. develop the UI with a storyboard
   2. can be as simple as on a napkin or with dedicated tools
   3. Good for first dialog with the client
2. **Functional Prototype**
   1. implement and deliver an operational system with minimal functionality
   2. then add more functionality
   3. good for incremental development
3. **Exploratory Prototype** \("Hack"\)
   1. implement parts of the system to learn more about the requirements
   2. good for paradigm breaks

###### Vertical vs. Horizontal Prototype

* **Vertical Prototype:** Prototypes one feature \(over several layers\)
* **Horizontal Prototype:** Prototypes one layer \(e.g. presentation layer\)

#### 2.1 Spiral Model

* Proposed by Boehm in 1987
* Consists of** 9 iterations** \(cycles\)
  * \[1\] Concept of Operations
  * \[2\] Software Requirements
  * \[3\] Software Product Design
  * \[4\] Detailed Design
  * \[5\] Code
  * \[6\] Unit Test
  * \[7\] Integration Test
  * \[8\] Acceptance Test
  * \[9\] Implementation
* In each iteration **4 basic activities** must be applied
  * \[1\] Determine objectives, alternatives and constraints
  * \[2\] Identify and evaluate alternatives
  * \[3\] Identify and resolve risks
    * If resolved: Results are evaluated and the next iteration is planned
    * If not: immediate termination of project 
  * \[4\] Develop a prototype and obtain approval for the next iteration

#### 2.2 Unified Process

* An **iterative** and **incremental** lifecycle model built on the idea of **cycles** in the lifetime of a software
* Each cycle consists of **4 phases**
  * \[1\] Inception
  * \[2\] Elaboration
  * \[3\] Construction
  * \[4\] Transition
* Each phase can be iterated. During an iteration several **workflows** are performed in parallel
  * **Core Workflows:**
    * Business Modeling
    * Requirements
    * Analysis and Design
    * Implementation 
    * Test
    * Deployment
  * **Supporting Workflows:**
    * Configuration & Change Management
    * Project Management
    * Environment

###### Phases of the Unified Process

The **2 phases **of the Unified Process are decomposed into 4 distinct phases

![](/assets/unified_process.png)

* **Engineering Stage:** \(Inception and Elaboration\)
  * less predictable and smaller teams
  * focusing on design and synthesis activities
* **Production Stage:** \(Construction and Transition\)
  * more predictable and larger teams
  * focusing on construction, testing and deployment activities

###### Phase vs. Iteration

* A **phase** creates a formal stake-holder approved version of artifacts
  * leads to "a major milestone"
  * phase-to-phase transitions are triggered by significant business decisions \(not the completion of software development activities\)
* An **iteration** creates an informal, internally controlled version of artifacts
  * leads to "a minor milestone"
  * iteration-to-iteration transitions are triggered by specific software development activities

#### 2.3 V-Model XT

* successor of V-Model 
* XT = extreme tailoring
* standard for German Government contracts
* incorporates duties of client
* Goals:
  * Minimize project risk
  * Improve and guarantee quality
  * Reduce costs
  * Improve communication
* Focus on products instead of activities \(no defined chronology of activities\)

##### General

* V-Model XT describes **WHO** has to do **WHAT** **WHEN** in a project
* Discriminates between different **Project Types** by
  * Role \(customer, contractor\_
  * Project topic \(HW, SW, complex, embedded, integration\)
* Each type has a **project execution strategy**
  * each stragey is a process model with milestones and decision points
  * V-Model XT = collection of different process models
* Task areas are described by **process components**
  * which define products, activities, roles and their relationships
  * some are mandatory \(V-Model kernel\), other subject to **tailoring**

##### Tailoring

* Select the applicable process components and a project execution strategy to create a project specific process.
* **Static Tailoring** occurs at project definition time \(before the project starts\)
  * project type and characteristics together suggest a set of process components
  * some choices are open \(e.g. optional process components\)
  * project specific adaptations may include
    * using different strategies for prototypes vs final development, etc
* **Dynamic Tailoring** may occur during the project execution
  * e.g. when HW functionality is to be realized, the component 'HW Development' will be dynamically included

##### Execution of a V-Model XT Project

1. Determine the project type and project characteristics
2. Choose a corresponding project execution strategy
3. Tailor the V-Model XT to your project
4. Repeat \(Iterate\)
   1. Identify all decision points to be reached in the next step
   2. For each decision point:
      1. Identify all products to be generated for that decision point \(direct or dependency\)
      2. Identify all activities needed for producing these products
      3. Perform the activities and generate the products.
   3. Evaluate the decision points until the project is finished

### 3. Agile Software Lifecycle Models

#### 3.1 Extreme Programming \(XP\)

#### 3.2 Kanban \(covered in separate class\)

#### 3.3 Scrum \(covered in separate class\)

### 4. Summary

##### Limits of Empirical Process Control Models

= situations where agile methods might not be appropriate

* when not supported by the company culture
* a project too big for regular complete integration
* environments where is inherently takes a long time to get feedback
* where you cannot realistically test

##### Agile Manifesto: Dealing with Uncertainty, Complexity and Change

![](/assets/agile_manifesto.png)

