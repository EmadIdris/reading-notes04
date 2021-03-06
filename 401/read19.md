
# Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server
![](https://d2908q01vomqb2.cloudfront.net/1b6453892473a467d07372d45eb05abc2031647a/2020/07/22/webserver5.png)

**Express is a web framework for Node.js . It simplifies the development of “serverless” web sites, web applications, and APIs. In a serverless environment, most or all of the backend logic is run on-demand in a stateless fashion (see Mike Roberts’ article on Serverless Architectures for a more detailed introduction). AWS Lambda, when used in conjunction with the new Amazon API Gateway features that I blogged about earlier this month (API Gateway Update – New Features Simplify API Development), allows existing Express applications to be run in serverless fashion. When you use API Gateway you have the opportunity to take advantage of additional features such as Usage Plans which allow you to build a developer ecosystem around your APIs, and caching which allows you to build applications that are responsive and cost-effective.**

# List the AWS Database offerings and talk about the pros and cons of each 
![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2018/07/Advantages-Disadvantages-of-AWS-01.jpg)
**Standard queues guarantee that a message is delivered at least once and duplicates can be introduced into the queue. FIFO queues ensure a message is delivered exactly once and remains available until a consumer processes and deletes it; duplicates are not introduced into the queue**

**FIFO queues are designed to ensure that the order in which messages are sent and received is strictly preserved and that each message is processed exactly once. Amazon SQS is a reliable and highly-scalable managed message queue service for storing messages in transit between application components.**

# How can the server be assured a message was properly received?
![](https://stackify.com/wp-content/uploads/2017/01/message-queue-793x397.jpg)
![](https://image.slidesharecdn.com/m05restapisandmq-190506110350/95/rest-apis-and-mq-12-638.jpg?cb=1557141036)

# What’s the difference between a FIFO and a standard queue?
| Term       |       Definition             |
| -----------|------------------------------|
|Serverless API|Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers. A serverless application runs in stateless compute containers that are event-triggered, ephemeral (may last for one invocation), and fully managed by the cloud provider.|
|Triggers|A trigger (from the Dutch trekken, meaning to pull) is a lever which, when pulled by the finger, releases the hammer on a firearm. In a database, a trigger is a set of Structured Query Language (SQL) statements that automatically "fires off" an action when a specific operation, such as changing data in a table, occurs.|
|Dynamo vs Mongo|DynamoDB is lightning fast (faster than MongoDB) so DynamoDB is often used as an alternative to sessions in scalable applications. DynamoDB best practices also suggests that if there are plenty of data which are less being used, move it to other table.|
|Dynamoose vs Mongoose|Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will be very familar/ Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node. js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.|