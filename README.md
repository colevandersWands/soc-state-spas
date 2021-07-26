# new objectives

Separation of Concerns -> State -> Single Page Apps

## lesson plans

rough plans for each Sunday:

- **Separation of Concerns**
  1. function roles (handlers, logic, components, procedures), reverse-engineering steps (HTML+CSS, listener, handler, refactor logic/components)
  2. nested DOM stuff, event delegation
  3. developing and testing components
- **State**
  1. what is state, component hierarchies render parts of state
  2. group project code review (a blog?)
- **SPAs**
  1. what is a spa, frontend routing
  2. group project code review (rewriting same project as last module)

---

## Projects

Each module will have it's own project scope and folder structure that builds on the previous module.

- **Separation of Concerns**: Given a simple website with 1-2 user interactions, a student can reverse-engineer the behavior following the steps and code splitting defined in this module.
  - _Language Level_\*: HTML5, CSS3, synchronous JS, DOM, event listeners + handlers, unit tests for logic and components
  - _Environment_: modern Browsers, and any JS environment that supports jest/jasmine-style BDD syntax - `describe`, `it`, `expect(_).toEqual(_)`
  - _Technologies_: JS and a unit testing environment, linting, CI, ...
  - _Starter_: a repository containing code quality scripts, github actions, testing configurations, folder structure, planning, ...
  - _Assessment Criteria_: do the CI checks pass, are the correct steps present in their branches and commit history, does it work, ...
- **State**: a website built around pre-defined data (maybe a simple blog?). largely projects are the same as the last module, conceptually students are approaching the project with a data-first mindset instead of UI-first
  - _Language Level_: HTML5, CSS3, synchronous JS, DOM, event listeners + handlers, unit tests for logic and components
  - _Environment_: modern Browsers, and any JS environment that supports jest/jasmine-style BDD syntax - `describe`, `it`, `expect(_).toEqual(_)`
  - _Technologies_: JS and a unit testing environment, linting, CI, ...
  - _Starter_: a repository containing code quality scripts, github actions, testing configurations, folder structure, planning, ...
  - _Assessment Criteria_: do the CI checks pass, are the correct steps present in their branches and commit history, does it work, does the project use state in a clear way, are there reusable components with a `test.html`, ...
- **Single Page Apps**: rebuild the same project as last module as a SPA, `<div id='root'>`, frontend routing, page components, ...
  - _Language Level_: HTML5, CSS3, synchronous JS, DOM, event listeners + handlers, unit tests for logic and components
  - _Environment_: modern Browsers, and any JS environment that supports jest/jasmine-style BDD syntax - `describe`, `it`, `expect(_).toEqual(_)`
  - _Technologies_: JS and a unit testing environment, linting, CI, frontend routing, ...
  - _Starter_: a repository containing code quality scripts, github actions, testing configurations, folder structure, planning, routing infrastructure, ...
  - _Assessment Criteria_: do the CI checks pass, are the correct steps present in their branches and commit history, does it work, does the project use state in a clear way, are there reusable components with a `test.html`, ...

> - \* language level: a subset of JavaScript adequate to build the project. students should limit their study to this language subset so they can focus on skill integration instead of extra language or paradigm complexity. Features not in the language subset can fall into different categories including: applicable to the task but out of scope, irrelevant to the task, or counterproductive (like using classes when a project is functional, or AJAX if a project is focusing on fetch)

---

## Learning Objectives

the module has multiple learning objectives determined by the sub-skills required to complete the module's project. they all have priorities/depths to help students and coaches can manage their efforts.

- 🥚: a student can apply this skill comfortably within the module's learning task with access to references. A learning task submitted at the end of the module should demonstrate proficiency in these objectives.
- 🐣: a student can apply this skill with effort and frequent support from references. A learning task submitted at the end of the module should demonstrate partial application of these skills.
- 🐥: a student understands the basic zoomed-out idea of this skill but may not be comfortable or proficient applying it. A learning task submitted at the end of the module may include attempts at applying these skills.
- 🐔: learning this skill is not required for the module's learning task but is relevant, if the student shows appropriate mastery of 🥚, 🐣 and 🐥 objectives. A learning task submitted at the end of the module should not demonstrate these skills if the higher priorities are not accounted for.

### Separation of Concerns

- 🥚 **event-driven programming**: identify the concept in a JS program via listeners & handlers
- 🥚 **entry points**: describe what an entry point is, there are 2 kinds in the programs for this module - initialization & interaction. identify them in a program
- 🥚 **function roles**: describe what function roles are and why they're important. they can identify a function's role given checklists for each role covered in this module: logic, handlers, components, procedures
- 🥚 **DOM access**: a student read and write values from the DOM in an event handler
- 🥚 **es5 vs. es6**: a student can demonstrate the change in developer-experience pre and post es6 by stepping through in the debugger and explaining differences in scoping (global vs. script, block vs. local, modules) between two programs with identical user experience but different implementations.
- 🥚 **Scope Hierarchy**: A student is comfortable navigating different scopes in the browser's debugger to understand an existing application (script, module, closure, local, block)
- 🥚 **Code Splitting**: A student can es modules to split their code into multiple files & folders according to function role, data, listeners and initialization. They can use generated dependency diagrams and documentation to understand and navigate this folder structure.
- 🐣 **reverse-engineering**: a student can incrementally reverse-engineer a level-appropriate user interaction following these steps: ui -> listener -> handler (-> logic and/or -> component)
- 🐣 **Naming Functions**: a student can come up with clear and helpful names for the functions in their program. A good function name will take into account the function's role and the program's domain
- 🐣 **DOM manipulation**: a student can manipulate the DOM when implementing level-appropriate user interactions
- 🐣 **Isolating Components**: a student can use a `test.html` file to render their components with different inputs
- 🐣 **Forms**: a student can do basic handling of form data via `event.target`
- 🐣 **Handling events**: a student can use the `event` argument to process user interactions, including bubbled events using `event.target`
- 🐣 **Passing Component Unit Tests**: a student can write vanilla DOM component functions to pass provided unit tests
- 🐥 **refactoring**: refactor a single-script tutorial-style web page into multiple files using imports and exports
- 🐔 **Writing Component Unit Tests**: a student can write unit tests to validate their component functions

### State

- 🥚 **State**: A student can explain the concept of state as the incremental changes occurring in program data between user interactions. They can read a well-structured log of initial and subsequent states to infer a user's journey with a level-appropriate program.
- 🥚 **Data-Driven Development**: A student understands applications as data + user interactions. They can demonstrate this by explaining how user stories can be applied directly to program state without going through a UI.
- 🐣 **Nested Data**: Given a nested data structure containing arrays, objects and primitive values, a student can 1) access a given value 2) update a given entry 3) extract and/or summarize subsets of the data
- 🐣 **Matching a JSON Schemas**: A student can write an object or array that matches a given schema.
- 🐣 **Rendering State**: Given a wireframe (or example site), data, and an HTML structure: a student can render the data to create a web page similar to the wireframe
- 🐣 **Reusing Components**: Given a wireframe and state data, a student can create a component hierarchy and a test/demo page for each component.
- 🐥 **Matching a JSON Schemas**: A student can write JS data that matches a schema
- 🐥 **Writing a JSON Schemas**: A student can write a JSON schema that matches several data instances.

### Singe Page Apps

- 🥚 **Page Components**: A student understands the concept of a single component "replacing" and HTML file. They can demonstrate this by creating component hierarchies for a given multi-page wireframe.
- 🐣 **Planning a SPA**: Students can work together to develop a SPA by developing + testing pages and components in isolation before merging
- 🐣 **Frontend Routing**: A student understand the concept of frontend routing. They can demonstrate this by explaining how URLs can be updated without refreshing the page by rendering a different page component.
- 🐔 **`history`**: a student can use the `history` API to manage browser url's in a small side-project
