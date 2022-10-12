# AWS: API, Dynamo and Lambda

[AWS API Gateway Overview](https://www.serverless.com/guides/amazon-api-gateway)

- What is Amazon API Gateway?
  - Amazon API Gateway is a managed service that allows developers to define the HTTP endpoints of a REST API or a WebSocket API and connect those endpoints with the corresponding backend business logic. It also handles authentication, access control, monitoring, and tracing of API requests.
- Why is Amazon API Gateway an important part of the Serverless ecosystem?
  - Within the Serverless ecosystem, API Gateway is the piece that ties together Serverless functions and API definitions. Being able to trigger the execution of a Serverless function directly in response to an HTTP request is the key reason why API Gateway is so valuable in Serverless setups: it enables a truly serverless architecture for web applications.
- How does API Gateway integrate with other AWS services?
  - Many AWS services support integration with Amazon API Gateway, including:
    - AWS Lambda: run Lambda functions to generate HTTP API responses.
    - AWS SNS: publish SNS notifications when an HTTP API endpoint is accessed.
    - Amazon Cognito: provide authentication and authorization for your HTTP APIs.
  - API Gateway supports direct integrations that can be configured in the API Gateway user interface (or via the API Gateway’s own API) for the following actions:
    - Invoking an AWS Lambda function.
    - Invoking another HTTP endpoint, with or without VPC Link.
    - Making an HTTP call against the API of any AWS service that provides an HTTP API.
    - Returning a mock response generated within API Gateway without calling out to other services.

[AWS API Gateway](https://aws.amazon.com/api-gateway/)

- What are the some benefits of using Amazon API Gateway?
  - Efficient API development, performance at any scale, cost saving at scale, easy monitoring, flexible security controls, RESTful API options
- What two API types might you choose from?
  - RESTful APIs and WEBSOCKET APIs

[AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

- What is DynamoDB?
  - DynamoDB is a hosted NoSQL database offered by Amazon Web Services (AWS). It offers:
    - reliable performance even as it scales;
    - a managed experience, so you won't be SSH-ing into servers to upgrade the crypto libraries;
    - a small, simple API allowing for simple key-value access as well as more advanced query patterns.
- Under what circumstances would you recommend DynamoDB over MongoDB?
  - For applications with large amounts of data and strict latency requirements, for serverless applications using AWS Lambda, or with data sets with simple, known access patterns

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

- Explain to a non-technical friend how DynamoDB works.
  - Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in security, continuous backups, automated multi-Region replication, in-memory caching, and data import and export tools.

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction)

- What is Dynamoose?
  - Dynamoose is a modeling tool for Amazon's DynamoDB.
- What are some key features of Dynamoose?
  - Type safety
  - High level API
  - Easy to use syntax
  - DynamoDB Single Table Design Support
  - Ability to transform data before saving or retrieving items
  - Strict data modeling (validation, required attributes, and more)
  - Support for DynamoDB Transactions
  - Powerful Conditional/Filtering Support
  - Callback & Promise support
  - AWS Multi-region support

[Return home](https://khofstetter94.github.io/reading-notes/)
