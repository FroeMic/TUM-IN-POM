## 007 Software Configuration Management I

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

### 3. SCM Activities

#### 3.1 Version Control \(Promotion Management\)

#### 3.2 Change Management

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



