# Software patterns, module 2
### Description:
###### Since description of the task was a little blurred, here I will provide explanation how I understood and designed it
- Core element is ***Project***. Project can have multiple ***Modules***. Each module represent individual part of project, such as Mobile app, Database, Web app and so on.
- To build (i.e. develop) project, to each of its Modules is attached ***Pipeline***. 
Each pipeline consists of multiple ***Stages*** (e.g. Designing, Developing, Testing, Delivering, etc.).
Stage may contain direct logic, or can contain another Stages (***CompoundStage***), which will be executed recursively as current Stage is executed (**`Composite pattern`**)
- Each module has a ***Team*** assigned to it. Each Team contains **TeamMember**s, these can be **Developer**, **BusinessAnalist**, **QA**,
- Developers can take additional role as a **SoftfareArchitect** or **TeamLead**, by wrapping themselves in corresponding wrappers (***`Decorator pattern`***)
- Each Developer also has main **Technology** (it can be **JS** or **Python**) (***`Bridge pattern`***)
### Conceptual UML diagram:
![UML diagram](https://github.com/olehhaliak/university-patterns-module2/blob/master/Conceptual%20UML%20diagram.png)
