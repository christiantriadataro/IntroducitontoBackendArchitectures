## Introduction to Backend Architectures

### Three commonly used architectures
- Monolithic
- Distributed (sercive-oriented)
- Serverless

### Monolithic

#### Definition
- Monolithic architecture is a model where all the necessary
  code and components for a software application are combined
  into a single unit.
- users -> Frontend & Backend (monolith) -> Database (instance)


#### Overview
- Monolithic architecture has all functionalities tightly coupled,
  running in the same system.
- This architecture is simple to develop, test, and deploy due to its unified system.

##### Pros
- Simplicity: Easier to develop, test, and deploy due to unified system.
- Consistency: Allows for uniformity in handling requests as every module 
  uses the same set of procedures.
- Efficiency: Since all the functionalities are interconnected,
  it can be more efficient in terms of inter-process communication.

###### Cons
- Limited Scalability: Scaling specific functions of a system is not possible.
  The entire system needs to be scaled.
- Lack of Flexibility: Changes to a single component can require the entire system
  be redeployed.
- Complexity: The system can become too complex and hard to manage as the 
  application grows.