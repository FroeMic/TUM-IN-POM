## 03 Scrum

###### 17 May - 23 May

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=581034)

---

### 1. Defined vs. empirical process control

##### How can we control software development with a process?

###### 1. Through Organizational Maturity

* Repeatable Process
* Capability Maturity Model Integration \(CMMI\)

###### 2. Through Agility

* Software development is empirical by nature
* It cannot be modeled with a defined process

##### Define vs Empirical Process Models

**Defined Process:** Planned, Follows strict rules, Avoids deviations  
**Empirical Process**: Not entirely planned; rather inspect and adapt

###### Defined Process Control Model

* requires that every piece of work is completely understood
* deviations are seen as errors that need to be corrected
* given well defined inputs, the same outputs are generated every time
  * Precondition: All tasks and activities are well defined and provide **predictability** and **repeatability**
  * If the preconditions fail: surprises, loss of control, incomplete / wrong work products

###### Empirical Process Control Model

* not all pieces of work are completely understood; imperfectly defined process
* deviations, errors and failures are seen as opportunities that need to be investigated
* **Expects the unexptected:** control and risk management is exercised through frequent inspection
* Condition when to apply this model:
  * change is frequent and cannot be ignored
  * e.g. change of requirements, change of technology, change in the organization, change of people \(?\)

##### Scrum is based on an Empirical Process Control Model

* Definition \(Rugby\):  A Scrum is a way to **restart the game after an interruption**
* Definition \(Agile Processes\):  Scrum is a technique that **deals with interruptions** \(change\)
  * Manages and controls software and product development with rapidly changing requirements
  * Improves risk management by improved communication and cooperation and the delivery of product increments

### 2. Scrum: An Example of Empirical Process Control

##### Scrum Artifacts

1. **Product Backlog:** List of requirements of the whole product
2. **Spring Backlog:** List of requirements for one iteration \("Sprint"\)
3. **Potentially Shippable Product Increment:** Release to the Product Owner that contains all results for the current sprint

##### Scrum Meetings

1. **Project Kickoff Meeting:** \(at the start of a project\)
   1. Create and prioritize Product Backlog
2. **Spring Planning Meeting:** \(at the start of each spring\)
   1. Create Sprint Backlog
   2. Important: Development Team and Product Owner select items together
3. **Daily Scrum Meeting:** \(everyday, about 15 minutes\)
   1. Standup Meeting to share **status**, **impediments** and **promises**
4. **Sprint Review Meeting:** \(at the end of each sprint\)
   1. Demonstration of realized backlog items to the Product Owner \(and other stakeholders\)
   2. Release and deliver the application \(product increment\)
   3. Important: Product Owner gives feedback
   4. Can be combines with the Sprint Planning Meeting for the next sprint.
5. **Sprint Retrospective:** \(after each sprint\)
   1. Opportunity to inspect the previous sprint and create a plan for improvements to be enacted during the next sprint

##### ![](/assets/scrum.png)

##### Scrum Roles

1. **Development Team:** self-organizing and cross-functional team, which realizes the product increment
2. **Scrum Master:** resolves impediments and is responsible for the process \(e.g. visualization of progress with burndown chart\)
3. **Product Owner:** defines the product and is responsible for the results

##### Sprint

* Time box during which the team creates a potentially shippable product increment.
* Typically 2-4 weeks long.
* Sprints have consistent duration throughout a project.
* A new sprint starts immedidately after the conclusion of a previous one.

### 3. Exercise: Modeling Scrum

// TODO: Model Scrum as activity diagram

```
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

### 4. Requirement Specification

##### Product Backlog

* Collection of items \(user stories, scenarios\) prioritized by the Product Owner
* Can be changed or reprioritized during projects
* Create on the basis of  problem statement before the actual project starts \(e.g. at Project Kickoff Meeting\)

##### Priority

* describes the importance of a requirements for the software to be developed
* if a requirement has high value \(e.g. core functionality\), it has a high priority
  * **Critical:** \(Prio 1\) - candidates for the first development sprints / must be part of the first product increment
  * **Major:** \(Prio 2\)  - must be realized within the project
  * **Minor:** \(Prio 3\) - desirable, if there is enough time
  * **Not Important:** \(Prio 4\) - might not be realized at all
* priorities can change during the project in Scrum
* Important: Prioritization is done by the Product Owner

##### Level of Difficulty

* T-Shirt sizes represent r

### 5. Exercise Apply Scrum



