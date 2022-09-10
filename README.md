## About me
[LinkedIn profile](https://www.linkedin.com/in/raphael-derbier-572423/)

[Resume](/assets/Raphael-Derbier-Resume-2022.pdf)

##  work on Natural Language Processing

I have used a mix of NLP techniques and a concept of ontology to create a "Conversational" user interface where people can just ask questions about their data.
Presented at a user conference in 2018.

[![IMAGE_ALT](https://img.youtube.com/vi/OTVENGvS72A/2.jpg)](https://www.youtube.com/watch?v=OTVENGvS72A)


One of the key design decision in my NLP approach is to use a Graph Database as the underlying information storage. I have used [Dgraph](https:///dgraph.io) as their query language (DQL) was what I needed for this project.

Graph technology is an effective choice when you don't know in advance the type of queries and "joins" that you have to support. That's usually the case in all businesses where different data are interconnected.

Here is an example of the conversational query using airline data about flight operations.

[![IMAGE_ALT](https://img.youtube.com/vi/VnkoLH0v3DM/2.jpg)](https://youtu.be/VnkoLH0v3DM)

## work on Augmented Reality with Hololens

### The Bike challenge demo

At major events, we had a bike challenge and visitors could ride 30 seconds to do their best. Data is collected through sensors.
We extended this experience : a spectator can wear Microsoft Hololens and look at the challenge and see the performance data ...

[![IMAGE_ALT](https://img.youtube.com/vi/KxpOcxRj_S4/1.jpg)](https://youtu.be/KxpOcxRj_S4)


A quick explainer of the type of data that we have included in the demo:

[![IMAGE_ALT](https://img.youtube.com/vi/vuGVqoXPMYM/3.jpg)](
https://youtu.be/vuGVqoXPMYM)

By implementing this first innovation project I realized that using enterprise data in the context of Augmented Reality has some very valid uses cases. The following is the introduction of the presentation I gave with a friend of mine at Global XR conference in 2020 on this subject.

[![IMAGE_ALT](https://img.youtube.com/vi/sfKdBPEMWTs/3.jpg)](https://youtu.be/sfKdBPEMWTs)

The presentation also contained a "brief history of enterprise software architecture" which hopefully can help AR developers to better understand the enterprise software and data landscape (and it was fun to do !).

[![IMAGE_ALT](https://img.youtube.com/vi/MmUKlYyrHA4/3.jpg)](https://youtu.be/MmUKlYyrHA4)

## work on Serverless architecture

In 2020, our group has been asked to create an application that could help companies to get back to office safely given the COVID pandemic. We prototyped a working solution in 2 weeks and we could start offering it as a SaaS service with a companion mobile app (PWA) in 3 months. I was in charge of the requirements, design and architecture of the applicative part. We wanted to offer the solution for free. So it had to be very cost effective, production ready, able to scale. The solution is based on a case management engine and we have added a client application and a contact tracing capability which I created based on AWS stack : S3, Route53, CloudFront, API Gateway, Lambda functions and DynamoDB plus the necessary architecture for security (VPCs, security groups ...).
![IMAGE_ALT](/assets/GatherSmart.png)

I reused the same architecture for a business notification solution.
This time I have added a push notification capability using SNS and some logic in lambda triggered by DynamoDB streams.

DynamoDB keys are used in way to have a multi-tenant solution based on the user organization. The organization info is derived by a lambda custom authorizer on the API (serverless framework) which decode the JWT token of the user after login.

The final result is an extremely cheap solution to start with (<5$ per month !), scallable and which pass all our internal security tests (pen testing, port scanning ...).

It took 9 months from ideation to production. Given all the interactions you have to have in large companies (marketing, legal, cloud operations, ...), I can say it's really fast.
