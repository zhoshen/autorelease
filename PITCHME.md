# Raptor.io Release Automation 

Simplify and visualize raptor.io release

---

### Why

- Release process is painful and boring: developers should focus on solving problems or features and test cases development
- Hard to know components release dependency
- Hard to track release artifact release status
- Hard to support fine grained releases

---

### Architecture

![Release Explained](./images/)


---

### Intent Objects

- raptoriorelease
* abc

- artifact
* abc
- dependencyupdate
* bcd
- controllers (operators)
* release controller
* artifact controller
* pom dependency controller

---

### Release Dependency Service

- Calculate current release dependencies
- Input: release artifact and version
- Output: All artiafct releases and its dependencies

---

### Release Service

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### POM Service

- Dispatcher: Manages Data Flow
- Stores: Handle State & Logic
- Views: Render Data via React

---

### Q/A
