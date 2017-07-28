## 18 Project Management Antipatterns

###### 26 July - 1 August

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=608413)

---

### 1. Pattern vs Antipattern

##### Definition: Pattern

To be considered a pattern, a solution must be applicable to more than one specific problem.

1. **Problem:** eloborates
    1. one **context**
    2. a set of **forces**
2. **Solution:** resolves these forces with
    1. several **benefits**
    2. several **consequences**
    3. solutions can generate **follow-on-problems**
    
**Important:** Patterns can become antipatterns (problematic solutions), when change occurs.

* Change of requirements
* Change of project parameters
* Change of methodology
    
##### Definition: Antipattern

Antipatterns identify and categorize common mistakes in software practice. Informal synonyms are
* Bad Practice
* Bad Idea or Pitfall
* Typical PM mistake
* Typical design error
* Bade use of an acitivity 

Antipatterns consists of **1 problem** and **2 solutions**

1. **Solution**
    1. one **context**
    2. a set of **forces**   
2. **Problematic Solution** describes a commonly occuring solution that causes
    1. multiple **negative consequences**
    2. multiple **negative symptoms**
3. **Refactored Solution** describes how the problematic solution can be reengineered and lead to
    1. multiple **benefits**
    2. multiple **consequences**
    3. potential **follow-on-problems**
    
![](/assets/pattern_vs_antipattern.png)

##### Applicability of Patterns and Antipatterns

* **Patterns** are good for problems, which do not have a solution yet
* **Patterns** emphasize the use of proven good design principles
* **Antipatterns** are good for emphasizing the recognition of mistakes

###### Changing bad solutions into better ones

* When a pattern becomes an antipattern, it is useful to have a proven approach how to change the problematic solution into a better one.
* **Incremental Reengineering** (refactoring)
    * process of incrementally changing the structure of a bad system / project / organisation into a better one with the use of antipatterns

###### Why antipatterns?

* The presence of good patterns alone in a successful system is not enough
* You must also show that those patterns are absent in failing systems
* Likewise it is useful to show the presence of certain patterns in failing systems and their absence in successful systems

### 2. Typical Mistakes in Software Engineering

##### How to kill a project!

* Show the same demo twice to the same audience
* Focus on technologies, not on problems and scenarios
* Don’t maintain consistency between releases
* Isolate team efforts from other teams within an organization
* Rewrite existing clients, servers and applications
* Change the purpose of the system so that the models describe the wrong objects

##### Root Causes for Antipatterns

Most common mistakes in software project management and development include:

* Insufficient communication with the client
* Unfulfilled requirements
* Insufficient testing
* Cost overruns and schedule slips

##### Seven Deadly Sins of Software Development

###### 1. Haste
* Solutions based on hasty decisions (“time is most important”) lead to compromises in software quality

###### 2. Pride (hubris)
*Not invented here (NIH): Not willing to adopt anything from the outside

######  3. Apathy
*Not caring about a problem, followed by unwillingness to attempt a solution

###### 4. Sloth
* Making poor decisions based on “easy” answers

###### 5. Ignorance
* Failure to seek understanding

######  6. Avarice (excessive complexity)
* No use of abstractions, excessive modeling of details

###### 7. Narrow-mindedness
* The refusal to use solutions that are widely known (“Why reuse? I only have to solve one problem”)

### 3. Taxonomy of Antipatterns

**Roles:** Developer, Architect, Manager

##### Development Antipatterns

* Perspective: Software Developer
* Issues: Software refactoring, modification of the source code to improve structure with respect to the long term maintainability

##### Architecture Antipatterns

* Perspective: Software Architect
* Issues: Partitioning of subsystems and components, platform independent definition of interfaces and connectivity of components

##### Management Antipatterns

* Perspective: Software Project Manager
* Issues: Software Project Organisation, software process model, human communication, rationale management and resolution of issues

![](/assets/antipattern_taxonomy.png)

### 4. Examples of Antipatterns

#### 4.1 Analysis paralysis

_Unrealizable models are worth nothing._

##### General Form

* Goal to achieve perfection and completeness of the analysis phase
* Generation of very detailed models
* Detailed analysis can be successfully completed prior to coding
* Assumption, that everything about a problem can be known a priori
* Analysis model will not be extended nor revisited during development

##### Symptoms and Consequences

* Cost of analysis exceeds expectation without a predictable end point
* Analysis documents no longer make sense to the domain experts

##### Typical Causes

* Management assumes a waterfall progression of phases

##### Refactored Solution

* Iterative development
* Incremental development assumes that details of the problem and its solution will be learned in the course of the development process
* Vertical prototyping
* Scenario based design
* Sprint based development

#### 4.2 Functional Decomposition (No OO)

##### General Form

* everything is a function, lots of files called misc, util, util1, aux1, aux2…
* **Unbalanced Forces:** management of complexity, change management is difficult

##### Symptoms and Consequences

* The functionality is spread all over the system
* Maintainer must understand the whole system to make a single change
* Code is complex, hard to understand, high coupling between code sections in different files, impossible to maintain
* User interface is often awkward and non-intuitive

##### Typical Causes

* Programmers have been trained only in an imperative / functional language
* Designers have been trained with a functional decomposition method 

##### Refactored Solution

* Object-oriented analysis
* Object-oriented reengineering (process)

#### 4.3 Corncob

##### General Form

##### Symptoms and Consequences

##### Typical Causes

##### Refactored Solution

#### 4.4 Death by Planning

##### General Form

##### Symptoms and Consequences

##### Typical Causes

##### Refactored Solution

#### 4.5 Mushroom Management

##### General Form

##### Symptoms and Consequences

##### Typical Causes

##### Refactored Solution

### 5. Summary

###### Example Antipatterns

* **Analysis paralysis**
    * Spending excessive time in requirements elicitation and analysis
* **Functional decomposition**
    * Design and implementation style of developers, who got their initial training in structured analysis methods and imperative languages, with no or little experience in OO methods and OO languages
* **Corncob**
    * Difficult people who usually create additional stress
* **Death by planning**
    * Too much planning, lack of an up-to-date project plan
* **Mushroom**
    * Bad understanding of requirements, management isolates developers from the system’s end users