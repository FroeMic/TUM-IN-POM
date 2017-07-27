## 12 Estimation and Scheduling

###### 28 June - 4 July

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=597843)

---

### 1. Motivation

##### Challenges for Estimation

##### Components of an Estimation

##### Estimation Personnel Cost

##### Estimating Development Time

### 2. Estimation Modeling

##### Basic Estimation Model

##### Top Down and Bottom Up Estimation

### 3. Traditional Estimation Techniques

##### Methods for estimating cost and effort

##### Expert Estimation

##### Algorithmic Estimation

###### Lines of Code

###### COCOMO

##### Problems with Traditional Estimation Techniques

### 4. Agile Estimation Techniques

##### T-Shirt Sizes

##### Planning Poker

###### Challenges

###### Advantages

###### Tips for Planning Poker

### 5. Dependency Diagrams

##### Overview

##### Activity-on-the-Arrow Diagram Notation

##### Activity-in-the-Node Diagram Notation

### 6. Critical Path and Slack Time Calculations

##### Critical Path

##### Non-Critical Path

##### Slack Time

##### Analyzing Dependency Graphs

###### Forward Pass Analysis in PERT Chart

###### Backward Pass Analysis in PERT Chart

###### Slack Time Calculation in PERT Chart

###### Critical Path Analysis in PERT Chart

##### Path Types in Dependency Graphs

##### Types of Dependencies

##### Frequently used formats for schedules

###### Milestone View

###### Activities View

###### Gantt Chart View

###### PERT

### 7. Reasons for Schedule Overruns

##### Overview

1. Activities don't finish early
2. Lateness is passed down in the schedule
3. Activities are not independent
4. Multitasking causes more delays
5. Features are not developed by priority
6. Uncertainty is ignored
7. Estimates become commitments

##### 1. Activities don't finish early

* Tendency that **one expands the scope** of the task to fill the estimated time
* Parkinson's Law: _Work expands so as to fill the time available for its completion._

##### 2. Lateness is passed down in the schedule

* Because traditional plans are activity based, they focus on the dependencies between activities
* Things start early only if EVERYTHING goes right. But the start late if anything goes wrong.
  * An **early** start of an activity does **require a combination of dependencies** to go well.
  * A **late** start of an activity does only **require one dependency** to be late.

##### 3. Activities are not independent

##### 4. Multitasking causes more delays

##### 5. Features are not developed by priority

##### 6. Uncertainty is ignored

##### 7. Estimates become commitments

### 8. Schedule Heuristics

##### 1. How to develop an initial project schedule

* Identify all your **activities**
* Identify intermediate and **final** dates that must be met
* Assign milestones to these dates
* Identify all activities and milestone** outside of your project** that may affect your projects schedule
* Identify "depend on" **relationships** between the activities
* Draw a dependency diagram for the activities and relationships
* Determine critical paths and slack times of non-critical paths

##### 2. How to shorten the project duration

* Re-check the original span time estimates
  * Ask other experts to check the estimates
  * Has the **development environment** changed? \(e.g. desktop vs mobile\)
* Consider different strategies to perform these activities
  * Consider buying a work product \(Buy vs Build\)
  * Consider hiring an external contractor
* Hire more experienced personnel
  * **Brook's Law:** Adding manpower to a late software project makes it later.
  * Trade-Off: Experts work faster, but cost more
* Try to find **parallelizable** activities on the critical path
  * Continue coding while waiting for the results of a review
  * Risk activity, since portions of the work may have to be redone
* Develop an **entirely new strategy** to solve the problem

##### 3. Mistakes when preparing schedules

###### Using Fudge Factors

* **Fudge Factor:**
  * the extra amount of time added to your best estimate to be "just safe"
* Don't use fudge factors!
  * If an activity takes 2 weeks and you add 50% fudge factor, chances are almost 0 that it will be done in less then 3 week \(reason: Parkinson's Law\)

###### The "Backing In" Mistake

* **Backing In:**
  * You start at the last milestone of the project and work your way back toward the starting milestone, while estimation durations will add up to the available time.
* Problems with Backing In:
  * You probably **miss activities** because your **focus is on meeting the time constraints** rather than identifying the required work.
  * Span times are based on what you "allow them to take", not on the time needed
  * The order of the activities may not be the most effective one.
* **Better:**
* Start estimating the required times and then try to shorten the project duration.

##### 4. How to become a good software project manager

###### 1.Don't assume anything

* Find out the facts
* use assumptions only as a last resort
* With every assumption risk is introduced

###### 2. Communicate clearly with your people

* Being vague just increases the chances for misunderstanding

###### 3. Acknowledge performance

* Tell you team members and peers when they are doing well

###### 4. View your people as allies not as adversaries

* Focus on common goals not individual agendas
* Make people comfortable by encouraging brainstorming and creative thinking

###### 5. Be a manager and technical leader

* Deal with people as well as with deliverables, processes, models and systems
* Create a sense of vision and excitement

### 9. Summary

##### Estimation is a basis for the decision to start, plan and manage a project

##### Estimating a project is a difficult project management function, however:

* Few software organisations have established a formal estimation process
* The estimation technique influences the result \(Cone of Uncertainty\)

##### Cost should not be estimated before the work is broken down into activities and tasks

* The dependency graph included the dependencies
* Schedule = Dependency Graph + time estimates

##### Critical Path Analysis

##### Many reasons for scheduling overruns

##### Scheduling Heuristics -&gt; How to become a good manager



