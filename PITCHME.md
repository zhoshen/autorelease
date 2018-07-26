## Raptor.io Release Automation 

Simplify and visualize raptor.io release

---

### Why

- Release process is painful and boring: developers should focus on solving problems or features and test cases development
- Hard to know components release dependency
- Hard to track release artifact release status
- Hard to support fine grained release controls

---

### Architecture

![Release Explained](./images/autorelease_arch.png)


---
### Intent Objects
- RaptorIORelease: top level release object
- Artifact: each individual release object
- DependencyUpdate: object to sync with pom update service
- Controllers (operators)
  * release controller
  * artifact controller
  * pom dependency controller
---
### Release Dependency Service

- Calculate current release dependencies
- Input: release artifact and version
- Output: all release artifacts and its dependencies

---

### Release Service

- Release service integrated with Jenkins and maven repo
- Build: using declared Jenkins file
- Release: dynamically created release pipeline stages for different types of artifacts

---

### POM Service

- Keep monitor the snapshot artifact and the new release artifacts
- Update pom dependency with the release artifact

---

### Demo
- Release monitor dashboard
- Command Line Query
- Test example demo

---

### Q/A
