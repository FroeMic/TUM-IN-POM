## 16 Release Management

###### 12 July - 18 July

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=605263)

---

### 1. Overview: Continuous Delivery and Release Management

#### 1.1 Motivation

**How it should NOT be done:** Delivery only after the implementation was finished
-> rare releases during development
-> little feedback from clients / users during development
-> "Throw a release over the fence" (dev environment != target environment)

##### Release Management

* All activities concerning the creation (build) and the delivery or deployment (release) of software
  * compile source code and link with all dependencies to executable
  * package everything into an executable application
* **Goal:** Automate as many steps as possible
* Release management defines workflows, activities, best practices, how and when to create releases
* Today: mostly continuous integration and continuous delivery

#### 1.2 Terminology

* **Continuous integration**: technique where members of a team integrate their work frequently. Usually each person integrates at least daily, leading to multiple integrations per day.
* **Continuous delivery**: approach in which teams keep producing valuable software in short cycles and ensure that the software can be reliably released at any time.
* **Continuous deployment**: every change that passes automated tests is deployed automatically.
* **Continuous software engineering**: organizational capability to develop, release and learn from software in short cycles.

##### Continuous Delivery vs Continuous Deployment

![](/assets/continuous_deployment.png)

##### Continuous Delivery: Benefits and Challenges

###### Benefits

* Accelerated time to market
* Building the right product: improved product quality and customer satisfaction
* Improved productivity and efficiency
* Reduced risk of a release failure

###### Challenges

* Organizational: Varying interests in different departments
* Process: Traditional processes hinder continuous delivery
* Technical: Maintainability of the source code & tailorable delivery workflows for heterogeneous project environments

#### 1.3 Release Management

The creation and delivery of releases to customers and users.

![](/assets/release_management.png)

##### Release Manager

* Release Management is the process of managing software releases from development \(changes to source code\) to the user
* Responsibilities:
  * **Facilitator:** liaison between different business units to promote smooth and timely delivery of software products and updates
  * **Coordinator:** coordinate disparate source trees, projects, teams and components
* Development and Operations department need to work together =&gt; DevOps

##### DevOps

* Development + Operations
* Emphasizes on communication, collaboration, integration and automation
* The Release Manager acts as a liaison between the involved departments within the software development team

![](/assets/build_management_model.png)

#### 1.4 Build Management

##### Build Management (continuous integration server)

* Regularly checks for changes published to the version control server (pull) or is notified when changes are available (push
* Builds the software
  * Compiles the source code
  * Executes the test cases (regression testing)
  * Packages the software
  * Code signs the software
* Notifies developers about build status
* Automatically detects multiple branches and creates a build plan for each branch (Bamboo)

##### Release Management (continuous delivery server)

* Distributes software to customers and users (a.k.a. Enterprise AppStore)
* Obtains user feedback about the usage of the software
* Collects crash reports
* Stores feedback and crash reports in issue tracker (Jira)

##### Feedback Management in Agile Projects

![](/assets/feedback.png)

##### Release Notes

* Describe the most important changes to the product since the last release
* **Important:** Write them from the viewpoint of the user
  * no technical terms the user does not understand
  * no complex details about the system
  * high level content (short and readable)
* Delivered and Distributed when an update is released
* Shared with end users, customers and clients


### 2. Management Issues and Best Practices

#### Continuous Delivery

* How often do you deliver your application?
* Which process changes do you have to implement to make customers aware of multiple releases during development
* How do you handle customers who do not react to releases?
* How many releases can a customer handle?
* How do you handle feedback within the sprint?
* What needs to be done to implement continuous delivery from scratch? (CI -> CD, CI -> CD -> Feedback)
* How can you tailor the workflow to specific project needs?

### 3. Continuous Software Engineering

##### Best Practices for Build and Release Management

* The process for releasing/deploying software must be **repeatable** and **reliable**
* If something is difficult or painful, do it more often
* Automate **every step** of the build process
    * Write test cases
* Integrate your changes early and often
* Release early and often to obtain feedback
* Release internally first
    * Test it thoroughly
    * Then promote the release to your users
* **React to crashes and user feedback**
* Improve continuously

##### Why is Continuous Delivery difficult for large systems?

* Large systems tend to have many dependencies, legacy code, ...
  * hard to maintain and extend
  * integration testing takes a lot of time
  * each change can lead to many errors (due to dependencies)
* Loose Coupling and High Cohesion are hard to maintain over time
* The middleware layer become a **monolith** => system too big to maintain

###### Conway's Law

_”Any organization that designs a system (defined broadly) will inevitably produce a design whose structure is a copy of the organization's communication structure.”_

###### Typical Structure for Large Systems

* Monolithic Layered Architecture
  * Organization in specialized teams: UI, Middleware, DBAs
  * Many different services in middleware layer
* Better Approach: Microservices
  * Organization: cross functional teams
  * Each microservice only contains 1 service with functionality
* **Benefits:**
  * Strong Module Boundaries (modular structure)
  * Independent Deployment (simple services are easier to deploy)
  * Technology diversity (possibility to mix languages / development frameworks)
* **Costs:**
  * Distribution (harder to program, remote calls have risk for failure)
  * Eventual Consistency (maintaining strong consistency almost impossible)
  * Operational Complexity (mature operations team needed)  

### 4. Summary

* **Build and Release Management** are important topics for today's software engineering projects
* Managers need the ability to use the concepts and tailor them to specific projects environments
* **Continuous Integration**
  * Continuously **build** \(compile, integrate, test\) the source code base
  * Continuously test changes to find regressions
* **Continuous Delivery**
  * Continuously **release** \(i.e. deliver\) applications to users
  * Continuously beta test applications with customers / users
  * Quickly obtain feedback to realize short development feedback cycles



