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
* choose specific characteristics and compiling those into a archetypal description
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
* Assume that some uncertainty will be resolved by statistics: \[min + 20% , max - 20%\]
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

_Architecture is defined by the recommended practice as the fundamental organization of a system, embodied in its components, their relationships to each other and the environment, and the principles governing its design and evolution._

= those parts, which are they hardest to change

##### How Software Architecture can help

1. turns a big problem into smaller more manageable problems.
2. shows people how to work together effectively.
3. provides a vocabulary for talking about complex ideas.
4. looks beyond features and functionality.
5. connects business goals with the practical realities of implementation.
6. helps us avoid costly mistakes.
7. enables agility.

##### Architecture Drivers

A good architecture balances these (often conflicting) goals:

![](/assets/software_quality_tree.png)

##### Software Architect Role

* In small teams: architecture is often defined & evolved by senior developers
* In bigger product development team, the role is given to dedicated people
  * Architecture Agents
  * Supporting Architect
* Often intensive work together with UX and Business

###### Duties
  * Clarify Requiremens
  * Design Structures
  * Design (crosscutting) concepts
  * Communicate Architecture
  * Shepard Implementation
  * Evaluate Architecture
  
##### Methodically Designing Software Architectures

  * iteratively design & decide
  * ARC42: Architecture documentation

##### 6 Principles of Continuous Architecture

1. Architect products, not just solutions for projects
2. Focus on Quality Attributes, not on functional requirements
3. Delay design decisions until they are absolutely necessary
4. Architect for change – „leverage the power of small“
5. Architect for build, test and deploy
6. Model the organization after the 
design of the system

##### What is good Architecture?

* Suits constraints that enable the long-term evolution of the software
* Solves business problems
* System remains easy to understand, change, extend
* Valuable

##### How to deal with large systems

###### Cognitive Mechanisms

  * allow comprehension of larger system
  * Chunking (Modularity)
    * responsibility, coupling, size, interfaces
  * Hierarchies (Hierarchical Layering)
    * No cycles - neither on architectural nor on class level
  * Schemata (Pattern Consistency)
    * Consistent and integrated pattern
    * Use a pattern language
    
###### Layering

  * **Domain Layering:** Contracting, Offer/Ordering, etc.
  * **Technical Layering:** Presentation, Business Logic, Database
  * In the long run, domain layering is more important than technical layering
  
###### Timing of Software Architecture

  * One Team: Continuously
  * More Teams: Before start of development
    * Planned Design instead of Emergent Design  
  
###### Current Trends

* Clean Code
* Design Patterns

##### Architectural Decision

###### Make good decisions:
– Create options, test them
– Delay decisions as long as possible (until last responsible moment)
– Try to make reversible decisions (if not too expensive)
– Communicate them well!

###### Strategic Decisions

* Decisions spanning several subsystems or components
* Decisions involving compromises or tradeoffs
* Decisions involving intense stakeholder discussions
* Decisions founded in organizational or political constraints 

### 5. Current trends: DDD and Microservices

##### Domain Driven Design

_The critical complexity of most software projects is in understanding the domain itself._

* creates a common vocabulary
* bounded context: decoupling!

###### Architecture driven by DDD

* Clean Architecture
* (really good read, 10/10 can recommend)
* [Article 8thlight](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html)

##### Microservices

* Monoliths put all functionality in on process and scales by replicating the monolith on several servers
* A microservice architecture puts each functionality into a separate service and scales by replicating those as needed
* Microservices are more complex to manage for **small projects**
* As complexity increases, productivity of monolithic architectures falls rapidly
* The decreased coupling of microservices reduces the loss of productivity for complex and large systems




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



