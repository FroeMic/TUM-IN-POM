## 12 Estimation and Scheduling

###### 28 June - 4 July

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=597843)

---

### 1. Motivation

* Nearly 2/3 of all projects significantly overrun their cost estimates
* 64% of features included in products are rarely or never used

##### Challenges for Estimation

* **Incomplete** knowledge about
  * Project scope and changes
  * Prospective resources and staffing
  * Technical and organizational environment
  * Infrastructure
  * Feasibility of functional requirements
* Comparability of projects in case of new or changing technologies, staff, methodologies
* Learning curve problem

##### Components of an Estimation

* **Costs**
  * Personnel
  * Material
  * Extra costs
* **Scope**
  * Number of requirements
  * Complexity of requirements
* **Time**
  * Development time
  * Project duration
  * Dependencies
* **Infrastructure** \(often forgotten\)
  * Rooms, technical infrastructure, ...

##### Estimation Personnel Cost

* **Personnel Type:** team leader, applicant domain expert, analyst, designer, programmer, tester, ...
* **Cost Rate:** cost per person per day
  * \[1\] Single cost rate for all types \(no differentiation necessary\)
  * \[2\] Assign different cost rates to different personnel types based on experience, qualification, skills
* **Personnel Costs = Person Days \* Cost Rate**

##### Estimating Development Time

* Development time is often estimated by the formula: **Duration = Effort / People**
  * **Problem:** Larger teams increase the communication complexity and decrease productivity
* Product Duration cannot be reduced arbitrarily by adding more people \(Brooks Law\)

### 2. Estimation Modeling

##### Basic Estimation Model

* **Input:** Parametric Data
  * Size & Project  Data
  * Software Process
  * Insight / Experience
  * Historic Data
  * Meta Model of Software Process
* **Output:** Estimate
  * Effort
  * Schedule
  * Cost

##### Top Down and Bottom Up Estimation

2 common approaches for estimations:

###### 1. Top-Down Approach

* Estimate the whole project
* Breakdown to different project phases and work products
* **Problem:** You did not break down the work before.

###### 2. Bottom-Up Approach

* Start with effort estimates for tasks at the lowest possible level.
* Aggregate the estimates until top activities are reached
* Preferred if you have activities and tasks and knowledgable developers

### 3. Traditional Estimation Techniques

##### Methods for estimating cost and effort

All methods require **knowledge about the subject.**

* **Expert Estimations:** \(Based on experience and domain knowledge\)
  * T-Shirt Sizes
  * Planning Poker
  * Delphi
  * Assessment meeting
* **Algorithmic Estimations:** \(Based on KPIs, formulas, metrics\)
  * LOC \(Lines Of Code\)
  * COCOMO II
  * Aron
  * Function Points

##### Expert Estimation

= guess from experienced people \(gut feeling\)

* no better than the participants
* suitable for atypical projects
* justification of the result
* important when no detailed estimation can be done
* works best if the estimates are for short term items

##### Algorithmic Estimation

###### Lines of Code

* Traditional way for estimating application size
* Advantage: easy to do
* Disadvantages:
  * Focus on developers poit of view
  * No standard definition of "Lines of Code"
  * You get what you measure \(reuse and refactoring is ignored\)
* **The use of LOC metrics for productivity should be regarded a malpractice.**

###### COCOMO

* Constructive Cost Model
* Top-down approach to estimate cost, effort and schedule software projects based on size and complexity
* **Assumptions**
  * Derivability of effort by comparing finished project \(database\)
  * System requirements do not change during development
  * Exclusion of some efforts \(administration, training, rollout, integration\)
* **Cocomo II**
  * Also applicable for iterative lifecycle models \(e.g. Spiral Model\)
  * Additionally addresses experience, developer skills and distributed development
* **Problems**
  * Judgement required to determine the influencing factors and their values
  * Experience showed deviation form actual effort by up to a factor of 4 \(Cone of Uncertainty\)
  * Some important factors are NOT considered:
    * skills of team members, travel, environment, UI quality, overhead cost

##### Problems with Traditional Estimation Techniques

###### Cone of Uncertainty

* lessons learned from NASA projects
* at the beginning \(initial concept, before requirements elicitation\) of a project estimates have an uncertainty factor of 4

###### Focus on completion of activities and not delivery of features

* customers get no value from completed activities

###### Wrong focus in schedule reviews

* The reviewers look for overlooked activities not for overlooked features

###### When faced with overrun schedules, teams

* attempt to save time by reducing quality
* introduce change-control policies that constrain highly valuable changes in the software system

### 4. Agile Estimation Techniques

##### T-Shirt Sizes

* Estimations are particularly challenging for inexperienced developers
* Start with a simple model: e.g. T-Shirt sizes
* Map T-Shirt sizes to story points
  * S -&gt; 1
  * M -&gt; 3
  * L -&gt; 8
  * XL -&gt; Too big, split into smaller issues
* Once developers are familiar, move on to more fine grained methods \(e..g Poker Planning\)

##### Planning Poker

* Packages expert estimations into an enjoyable approach
* All participants are estimators, not just the M
* The estimation team should be &lt; 10 people
* Estimates are arrived by **consensus building** \(Do not average!\)

###### Procedure

1. Read the acceptance criteria and discussion points on the Confluence page
2. Discuss how you would implement the user story
3. Individually estimate the user story
4. Simultaneously reveal the cards
5. Compare the points on the cards with each other, and discuss the differences
6. If necessary, play a second and third round Planning Poker
7. Agree on a final decision

###### Challenges

* based on expert opinion
* other teams may come up with completely different estmation
* estimations change with skill / experience
* teams estimates, while individual members are owners
* many people estimating might lead to long discussion
* lazy developers may overestimate tasks
* people tend to average out the point, which does not facilitate a discussion

###### Advantages

* Group Estimation = Wisdom of the Crowd
* The conversation / discussion following an estimate is a great way to pool important issues
* Story points can be used to determine the Sprint Velocity

###### Tips for Planning Poker

* **Keep discussions productive:** Set a limited amount of time for each user story
  discussion. This helps teams learn to estimate more rapidly within agile planning
* **Break out into smaller sessions:** Playing Planning Poker with a sub-set of the team
  is a good option if the number of user stories is too big
* **Choose the right time to play:** Consider playing it several times; once at the kick off,
  and once before each Sprint
* **Write down the reason for the awarded points:** If a user story receives too many
  points, make sure to note what were the Acceptance Criteria that led to that estimation
* **Consider the level of uncertainty:** Does the implementation of this user story
  depend on too many unknown factors? If yes, maybe award more points
* **Distribution of workload according to skill:** Developers who estimate few points
  are good candidates to implement the user story

### 5. Dependency Diagrams

##### Overview

* Dependency Diagrams consist of 3 elements
  * **Event:** A significant occurrence in the life of a project
  * **Activity:** Amount of work required to move from on event to the next
  * **Span Time:** The actual calendar time required to complete an activity
    * Relevant Parameters: Availability of resources, Parallelizability of Activity
* Dependency Diagrams are drawn connected graphs of nodes and arrows.
* Common notations are
  * 1\) Activity on the arrow notation
  * 2\) Activity in the node notation

![](/assets/dependecy_diagrams.png)

##### What do we do with these diagrams?

1. Compute project duration
2. Determine activities that are critical to ensure timely delivery 
3. Analyse the diagrame
   1. Find ways to **shorten project duration**
   2. Find ways to do **activities in parallel**
4. 2 techniques used
   1. **Forward pass analysis** \(determine critical path\)
   2. **Backward pass analysis** \(determine slack time\)

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

* Activities are independent when the duration of one activity does not influence the duration of another activity
* In Software Development most activities are **inter-dependent** 
* When activities are dependent, ** variations in completion time do not balance out**

##### 4. Multitasking causes more delays

2 Tasks: If you are block on Task A, work on Task B

* &gt; 2 Tasks: 
  * **Time spent switching between tasks become costly**
  * Tasks remain in progress longer
  * **Developer Overload:** loading every developer to 100% will congest the system

##### 5. Features are not developed by priority

* Traditional planning assumes that all activities will be completed
  * If all work is completed the order does not matter
  * In reality the project team is often **scrambling to meet the schedule** and drops features
  * Features with high value might be dropped

##### 6. Uncertainty is ignored

* Traditional planning approaches ignore uncertainty
* Better approach: Allow for short iterations
  * reduces uncertainty

##### 7. Estimates become commitments

* Every estimate indicates a probability that the work will be completed in time
* Estimates are no commitment. There is a risk that they will not be met.

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



