# android-boilerplate
Clean architecture using SOLID principles and MVVM

## Clean Architecture & its Pros
1) Organise a project to achieve maintainability and scalability
2) One concern per component
3) Structured in layers of dependency
4) Implementation layers depends on abstract layers
5) Not only limited to mobile development
6) Strict architecture - hard to make mistakes
7) Business logic is encapsulated/seperated which makes it easy to use and test
8) Enforcement of dependencies through encapsulation
9) Allows for parallel development
10) Highly scalable
11) Easy to understand and maintain
12) Testing is facilitated
   
<img width="980" alt="Screenshot 2023-10-24 at 12 09 00 pm" src="https://github.com/nirvikBasnet/android-boilerplate/assets/46699486/0a8e7209-6319-490f-958c-980c26a3f4f4">

### Clean Architecture components

1) Domain Objects
    a) Foundational business logic
    b) POJOs

2) Use Cases
     a) Business logic, plain code 
     b) No other dependencies (do not depend on android system or particular architecture)
     c) A use case doesn't know how the result is going to be used

3) Controllers, presenters, adapters (Takes data from use cases transforms it and present it to upper layer) 
     a) Interfaces
     b) Retrieve data from various sources
     c) Present data in a specific format (e.g xml, JSON)
     d) Depend on lower level

4) Infrastructure
    a) How the data is interpreted and presented
    b) Most volatile layer, likely to change
    c) Interacts with interfaces to retrive data
    d) UI, Frameworks, devices etc
