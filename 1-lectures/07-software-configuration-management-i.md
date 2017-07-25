## 07 Software Configuration Management I

###### 7 June - 13 June

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=589540)

---

### 1. Motivation

##### Why Configuration Management?

* Multiple people work on artifacts that are changing
* Mote than one version of the artifacts has to be supported
  * Released software systems
  * Custom configured systems \(different functionality\)
  * Systems under development
  * Software running on different machines & operating systems
* =&gt; Need for coordination

###### **Software Configuration Management \(SCM\)**

* Manages evolving software systems
* Controls the costs involved in making changes to the system

##### What is Configuration Management

* Definition of **Software Configuration Management**
  * a set of management disciplines within a software engineering process to develop a baseline
  * baseline = a work product that can be changed inly through a change control procedure
* IEEE 828-2012: Standard of Configuration Management in Systems and Software Engineering

##### Administering Software Configuration Management

* SCM is a **project function** with the goals to make technical and managerial  activities more effective
* SCM can be administered in several ways
  * organization-wide
  * project-specific
  * distributed among all project members
  * mixture of the above

##### Configuration Management Roles

* **Configuration Manager**
  * Responsible for identifying configuration items
  * responsible for defining the procedures \(workflows\) for creating promotions / releases
* **Change Control Board Member**
  * responsible for approving or rejecting change requests
* **Developer**
  * creates promotions triggered by changes requests or the normal development activities
  * checks in changes and resolves conflicts
* **Auditor**
  * responsible for the selection and evaluation of promotions for release
  * responsible for the consistency and completeness of the release

##### Configuration Management Activities

1. **Configuration Item Identification** \(Modeling the system as a set of evolving components\)
2. **Promotion Management** \(Creation of versions for developers\)
3. **Build and Release Management** \(Creation of versions for clients and users\)
4. **Change Management** \(Handling, Approving, Tracking of change requests\)
5. **Branch Management** \(Management of concurrent development\)
6. **Variant Management** \(Management of coexisting version\) **\(Not Covered\)**

### 2. Terminology

##### ![](/assets/scm.png)

##### Configuration Item

* An aggregation of software, hardware \(or both\) designated for configuration management and treated as a single entity in the configuration management process
* Software Configuration Items
  * Source Files
  * Models
  * Tests
  * Binaries
  * Documents
  * Configurations
* Hardware Configuration Items
  * CPUs
  * Bus Speed Frequencies
  * Sensors
  * Actuators

##### Configuration Item Identification

* Not every entity need to be under configuration management control
* 2 Issues:
  * \[1\] **What**: Selection of configuration items
    * What should be under configuration control?
  * \[2\] **When**: When do you start to place entities under configuration control?
    * In early days, it was an activity
    * Today it should be a **project function** \(from the beginning to the end of the project\)

##### SCM Directories

* **Programmer's Directory** \(IEEE 1042: Dynamic Library\)
  * also called _working copy_
  * library for holding newly created or modified software entities
* **Master Directory** \(IEEE 1042: Controlled Library\)
  * manages the current baseline\(s\) and is for controlling changes made to them
  * changes must be authorized
* **Software Repository** \(IEEE 1042: Static Library\)
  * Archive for the various baselines released for general use
  * Copies of these baseline may be made available to requesting organizations

##### Version

* **Version:** An initial release or re-release of a configuration item associated with a complete compilation or recompilation of the item. Different versions have different functionality.
* **Release:** The formal \(external\) distribution of an approved version; e.g. a potentially shippable product increment in Scrum.
* **Promotion:** A version that is made available **internally** to other developers; e.g.  new commit in the version control system.
* **Revision:** Change to a version that correct only errors in the design / code, but does not affect the documented functionality.

##### Baseline

* A specification or product that has been formally reviewed and agreed to by the responsible management
* Thereafter is serves a the basis for further development and can be change **only** through change control procedures
* Example:
  * Baseline A: The API was completely defined. The bodies of the methods are empty
  * Baseline B: All data access methods are implemented and tested
  * Baseline C: The GUI is implemented

###### Types of Baselines

* As systems are developed, a series of baselines are developed \(usually\) after a review \(analysis review, design review, code review, system testing, ...\)
  * **Developmental Baseline**
  * **Functional Baseline**
  * **Product Baseline**
* Branch Management allows to transition between these baselines

###### Naming Scheme of Baselines \(Tagging\)

* Many naming schemes exist
* Example: **A3 Digit Scheme**
  * \[Major Release\].\[Minor Release\].\[Small Revision\]

### 3. SCM Activities

#### 3.1 Version Control \(Promotion Management\)

#### 3.2 Change Management

* Change Management is the handling of **change requests**
* The general change management **process:**
  * \[1\] A change is requested
  * \[2\] The change request is evaluated against requirements and project constraints and reviewed by the **configuration control board** 
  * \[3\] The change request is **approved** or **rejected**
  * \[4\] If it is approved, it is assigned to a developer, designed, implemented and tested
  * \[5\] The implemented change is audited to create another baseline

![](/assets/change_process.png)

##### Change Request

* Specifies the procedures for requesting a change to a baselined configuration item and the information to be documented
  * Name\(s\) and version\(s\) of the configuration item\(s\) where a problem appears
  * Originator's name and address
  * Date of request
  * Indication of urgency
  * The need for the change
  * Description of the requested change

##### Change Policies

* The purpose of the change policy is to guarantee that each promotion or release conforms to commonly accepted criteria
* Examples for Change Policies
  * _No developer is allowed to promote source code that was compiled with warnings or errors._
  * _No baseline can be released without having been beta-tested by at least 500 external testers._

##### Change Management Activities and Responsibilities

1. **Software Configuration Control** \(Managing a Change Request\)
2. **Software Configuration Status Accounting**
3. **Software Configuration Auditing**

###### 1. Software Configuration Control \(Managing a Change Request\)

* Define a change request form
* Define management procedure for
  * Identification of the need for a change request
  * Analysis and evaluation of a change request
  * Approval or disapproval of a change request
  * Implementation, Verification and Release of the change

###### 2. Software Configuration Status Accounting

* Answers the following questions
  * What elements are to be tracked and reported for baselines and changes?
  * What types of status account reports are to be generated? What is their frequency?
  * How is information collected, stored and reported?
  * How is access to the configuration management status data controlled?

###### 3. Software Configuration Auditing

* Identifies audits for the project.
* An **audit** determines for each configuration item, if it meets the required physical and functional characteristics.
  * Independent examination of a work product or a set of work products to assess compliance with specifications, standards, contractual agreements or other criteria
  * Audits are conducted according to a well-defined process consisting of various auditor roles and responsibilities
* The successful completion of an audit can be prerequisite for the establishment of the product baseline
* For each audit, the auditor has to define:
  * Objectives
  * Configuration Items under review
  * Schedule for the review
  * Procedures for conducting the review
  * Participants by job title
  * Required documentation
  * Procedure for recording deficiencies and how to correct them
  * Approval criteria

### 4. Summary

##### Software Configuration Management

* **Software Configuration Management**: A project function including 6 management activities within a software engineering process
  * **Promotions** are internal versions for other developers \(e.g. made available through version
    control\)
  * **Releases** are external versions for clients and users
* Change management controls how changes are handled in the process
* Distributed Version Control is state of the art and allows developers to collaboratively
  work on source code
  * benefits over centralized version control
* As developer and \(technology\) manager, you need to understand and use version control
* If you follow best practices, you work more efficiently and you avoid merge conflicts

##### Git

* Git is an example of a powerful and flexible distributed version control system which is widely used in practice
* You should be able to use the most important basic git commands
  * **Clone** a remote repository into your local file system
  * **Pull** changes from the remote into your local repository
  * **Commit** changes in your filesystem into your local repository
  * **Push** your local commits to the remote repository



