Serverless Web Application Workshop

In this workshop you'll deploy a simple web application that enables users to request unicorn rides from the Wild Rydes fleet. The application will present users with an HTML based user interface for indicating the location where they would like to be picked up and will interface on the backend with a RESTful web service to submit the request and dispatch a nearby unicorn. The application will also provide facilities for users to register with the service and log in before requesting rides.

The application architecture uses AWS Lambda, Amazon API Gateway, Amazon S3, Amazon DynamoDB, Amazon Cognito, and AWS Amplify Console. Amplify Console hosts static web resources including HTML, CSS, JavaScript, and image files which are loaded in the user's browser via S3. JavaScript executed in the browser sends and receives data from a public backend API built using Lambda and API Gateway. Amazon Cognito provides user management and authentication functions to secure the backend API. Finally, DynamoDB provides a persistence layer where data can be stored by the API's Lambda function.

See the diagram below for a depiction of the complete architecture.

![image](https://user-images.githubusercontent.com/115881685/209079068-8814806e-6ac4-4bcd-b5a1-cff1a8a5c25e.png)

## Modules

This workshop is divided into four modules. Each module describes a scenario of what we're going to build and step-by-step directions to help you implement the architecture and verify your work.

1. [Static web hosting](https://github.com/georgeonalo/Serverless-Web-Application-1_StaticWebHosting-)

Deploy the static website using AWS Amplify Console by first creating a git repository (in either CodeCommit or GitHub) and then pushing the site code.

2. [User Management](https://github.com/georgeonalo/Serverless-Web-Application-2_UserManagement-)

Configure user management for the website using Amazon Cognito.

3. [Serverless Backend](https://github.com/georgeonalo/Serverless-Web-Application-3_ServerlessBackend-)

Create an AWS Lambda function that will persist data to an Amazon DynamoDB table.

4. [RESTful APIs](https://github.com/georgeonalo/Serverless-Web-Application-4_RESTfulAPIs-)


Expose the Lambda function via an Amazon API Gateway as a RESTful API that the static site can call.

⚠️ These modules are intended to be executed linearly.

After you have completed the workshop you can delete all of the resources that were created.

### Next

✅ Review and follow the directions in the [setup guide](https://github.com/georgeonalo/Serverless-Web-Application-0_Setup-), wherein you'll configure your AWS Cloud9 IDE and setup pre-requisites like an AWS Account.

