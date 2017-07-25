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

##### Types of Prototypes

#### 2.1 Spiral Model

#### 2.2 V-Model XT

#### 2.3 Unified Process

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

