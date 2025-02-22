#### Distributed (service-oriented)

##### Pros
- Independent Development: Each service can be developed
  independently by a team that is focused on that service.
- Independent Deployment: Services can be deployed independently.
  FBR (Feature-based Release)
- Fault Isolation: A process failure should not bring the whole system down.
- Mixed Technology Stack: Different services can use different technologies.

##### Cons
- Distributed System Complexity: Developers must deal with the additional
  complexity of creating a distributed system.
  Search: docker -> Kubernetes (namespaces)
- Development and Testing: Writing and testing applications is more difficult
  due to it being a distributed system.
  Nix: batch update test, 
- Data Management: Managing data consistency can be challenging.