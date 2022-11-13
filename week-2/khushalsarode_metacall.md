Link to the Article => https://aviyel.com/post/3829/what-is-function-as-a-service-faas-in-cloud-computing

# {What is Function-as-a-Service (FaaS) in Cloud Computing}
**Introduction**

Nowadays, [cloud computing](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-cloud-computing/) is being widely used in the IT industry. It is because entities are only entitled to pay for the services they use on the platform. Cloud computing is the servers, storage units, databases, networking, software, analytics, and intelligence and computational infrastructure located at multiple locations, whereas each (location) is referred to as a data center, which we use on-demand as per necessity. The cloud is secure, faster, more convenient, and flexible.

The cloud provides main three types of services:

1. **Infrastructure-as-a-Service (IaaS)**
    
2. **Platforms-as-a-Service (PaaS)**
    
3. **Software-as-a-Service (SaaS).**
    

So, that's a background study for the topic of discussion.

## What is Function as a Service?

Prior to that, as you are all aware, a function is a block of code that is designed to solve or provide specific functionality in a program.

That is the same concept as how functions are used as a service in cloud computing!

Didn't get it?

Faas is a type of cloud computing service that provides a platform for customers to develop, run, and manage application functionalities without the complexity of building and maintaining the infrastructure that is typically associated with developing and launching an app.

## Various start-ups, such as PiCloud, first offered FaaS around 2010.

When we host an application in the cloud, we must manage the application's resources. However, when we use a function as a service, the provider manages all of these resources automatically. We can manage and interact with applications and cloud functions directly without hosting.

The function as a service is compatible with and supports languages such as [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript), [Linux](https://www.linux.org/), and [HTML](https://www.w3schools.com/html/) code. This function is triggered by events and does not require any infrastructure.

In general, each function should store one functionality. They are held accountable for every execution.

## Overview

FaaS is a subset of the larger serverless computing concept. Servers do exist, but they are abstracted as much as possible. You don't have to be concerned about maintenance, security, or elasticity. Everything scales based on the number of requests received.

All that remains is to build your function and assign it a trigger. When triggered, the serverless computing service creates a container in milliseconds that runs your code and returns the desired result. The result can be a computational output or a JavaScript output, among other things.

  

![](/cdn-cgi/image/format=auto/https://lh5.googleusercontent.com/lg64wjTJMhcdG_ejcfCpaVJn9NGbqgkkoshkd8or3P5gbdv9eEAPDbsBO7i1bo16F1yu9mNgKpGLoJBwwDEBBUGjkddlbuU8sCqK8aI-vlLDDu-u-oZ5TMmv_FkNWrx6C2NCioW_EE5E-oCEMEYYcZnXSyj0g7SR77rhSoeev1v9plgCM6J09vhy5Q)

  

Providers of cloud services that support FaaS

- [Metacall](https://metacall.io/)
    
- [IBM Cloud Functions](https://cloud.ibm.com/functions)
    
- [Microsoft Azure Functions](https://learn.microsoft.com/en-us/azure/azure-functions/functions-overview) (open source)
    
- [AWS Lambda](https://aws.amazon.com/lambda/), by Amazon
    
- [Google Cloud Functions](https://cloud.google.com/functions)
    
- [OpenFaaS](https://www.openfaas.com/) (open source)
    
- [Cloudflare workers](https://workers.cloudflare.com/)
    
- [Twilio functions](https://www.twilio.com/docs/serverless/functions-assets/functions)
    
- [Netlify functions](https://www.netlify.com/products/functions/)
    
- [Alibaba functions](https://www.alibabacloud.com/product/function-compute)
    

## What Is the Difference Between Serverless and FaaS?

FaaS is not the same as, but a subset of, Serverless. Serverless computing focuses on a specific service category, such as databases, messaging, APIs, or storage, where the management, configuration, and billing of servers are invisible to end users. FaaS, on the other hand, is one of the most important serverless architecture technologies. It focuses on event-driven computing paradigms in which entire application codes are only executed in response to requests.

How Exactly Does Faas Work? A function as a service is an event-driven code stored remotely on the cloud that is executed when the website requests it to perform specific tasks.

For example, if you want to convert files from one format to another, you upload the file, which is then passed on to the function in the data center, which processes the file and returns the required output to the website.

A function is essentially a microservice that can only respond to an event by performing one action. When a function is triggered, the provider will launch a server. It will run the function before shutting down the server. When the server is shut down, the same computing resources can be allocated elsewhere because serverless offerings are only active when the function is being used.

## Reasons to Use FaaS

There are numerous advantages to utilizing FaaS architecture. Here are a few reasons why you might want to use FaaS for your application:

- The ability to focus solely on coding and development for your application.
    
- Cost savings by paying for only what you use.
    
- The ability to [auto-scale](https://www.techtarget.com/searchcloudcomputing/definition/autoscaling) without capacity planning or ongoing maintenance
    
- Faster time to market due to the ease of development and testing
    
- FaaS's runtime is extremely fast and takes milliseconds. For those used to the minutes or hours other systems take to run, this speed doesn’t compute.
    
- No capacity planning is required. Unlike other models, FaaS requires no capacity planning.
    

## Consideration when using Faas service

### 1\. Make each function perform only one action:

FaaS functions should be designed to perform a single task in response to an event. Make your code scope as small, efficient, and lightweight as possible so that functions load and execute quickly.

### 2\. Don’t make functions call other functions:

The value of FaaS is in function isolation. Too many functions will increase your costs and negate the value of function isolation.

### 3\. Use as few libraries as possible in your functions:

Using too many libraries can slow down functions and make them difficult to scale.

## What are the advantages of using FaaS?

### 1\. Improved developer velocity

This reduces software development time because developers spend more time implementing logic and less time worrying about servers and deployment when using functions as a service.

Built-in scalability Developers do not need to worry about preparing for high traffic or heavy use. All scaling issues will be handled by the serverless provider.

Cost efficiency Serverless FaaS providers, unlike traditional cloud providers, do not charge their clients for idle computation time. As a result, clients only pay for the computation time they use and do not waste money over-provisioning cloud resources.

### 2\. A Robust Cloud Infrastructure

Because it is spread across multiple availability zones per geographic region, FaaS provides inherent high availability and can be deployed across any number of regions without incurring additional costs.

## What are the drawbacks of FaaS?

### 1\. Reduced System Control

Having a third party manage part of the infrastructure makes it difficult to understand the entire system and complicates debugging.

### 2\. More Complexity Required for Testing

It can be difficult to integrate FaaS code into a local testing environment, making thorough application testing more difficult.

### 3\. Security Issues

FaaS may introduce security risks such as malicious hacking and data leakage. Users may gain access to each other's sensitive data if elements such as Google Cloud functions are running on a multi-tenancy server.

### 4\. Transparency

The backend infrastructure is less transparent with FaaS. FaaS is difficult to budget for with a pay-per-use model.

## Conclusion

Here you are! I hope you understand theoretically the Function as a service in cloud computing. Most of the important topics you should know about FaaS are covered above but keep in mind that this may be what you're looking for. To learn more about FaaS, head over to this site for a comprehensive technical reference on FaaS and cloud computing in general.
