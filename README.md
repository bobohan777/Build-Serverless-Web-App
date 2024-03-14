# Build a Serverless Web Application
with AWS Lambda, Amazon API Gateway, AWS Amplify, Amazon DynamoDB, and Amazon Cognito


## **Overview**

Create a simple serverless web application that enables users to request unicorn rides from the [Wild Rydes](http://www.wildrydes.com/) fleet. The application will present users with an HTML-based user interface for indicating the location where they would like to be picked up and will interact with a RESTful web service on the backend to submit the request and dispatch a nearby unicorn. The application will also provide facilities for users to register with the service and log in before requesting rides.



## Prerequisites

- AWS CLI
- ArcGIS
- Notepad++
- Chrome
- AWS Lambda
- Amazon API Gateway
- AWS Amplify
- Amazon DynamoDB
- Amazon Cognito

## **Application architecture**

The application use AWS Amplify, Amazon Cognito, AWS Lambda, Amazon DynamoDB, Amazon API Gateway. 

Amplify Console provides continuous deployment and hosting of the static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser. 

JavaScript executed in the browser sends and receives data from a public backend API built using Lambda and API Gateway. 

Amazon Cognito provides user management and authentication functions to secure the backend API. Finally, DynamoDB provides a persistence layer where data can be stored by the API's Lambda function.

![alt text](image.png)

**Step 1: Static Web Hosting**

AWS Amplify hosts static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser.


**Step 2: User Management**

Amazon Cognito provides user management and authentication functions to secure the backend API.


**Step 3: Serverless Backend**

Amazon DynamoDB provides a persistence layer where data can be stored by the API's Lambda function.


**Step 4: RESTful API**

JavaScript executed in the browser sends and receives data from a public backend API built using Lambda and API Gateway.


(After this lab practice, Terminate all the resources you created throughout this lab.)


## **Part 1: Static Web Hosting with Continuous Deployment**

In static web content including HTML, CSS, JavaScript, images, and other files that will be managed by AWS Amplify console. End users will access to site using public website URL which exposed by AWS Amplify console. It’s no need to run any web servers or use other services to make site available.



## **Implementation**

**Select a region**

Choose **US East (N. Virginia)** region.

![alt text](image-1.png)


**Create Git repository**

Install AWS CLI

AWS CLI install by following reference.

https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html


Open AWS CodeCommit console


![alt text](image-2.png)


Create repository

![alt text](image-3.png)


Enter **wildrydes-site** for the **Repository name**.

Choose create

![alt text](image-4.png)


![alt text](image-5.png)












