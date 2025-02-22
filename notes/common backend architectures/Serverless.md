#### Serverless

##### Definition 
- Serverless architecture refers to applications that significantly depend
  on third-party services (backend-as-a-service or "BaaS") or on custom code that's run in ephemeral
  containers (function as a service or "FaaS)
  BaaS - Firebase, Supabase
  FaaS

###### Overview
- Serverless architectures, the app logic is still run on servers, but 
  all the server management is done by the cloud provider (AWS, Azure, GCP, etc.). 
  You just need to run your code, and the cloud provider takes care of the rest.

Example
- users (traffic) -> frontend (serverless)
- users (traffic) -> API Gateway (serverless) -> addToCart(function) -> database (serverless)
- users (traffic) -> API Gateway (serverless) -> processOrder(function) -> database(serverless)
- frontend master -> frontend (serverless)


###### Pros
- No server management is required.
- Costs based on usage, not on pre-purchased capacity.
- Automated scaling. (rate limiting, thresholds, bill alerts)


###### Cons
- The architecture can be more expensive for long-term applications
- Testing can be difficult due to the environment's reliance on the internet.
- Troubleshooting and debugging is also more complex.


##### Use Cases
- Real-time file processing: As soon as a file is uploaded in S3, AWS Lambda can
  trigger a function to process it.
- Real-time stream processing: Perform real-time analytics on data
  streams using Kinesis.
- Extract, Transform, Load (ETL): Perform ETL on demand. For example,
  when a new file is uploaded to S3, AWS Lambda can trigger to process the data
  and load it into a database.
- Websites: Websites that are purely static (HTML, CSS, JavaScript) can be served
  from S3 directly.