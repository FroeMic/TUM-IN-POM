## 05 Usability Management I

###### 31 May - 6 June

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=585723)

---

### 1. Motivation

#### 1.1 Usability Disasters

Many Software Failures are due to Faults in the User Interface. Examples:

* German / Munich MVV ticket machines
* Questionably labeled elevator buttons
* Control rooms in nuclear power plants

#### 1.2 Terminology

##### Usability

* measures how well a user can use the system functionality
* is measured in 5 categories
  * **\[1\] Learnability:** faster to learn =&gt; higher usability
  * **\[2\] Efficiency:** less steps to accomplish =&gt; higher usability
  * **\[3\] Memorability:** how quickly can a user reestablish proficiency
  * **\[4\] Errors:** amount of errors by the user, severity, recoverability
  * **\[5\] Satisfaction:** users come back more often, if the design / experience is pleasant

**"The system is easy to use"** - frequently misused term, often such systems are rather unusable  
**Unusability** - the user has extreme difficulties to learn or use the system  
**User Experience** - A person's perceptions and responses that result from the use and/or anticipated use of a product, system or service. \(= all effectsof a product /service on the user, **before, during** and **after** the interaction\)

##### \(Good\) User Interfaces are hard to design

###### Developer is not equal to the user

* Developers mostly communicate with other developers
* UI development is about communicating with users

###### The User is always right

* consistent problems are the system's fault

###### ... but the User is not always right

* users are not designers

###### UI development takes effort

* 50% of design, implementation and maintenance

###### Managers must be involved \(usability management\)

##### Usability Management

Usability is multidimensional

1. Learnability: Is the UI easy to learn?
2. Efficiency: Once learned, is it fast to use?
3. Memorability: Is it easy to remember what the user has learned?
4. Error Handling / Robustness: Are errors recoverable?
5. Satisfaction: Is the UI enjoyable to use?

### 2. Usability Heuristics \(Nielsen\)

#### 2.1 Methods to reach good usability

##### Heuristics Evaluation

* a usability engineering method to find usability problems in user interface design

##### Usability Testing

* watching a user interact with the user interface of the system
* uses scenario-based testing
* involves creation of a test scenario
* the user performs a list of tasks, while the observer watches and takes notes and compares the observed with the specified behavior 

**Difference:** Usability Testing vs Heuristics Evaluation is similar to Walkthrough vs Inspection

#### 2.2 Nielsen's 10 heuristics

###### Meet the Expectations

1\) Match the real world  
2\) Consistency and standards  
3\) Help and documentation

###### The user is the boss

4\) User control and freedom  
5\) Visibility of system status  
6\) Flexibility and efficiency

###### Handle Errors

7\) Error prevention  
8\) Recognition, not recall  
9\) Error reporting, diagnosis and recovery

###### Keep it simple

10\) Aesthetic and minimalist design

##### 1. Match the real world

* Speak the user's language
* Don't limit user defined names
* Allow aliases in command language
* Use metaphores
* Natural Mapping

##### 2. Consistency and standards

* Principle of least surprise
  * similar things should look and act similar
  * different things should look different
* Other properties
  * consistent size, location, color, wording, ...
* Command / Argument Order
  * Noun-Verb-Order vs Verb-Noun-Order
* Follow platform standards

##### 3. Help and documentation

* Users don't read manuals
* BUT manuals and online help are vital \(if user is frustrated\)
* Help should be:
  * searchable
  * context sensitive
  * task oriented
  * concrete
  * short

##### 4. User control and freedom

* Clearly mark exits
* Users should be able to explore interface \(cancel / undo option\)
* Users should not feel trapped by the interface
* All dialogs should have a cancel button

##### 5. Visibility of system status

* Keep user informed about system state
* Response times
  * &lt; 100 ms \(instantaneous\)
  * &lt; 1s \(user notices, but no feedback needed\)
  * &lt; 5s \(display busy cursor\)
  * &gt; 5s \(display progress bar\)

##### 6. Flexibility and efficiency

* Provide shortcuts for frequent operations
  * keyboard accelorators
  * command abbreviations
  * styles
  * bookmarks
  * history
  * ...

##### 7. Error prevention

* Selection is less error prone than typing
* Disable illegal commands

##### 8. Recognition, not recall

* Use menus, not command languages
* Use combo boxes, not text boxes
* Use generic \(polymorphic\) commands where possible \(Open, Save, Copy, Paste\)
* All needed information should be visible

##### 9. Error reporting, diagnosis and recovery

* Be precise \(restate user's input\)
* Give constructive help
* Be polite and do not blame
* No 'fatal errors' or 'illegal commands'
* Hide technical details \(stack trace\) until requested

##### 10. Aesthetic and minimalist design

* Good design is about simplicity
  * less is more \(KISS\)
* Good graphic design
  * few colors / fonts
  * follow color guidelines
  * align controls
* Use concise language

#### 2.3 Heuristics Evaluation

* application of Nielsen's 10 heuristics
* is an **inspection method**
  * different from user testing
* Performed by a usability expert
* Basic steps:
  * 1\) Evaluator inspects the interface thoroughly
  * 2\) Evaluator compare the user interface against Nielsen's 10 heuristics
  * 3\) Evaluator provides a list of usability problems

##### Good Heuristic Evaluation

* Justify every problem with a heuristic
* List every problem
* Go through the interface at least twice
* Don't limit yourself to the 10 heuristics

##### Formal Evaluation Process

1. Training
   1. Meeting for Design Team and Evaluators
   2. Introduce application, target users, domain, scenarios
2. Evaluation
   1. Evaluators works separately
   2. Each of the generates written reports or oral comments
   3. Focus on generating problems, NOT ranking them
   4. 1-2h per evaluation
3. Severity rating
   1. Prioritize all found problems
   2. Take the mean of all evaluators ranking
4. Debriefing
   1. Evaluators and UI designers discuss the results and brainstorm solutions

### 3. Usability Testing

##### Usability Testing Methods

* AB Testing
* Expert Interview
* Task \(Scenario\) based usability testing
* Think aloud protocol
* First use experience
* Eye / Mouse tracking
* User Questionnaires

##### How much testing?

* Testing is like sex: when it is good, it is very, very good; and when it is bad, it is better than nothing. 
* Nielsen showed that 
  * already **5 users** revealed **85%** of usability problems
  * **15 users** reveal almost all problems

### 4. Prototyping

_Prototyping is **externalizing** and** making concrete a design** idea for the purpose of evaluation._

##### Why Prototyping?

* Instant gratification
* Tangibility \(helps to understand a system early on\)
* Improves poort communication
* Allows early decision making
* Mistakes can be found early 

###### Failures are helpful

* Success in Engineering is defined by its failures \(paradoxical approach to design\)
  * better information comes from failing designs
  * failures draw more scrutiny and result in better solutions

###### Knowledge must be falsifiable

* There is no absolute truth; One can only build theories that are 'true' until someone falsifies it
* Falsification = the act of disproving a theory or hypothesis
* In software engineering any system \(e.g. UI\) is a model, thus a theory
  * models are often built to find counter examples
  * Testing = act of disproving a model
* Prototypes can be used to test 

#### 4.1 Types of Prototyping

![](/assets/protoyping_types.png)

##### Horizontal vs Vertical Prototypes

| **Horizontal Prototype** | **Vertical Protoype** |
| :--- | :--- |
| Show wide range of features | Show small range of features \(scenario / user story\) |
| Horizontal Integration \(bottom-up or top-down\) | Full implementation of those features |
| Used in linear processes \(no full implementation till the end\) | Vertical Integration |
|  | Used in agile processes |

##### Integration Approaches during Prototyping

**\[1\] Horizontal** \(traditional\)  
**\[2\] Vertical** \(agile\)  
**\[3\] UI-Centric** \(?? from both sides\)

####  4.2 Evaluating Prototypes

* Heuristics Evaluation can already be used for the evaluation of prototypes
* Heuristics evaluation works on
  * sketches
  * paper prototypes
  * unstable prototypes
* "Missing element" problems are hard to find on sketches \(=&gt; look harder for them\)

##### Tips for creating paper prototypes

* create as many as possible
* invest as little time as possible in the first iterations
* use test persons, which are in the target group of that software
* Don't limit yourself by thinking 'Is this even possible'
* Involve as many people as possible

### 5. Usability and Serious Games

### 6. Summary

##### General

* Usability is important
* Heuristics \(e.g. Nielsen's 10 heuristics\) help to evaluate / test the usability of a system

##### Benefits of Prototyping

* allow to get early feedback -&gt; saves time while developing
* easier to understand the texts or diagrams -&gt; easier communication
* improve usability

##### Benefits of Serious Games

* increase motivation
* focus on fun

##### Usability

* measures how well a user can use the system functionality 
* is measure in 5 categories
  * Learnability
  * Efficiency
  * Memorability
  * Errors
  * Satisfaction
* Meet expectations, The User is the Boss, Handle Errors, KISS

##### How to reach good usability

* **Follow Usability Heuristics:** e.g. Nielsen's 10 Usability Heuristics
* **Usability Testing:** Test your ideas
* **Prototyping:** Identify problems early
* **Serious Games:** Focus on fun and motivation
* **Human Capabilities:** Model of the User \(Newell\)



