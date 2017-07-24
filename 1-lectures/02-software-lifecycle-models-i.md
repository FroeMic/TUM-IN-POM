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



