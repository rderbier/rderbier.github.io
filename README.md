## About me
[LinkedIn profile](https://www.linkedin.com/in/raphael-derbier)

[Resume](/assets/Raphael-Derbier-Resume.pdf)

## Natural Language Processing (NLP) & Conversational Interfaces

### Graph-Powered Conversational Query Engine
In 2018, I have used a mix of NLP techniques and a concept of ontology to create a "Conversational" user interface where people can just ask questions about their data in plain english. A pre-LLM project !

- Developed a **natural language interface** for querying complex datasets, combining **NLP techniques** and **ontology-based graph databases**.
- **Key innovation**: Used **[Dgraph](https://dgraph.io/)** for its flexible query language (DQL), enabling dynamic queries of interconnected business data.
- **Use case**: Demonstrated with airline flight operations data, allowing users to ask questions conversationally.
- **Presented at a user conference in 2018**.

📺 **[Demo: Conversational Query Engine](https://youtu.be/OTVENGvS72A)**
📺 **[Demo: Airline Data Use Case](https://youtu.be/VnkoLH0v3DM)**

> Graph technology is an effective choice when you don't know in advance the type of queries and "joins" that you have to support. That's usually the case in all businesses where different data are interconnected.



## Augmented Reality (AR) with Microsoft HoloLens

### The Bike challenge demo

At major events, we had a bike challenge and visitors could ride 30 seconds to do their best. Data is collected through sensors.
We extended this experience : a spectator can wear Microsoft Hololens and look at the challenge and see the performance data ...

[![IMAGE_ALT](https://img.youtube.com/vi/KxpOcxRj_S4/1.jpg)](https://youtu.be/KxpOcxRj_S4)


A quick explainer of the type of data that we have included in the demo:

[![IMAGE_ALT](https://img.youtube.com/vi/vuGVqoXPMYM/3.jpg)](
https://youtu.be/vuGVqoXPMYM)

By implementing this first innovation project I realized that using enterprise data in the context of Augmented Reality has some very valid uses cases. 

The following is the introduction of the presentation I gave with a friend of mine at Global XR conference in 2020 on this subject.

[![IMAGE_ALT](https://img.youtube.com/vi/sfKdBPEMWTs/3.jpg)](https://youtu.be/sfKdBPEMWTs)

The presentation also contained a "brief history of enterprise software architecture" which hopefully can help AR developers to better understand the enterprise software and data landscape (and it was fun to do !).

[![IMAGE_ALT](https://img.youtube.com/vi/MmUKlYyrHA4/3.jpg)](https://youtu.be/MmUKlYyrHA4)

## Serverless Architecture: Scalable, Cost-Effective Solutions


### GatherSmart: Safe Return-to-Office SaaS (2020)
In 2020, our group has been asked to create an application that could help companies to get back to office safely given the COVID pandemic. 
- **Challenge**: Build a **COVID-safe office reentry solution** in **2 weeks** (prototype) and **3 months** (production SaaS + PWA).
- **Role**: Led **requirements, design, and architecture** for a **case management engine** with **contact tracing**.
- **Tech stack**: AWS (**S3, Route53, CloudFront, API Gateway, Lambda, DynamoDB**), with **VPCs and security groups** for compliance.
- **Result**: A **multi-tenant, scalable solution** costing **< $5/month** to start, passing all security tests (pen testing, port scanning).

![IMAGE_ALT](/assets/GatherSmart.png)

### Business Notification System
- Reused the **serverless architecture** to build a **push notification system** using **SNS** and **DynamoDB streams**.
- **Multi-tenancy**: Achieved via **custom Lambda authorizers** decoding JWT tokens for user organization context.

