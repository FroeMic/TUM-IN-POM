## 15 Agile Architecture

###### 12 July - 18 July

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=603988)

---

### 1. Motivation

* Product development and project management are different
* User Story Mapping is a good technique for providing initial rough estimations of a system
* Software architecture is importany
* Quality attributes should drive the architecture
* Software architecture can be managed continuously
* Duties of the _Software Architect_ role

##### The world is changing fast ...

* Requirements may only be _hypotheses_ and change quickly
* Current market trend is that _products_ change to _services_  \(first mover often win\)
* High uncertainty requires a different mindset than traditional environments \(Lean Startup, Design Thinking\)
* Agile software development and good software architecture enable the necessary flexibility

### 2. Product vs Project

_In reality most IT projects are products. Work accordingly!_

* IT Industry talks about "IT projects"
* However, in practice we work on systems as long as they are needed / valuable
  * most effort is long-term
  * things have to be good, flexible, etc. in the long term
* This requires **Product Management** not project management
  * Products are only successful with good Product Management
  * Focus on **value creation** not time & budget

### 3. Agile Release Planning

##### Personas

* Construct a profile containing information about the type of user relevant to the software being created
*  choose specific characteristics and compiling those into a archetypal description
* based on assumptions
* most of the time you will have 3 - 5 personas

##### User Story Mapping

* Horizontal Axis: Time
* The Backbone
  * at top
  * Main Activities of Personas
* The Walking Skeleton
  * under activities
  * Tasks for each Activity / Persona
  * ordered by neccessity
* Create releases from coherent experiences

![](/assets/user_story_mapping.png)

###### From Estimation Points to Time

* Have a closer look at 2 - 5 user stories
* Break them down as far as possible
* Guess the minimal / maximal person days for each task
* Assume that some uncertainty will be resolved by statistics: [min + 20% , max - 20%]
* **After 2-3 sprint reestimate the backlog based on experience**

##### Team velocity

* To get a better understanding of the team velocity check the velocity after 3-4 sprints, then
  * check your backlog for completeness
  * reestimate the backlog
  
##### Key Messages: Agile Release Planning

* Think in products, not projects
* User Story Mapping is a proven, fast & useful method to create a common understanding of a system
* All stake holders have after such a workshop a common vision for the product development start
* Together with the first few sprints this gives a solid base for planning

### 4. Agile Software Architecture

### 5. Current trends: DDD and Microservices

### 6. Summary

##### Without Good Software Architecture

* Adding features will get more and more expensive
* Developers don‘t want to work on the system
* If you change one part of the system, a completly mentally unrelated other part of the system might get broken
* You can‘t use the system in other environments than the current one
* you have to think about rewriting the whole system \(expensive, big risk\) or get out of business..

##### 6 Principles of Continuous Architecture

1. Architect products, not just solutions for projects
2. Focus on Quality Attributes, not on functional requirements
3. Delay design decisions until they are absolutely necessary
4. Architect for change – „leverage the power of small“
5. Architect for build, test and deploy
6. Model the organization after the design of the system

7. Think in products

8. Agile estimation and planning of products is possible, e.g. with User Story Mapping

9. Software Architecture is important to create and maintain the foundation of products and have options for the future



