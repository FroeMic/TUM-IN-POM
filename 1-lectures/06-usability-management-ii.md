## 06 Usability Management II

###### 31 May - 6 June

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=588466)

---

### 1. Prototyping

##### Revolutionary vs. Evolutionary Prototyping

| **Revolutionary Prototyping** | **Evolutionary Prototyping** |
| :--- | :--- |
| =&gt; get user experience with a **throwaway** version | =&gt; used as the **basis** for the implementation |
| **Advantage:** Can be developed in a short amount of time | **Advantage:** Short time to market |
| **Disadvantage:** Users may have to accept that features in the prototype are too expensive to implement | **Disadvantage:** Can be used only if the target system can be constructed in a prototype |

##### Low Fidelity vs High Fidelity Prototyping

| | **Advantages** | Disadvantages |
| :--- | :--- | :--- |
| **Low Fidelity** | | |
| | - Easy to Produce | - Mostly not reused |
| | - More Feedback | - Important details are ignored |
| | - No design decisione | |
| **High Fidelity** | | |
| | - More realistic | - May cause much effort |
| | - More detailed problems can be | - Less feedback |
| | - More impressive | - High expectations \(especially with interactive prototypes\) |

##### Risk of Prototyping

* Developer may become attached to the prototype
* Excessive development time of the prototype
* Customer might not appreciate how much work must be done to turn a prototype into a fully functional system
* User may confuse prototype with finished system
* Negative feelings towards the software, if the prototype has problems
* Cost of implementing a prototype

##### Managing Expectations

* Non-Programmers will use the state of the UI as a proxy for estimating how far program development is
* 90% worse UI =&gt; user will thing the program is 90% worse
* 100% beautiful UI =&gt; user will think program is almost finished

##### Storyboarding

* Modeling the UI as a Finite Automation
* Makes it possible to navigate through the UI with the users
* Often models can be used to generate code
* Allows to **combine evolutionary prototyping with low-fidelity prototyping**

### 2. Human Capabilities

##### Model of the User as a cognitive machine

* **Perceptual Processor**: Eyes, Ears
* **Motor Processors**: Muscles
* **Cognitive** Processor: Brain
* Long-term / working memory

###### Processor Cycle Times

* **Cycle Time** = time to accept an input an produce an output
* Eyes / Ears \[50ms - 200ms\]
* Muscles \[25ms - 170ms\]
* Brain \[30ms - 100ms\]

##### Fitt's Law

* Specifies how fast you can move your hand \(mouse\) to a target of certain size at a certain distance without overshooting it.
* Time = a + b \* log \(Distance / TargetSize + 1\)

###### Consequences

* Targets at the screen edge are easy to hit \(no correction cycle needed\)
* Hierarchical menus are hard to hit \(many correction cycles\)
* Pie menus are faster than popup menus \(each menu item is the same distance away from the pointer\)

##### Model of the Human Memory

###### Memory Attributes

* Encoding: type of things stored
* Size: number of things stored
* Decay Time: How long does the memory last?

###### Long Term Memory

* Large Capacity
* Little decay
* Elaborative practice moves chunks from short term memory to long term memory by making connections with other chunks

###### Short Term Memory

* Capacity: 7 ± 2 chunks
* Fast Access Time: ~70ms
* Fast Decay: 7\*\[5s - 226s\]
* depends on number of chunks
* distraction destroys short term memory
* Interference: A distraction where different stimuli activate conflicting chunks
* these chunks are harder to retain in short term memory
* example: color names, written in a different color

##### Noise in communication

* Explanation for _interference example with colors_
* at school we learned that words are more important than color
* saying the color of each word slows us down
* making a choice between conflicting options slows us down
* When projects become complex many choices need to be made
* Preferences and practices learned may unconsciously make decisions, when the requirements of a technology or system are not completely understood

### 3. Summary

##### Benefits of Prototyping

* Prototypes allow to get early feedback —> save time while developing
* Prototypes are easier to understand than text or diagrams —> easier communication
* Prototyping improves the usability

##### Prototyping Risks

* Wrong expectations about the progress of non-programmer
* User confusion between prototype and finished system

##### Other

* **Human capabilities** are limited: users rely on clues (e.g. natural mapping, affordances) in
order to learn from the design model
* **Fitt’s Law**: how fast you can move your hand to a target of a certain size at a certain distance
* Natural Mapping and Affordances are clues that help us to design user interfaces


