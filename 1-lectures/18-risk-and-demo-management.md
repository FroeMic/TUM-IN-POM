## 18 Risk and Demo Management

###### 19 July - 25 July

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=606694)

---

### 1. Risk Management

_Risks must be taken because the greatest hazard in life is to risk nothing._

##### Risk

* ... is the deviation of a result of a future event from expectations
* ... is uncertain whether it will materialize or 
* ... is a potential harm that may arise of such an event
* ... depends on our decisions

**Murphys's Law:** _“Anything that can go wrong, will go wrong”_

##### Risk Differentiation

![](/assets/risk_differentiation.png) 

##### Risk Assessment

**Important:** Accept the uncertain, but identify risks!

###### Identify Risks

* What might affect the project objectives? (internal / external)
* Performed by project management AND team
* **Methods:** brainstorming, checklists, expert discussions, SWOT analysis
* Categorize risks (complexity, technology, communication, ...)
* Assign risk triggers
* In agile Projects (Scrum)
    * Daily Scrum: status, **impediments**, promises
    * Sprint Review: identify improvements for next sprint

###### Risk Assessment Matrix

* 3 Dimensions: Impact, Probability, Control

![](/assets/risk_assessment_matrix.png)

##### Risk Mitigation

Risk Mitigations can be grouped into 4 possible types.

1. **Avoidance**
    * Try to avoid risk occurrence
    * Mostly used at planning phase
2. **Control**
    * Identify actions to control risk occurrence and impact
    * Most common response
3. **Transfer**
    * Delegate risk (e.g. to subcontractors)
4. **Investigation**
    * Try to analyze risk further
    * Risk is not reduced

###### Risk Mitigation Plan

* Periodic Risk Assessment
* Possible Escalation to upper management

##### Risk Management Skills

1. **Rules**
    * Update risk log
    * Establish contingency plan
2. **Knowledge**
    * Specific IT knowledge
    * Business / functional know how
3. **Distance**
    * Challenge time and cost estimates
    * Listen to different opinions
4. **Intuition**
    * Expert Estimations
    * Feeling about risks and problems

### 2. Demo Management

##### Motivation

* Boring demonstrations do not convince your customer for future investments or users to buy your software
* Decisions are heavily influenced by feelings
* Combination of technical and marketing skill required

##### How to make a great, convincing and entertaining demo?

* Selection of the right demo: focus on the core value to end users
* Influenced by the real world usage of the software
* Described by visionary scenarios in the problem statement

#### 2.1. Tornado Model: From Visionary Scenario  to Demo Scenario

#### 2.2 Mock Object Pattern

##### Can we do a demo with a missing subsystem?

Yes! We use **model based demonstration:**

##### Model-Based Demonstration

1. We start with the **System Model**
2. We identify the **SUD** (System under Demo)
3. Find other objects that interact with the SUD, but are not implemented yet. These are **Collaborators**.
4. To interact with Collaborators, create **Mocks**
5. **Mocks** mimic the behavior of the Collaborators

##### Mock-Object Pattern

Good design is crucial when using mock objects: the real object (subsystem) must be specified with an interface (façade) and a class for the implementation.

* The mock collaborator replaces the behavior of the collaborator (the real object)
* A mock object can be created at startuptime with a factory pattern
* Mock objects can be used for testing state of individual objects as well as the interaction between objects

![](/assets/mock_object_pattern.png)

##### Taxonomy of Doubles

* **Dummy object:** often used to fill parameter lists, passed around but never actually used
* **Fake object:** a working implementation that contains a “shortcut” which makes it not suitable for production code
* **Stub:** Provides canned answers to calls made during the test. Provides always the same answer
* **Mock object:** mimic the behavior of the real object. Know how to deal with a specific sequence of calls they are expected to receive

##### Software Demo Tips

* Be enthusiastic and convincing, but don’t lie
* Have a strong opening
* Include humor (ideally subtle but funny jokes), but don’t make fun of somebody
* Focus on user needs and problems that the software solves
    * Find the right balance between marketing and technical complexity
    * Explain technical decisions and details in a way that even non IT people can understand it
* Prefer application domain terminology instead of solution domain terminology
* Prepare backups (videos, pictures) in case something goes wrong (Murphy’s law)
* If something goes wrong, accept the failure and deal with the situation

#### 2.3 Demo Feedback

![](/assets/demo_feedback.png)

* Developers deliver the demo application to the customer
* They present the demo application and request feedback from the customer
* The feedback is then used to refine the initial visionary scenario (or design)
* Notice: developers should be honest about
what is implemented and what is mocked

![](/assets/demo_feedback.png)
### 3. Summary

* Preparing a great demo of your application convinces the customer
    * Play the role of the user of the application in an authentic way, e.g. dress up like the real user
    * Use humor in your demonstrations (but: don’t overdo it)
* Prepare a screenplay with the scenes of the demo (based on the event-flow of the demo
scenario)
* Use the mock object pattern to mimic the behavior of collaborating objects that are not
implemented yet
* With a great demo, all stakeholders understand the purpose of the application
* Remember Murphy’s Law and prepare for it: _“anything that can go wrong, will go wrong”_
    * Use risk management and have a backup plan if risks materialize as problems
    * Prepare backups for your demo, e.g. videos and images
