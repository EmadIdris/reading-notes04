# What are serverless functions?

![](https://cdn-media-1.freecodecamp.org/images/1*x_v5NRC3TTMt1MaYl1gMUg.jpeg)
**Serverless computing is an execution model for the cloud in which a cloud provider dynamically allocates—and then charges the user for—only the compute resources and storage needed to execute a particular piece of code. Serverless functions are event-driven, meaning the code is invoked only when triggered by a request.**

# If you were to create a system that emulated Lambda functions, how would you do it?
![](https://openupthecloud.com/wp-content/uploads/2020/11/docker-lambda.png?ezimgfmt=rs:342x188/rscb2/ng:webp/ngcb2)

1- Open the Functions page on the Lambda console. 
2- Choose Create function.
3- Under Basic information, do the following: 
  a- For Function name, enter my-function. 
  b- For Runtime, confirm that Node.js 14.x is selected. Note that Lambda provides runtimes for .NET (PowerShell, C#), Go, Java, Node.js, Python, and Ruby. 
4- Choose Create function. 

**Lambda creates a Node.js function and an execution role that grants the function permission to upload logs. The Lambda function assumes the execution role when you invoke your function, and uses the execution role to create credentials for the AWS SDK and to read data from event sources.**

# Describe how a CDN works (Content Delivery Network)
![](https://www.globaldots.com/hs-fs/hubfs/cdne.png?width=590&name=cdne.png)
**To minimize the distance between the visitors and your website's server, a CDN stores a cached version of its content in multiple geographical locations (a.k.a., points of presence, or PoPs).In essence, CDN puts your content in many places at once, providing superior coverage to your users.**

| Term       |       Definition             |
| -----------|------------------------------|
|Serverless Functions|Serverless is a cloud-native development model that allows developers to build and run applications without having to manage servers. There are still servers in serverless, but they are abstracted away from app development|
|Cloud Storage|Cloud storage uses data centers with massive computer servers that physically store the data and make it available online to users via web. Users can remotely upload their content, store them and retrieve the data as and when required.|
|CDN|The most common use case of a CDN is to cache content and deliver it to the end-user, reducing the zpage load time. This means that the content should be cached on the CDN edge as long as possible. ... For example, your CDN has stored, on its edge servers, a copy of the black Nike running shoe that we talked about earlier|

