## 10 Software Configuration Management II

###### 21 June - 27 June

###### Slides: [Moodle](https://www.moodle.tum.de/mod/resource/view.php?id=594684)

---

### 1. Branch and Merge Management

#### 1.1 Branch Management

* controls concurrent development 
* defines rules for creating and merging \(promoting\) branches

##### Example Branching Model

* **Master Branch:** External Releases \(e.g. Product Increment\)
  * external releases
* **Development Branch:** Promotions that can be used as internal releases
  * collection of promotions
  * candidates for releases
* **Feature Branches:** Incremental development and explorations
  * under control of one or more programmers

##### Merge Management with Pull Requests and Code Reviews

* Before changes in feature branches are merged \(promoted\) into the development branch, a reviewer reviews the changes
* The reviewer only approves changes, if the follow specified quality requirements

###### Code Review Workflow

![](/assets/code_review_workflow.png)

##### Best practices for branch and merge management

* Use branches to control concurrent development and explorations
* Agree on a workflow \(branching model\)
* Map backlog items / requirements to feature branches \(workflow automation\)
* Only one person at once works with non-merge-able files
  * Communicate with your team
  * Minimize the working time on such files
* **Important:** Minimize feature branch lifetime 
  * Split large requirements \(e.g. user stories, scenarios\) into smaller ones
  * Pull regularly from the development branch into the feature branch
  * Otherwise your branches might diverge heavily, resulting in serious, hard to resolve merge conflicts

#### 1.2 Feature Toggles

* In practice, some feature branches are open for a long time, due to large requirements and lazy or overburdened reviewers
* Therefore some teams have different development models
  * Only one branch exists
  * Each commit is reviewed
  * Feature toggles are used to activate features once they are finished

### 2. Summary

* A branching model controls the concurrent development and defines rules when branches are created and merged
  * structure development according to backlog items
  * work on the same codebase with multiple developers
* Pull Requests facilitate to communicate directly on the changed code
  * Only reviewed code \(high quality\) will be merged to development \(prevents broken window theory\)
  * Reduced overhead for code reviewers \(only changes need to be reviewed\)
  * Inexperienced team members improve their skills \(asynchronous pair programming\)
* Branch and Merge Management are important management activities to structure concurrent development



