#### Distributed (microservices)

##### Definition
- "Microservices" are a specific style of service-based architecture.
  In a microservices architecture, each service is small, independent, and 
  loosely coupled.
- "Microservices" run in their own process and communicate with other "services"
  using protocols such as HTTP/REST or messaging queues. They can be developed,
  deployed, and scaled independently, which offers more flexibility than traditional
  service architectures.
- users -> frontend (service) -> payments (microservice) -> database (instance)
- users -> frontend (service) -> users (microservice) -> database (instance)

- search: event buses
- search: queues