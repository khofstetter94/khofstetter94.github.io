# AWS: Events

[AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

- What is the difference betweeen SQS and SNS?
  - SNS is a distributed publish-subscribe service. Amazon SNS is a fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients. Amazon SNS makes it simple and cost effective to send push notifications to mobile device users, email recipients or even send messages to other distributed services.
  - SQS is distributed queuing service. Amazon SQS is a fully managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications. SQS is distributed queuing system. Messages are not pushed to receivers. Receivers have to poll SQS to receive messages.

- What are some use cases for both SNS and SQS?
  - Choose SNS if:
    - You would like to be able to publish and consume batches of messages.
    - You would like to allow same message to be processed in multiple ways.
    - Multiple subscribers are needed.
  - Choose SQS if:
    - You need a simple queue with no particular additional requirements.
    - Decoupling two applications and allowing parallel asynchronous processing.
    - Only one subscriber is needed.

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

- Describe how to use SQS and SNS in a “fanout” pattern.
  -
- Explain how “push notifications” work, using SNS.
  -

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

- How might a large scale, distributed application make use of a Queue system like SQS?
  - SQS can hold a lot of messages, for a long period of time, and will grow with your application.

## Things I want to know more about

-

[Return home](https://khofstetter94.github.io/reading-notes/)
