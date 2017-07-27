## 13 Build Management

###### 5 July - 11 July

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=601002)

---

### 1. SCM: Build Management

##### Requirements for Build Management

Large and distributed software project need to provide a development infrastructure with an integrated build management that supports:

* regular builds from the master directory
* automated execution of tests
* email notifications
* determination of code metrics
* automated publishing of the application and test results

###### Tools for Build Managements

* Unix's Make
* Ant 
* Maven

##### Activities in Build Management

The transition from source code to executable application contains many mechanical \(usually boring\) activities.

* Setting required paths and libraries
* Compiling Source Code
* Copying source files
* Setting file permissions
* Packaging the application

Executing these steps manually is time consuming and the chance of introducing failures is high.

##### Reasons for Continuous Integration

* **Risk 1:** The later the integrations occurs in a project, the bigger the risk that unexpected failures occur.
* **Risk 2:** The higher the complexity of the software system, the more difficult is the integration of its components.
* Continues Integration addresses these risks **by integrating and testing as early and frequently as possible.**

### 2. Overview: Testing and Continuous Integration

##### Motivation

* Faults are everywhere

##### Terminology

* **Failure:** Any deviation of the observed behavior from the specified behavior
* **Error:** \(Erroneous State\) The system is in a state such that further processing by the system can lead to failure
* **Fault:** The mechanical or algorithmic cause of an error \(informally: bug\)
* **Validation:** Activity of checking for deviations between the observed behavior of a system and its specified behavior

##### Fault Handling Techniques

* **Fault Avoidance**
  * use methodology to reduce complexity
  * use software configuration management to prevent inconsistency
  * apply verification to prevent algorithmic faults
  * use review to identify faults already in the design
* **Fault Detection**
  * Testing: Provoke failures in a planned way
  * Debugging: Find and remove faults
  * Monitoring: Deliver information about the state and unusual behavior \(used during debugging\)
* **Fault Tolerance**
  * Exception Handling, modular redundancy

###### Taxonomy of Fault Handling Techniques

![](/assets/fault_handling_techniques.png)

##### Testing Activities

![](/assets/testing_activities.png)

###### Types of Testing

* **Unit Testing:**
  * individual components \(class or subsystem\) are tested
  * carried out by developers
  * **Goal:** confirm that the component or subsystem is correct and carries out the intended functionality
* **Integration Testing:**
  * Groups of subsystems \(collection of subsystems\) and eventually the entire system are tested
  * carried out by developers
  * **Goal:** test the interfaces between the subsystems
* **System Testing**
  * the entire system is tested
  * carried out by developers
  * **Goal:** determine whether the system meets the requirements \(functional and non-functional\)
* **Acceptance Testing**
  * evaluates the system delivered by developers
  * carried out by the client and may involve executing typical transactions on site
  * **Goal:** demonstrate that the system meets the requirements and is ready to use

###### Acceptance Testing

* **Goal:** demonstrate that the system is ready for operational use
  * many tests can be taken from integration and system testing
  * choice of tests is made by the client
  * executed by the client, not the developer
* **Alpha Test:**
  * client uses the software at the developer's environment
  * software usage in a controlled setting with the developer ready to fix bugs
* **Beta Test:**
  * conducted in the client's environment \(developer not present\)
  * software gets realistic workout in target environment

##### Definition: Continuous Integration

_A software development technique where team members integrate their work frequently. Usually each person integrates at least daily, leading to multiple integrations each day._

=&gt; Each interaction is verified by an automated build, which includes the execution of tests \(regression tests\) to detect errors as quickly as possible.

###### Advantages

##### Regression Testing 

### 3. Summary



