# MuleSoft
Práctica MuleSoft Trainee

## Prerequisites
1. Download and install Rest Client (Postman, SOAP UI, etc).
2. Create an account in Anypoint Platform. [Link](https://anypoint.mulesoft.com/login/#/signup?apintent=generic)
3. Download and install MuleSoft's IDE (Anypoint Studio) [Download](https://www.mulesoft.com/lp/dl/studio)

## NOTE
If you want to show the first 7 activities you need to check hellomule repository.
The 8th activity is on the hellomule-2 repository.

### Tutorial file
If you want to show my tutorial document you have this link: [Document](Actividades.pdf)

### Build your first Hello Mule application  
[Link to MuleSoft Tutorial](https://developer.mulesoft.com/tutorials-and-howtos/getting-started/hello-mule/)  
In this tutorial you will create and deploy your first Mule application.
You will learn about environment, know some elements, their functions and how configure them.

### How to set up your global elements and properties files in Anypoint Studio  
[Link to MuleSoft Tutorial](https://developer.mulesoft.com/tutorials-and-howtos/getting-started/global-elements-properties-files/)  
You will learn to create global elements, these elements are important to have a better control of your project, your files will be better organized.
Also you will learn to do dynamic paths to declarate information like port, host, etc.

### Create your environments’ secure properties files  
[Link to MuleSoft Tutorial](https://developer.mulesoft.com/tutorials-and-howtos/getting-started/global-elements-properties-files/)  
It is very important to have your information secure, you must have the information protected.
You need validation to know that the information is secure and your sensitive information is protected (mainly passwords, keys, etc).
You learn to know to encrypt the information and configure these properties in CloudHub too.

### Create a new API in API Manager  
[Link to MuleSoft Tutorial](https://developer.mulesoft.com/tutorials-and-howtos/getting-started/how-to-setup-api-autodiscovery-anypoint-studio)  
You can create an API in the Anypoint Platform, the configuration, you can test in local and in CloudHub.
You will implement an autodiscovery to find the API's available automatically.
Yo do a connection wit the environment to detect the API's you create and after that you can enforce policies directly from API Manager without needing to redeploy your Mule application

### How to apply Client ID enforcement policy to your Mule app in API Manager  
[Link to MuleSoft Tutorial](https://developer.mulesoft.com/tutorials-and-howtos/getting-started/client-id-policy/)  
The policies are rules to request and responses from an API. Theses rules manage diferent things like security, authentication, authorization, etc.
You will implement a authentication policy and when you make a request, you will need to add a client and a secret authentication (password) in your configuration to receive a successful response.

### Best practices to design your first API Specification  
[Link to MuleSoft Tutorial](https://developer.mulesoft.com/tutorials-and-howtos/getting-started/best-practices-first-api-spec/)
**API**  
An API is a type of thechnology that allows applications to talk to one another.
The user sends a request to get a specific information, in response the systems returns data or functionality.

**API Specification**
When you make a request or response to an API you make using a format. The format RAML (RESTful API Modeling Language) and OAS (Open API Specification) provides the specific guidelines by which the API is built and communicates, just like an assembly guide ans user manual

**API Specification's components and best practices**
1. API Basics
   The specification must clearly state the title of the API, the industry standard,        need specify a base URI which is the URL in which your API is hosted and specify the     communication protocol.
2. Resources
   Use nouns as resources instead of verbs. This give more flexibility when you are         designing your resources since they are tightly coupled to a specific action.
3. Methods
   There are different HTTP request methods, and each one has different functions
    
| Method | Used for |  
| ---| --- |  
| GET    | Retrieving data. |  
| POST   | Creating data. |  
| PATCH  | Updating data. It will update partial data of an instance. |  
| PUT    | Updating data. It will update the entire instance. |  
| DELETE | Deleting data. |  

4. Query Parameters
Sorting can be a very expensive operation and it can lead to large costs down the road if not performed efficiently. You should offer a sorting operation such a sort or order_by. Filtering could be another useful feature to control results or restrict them based on certain values.

5. Status Codes
Each HTTP response status code have different mean. In the next table you can see the most popular status codes.

| Status Code | Meaning |
| --- | --- |
| 200 OK | The request was a success |
| 201 Created | A new resource was successfully created |
| 400 Bad Request | The server could not understand the request. The request needs to be modified before re-sending it |
| 401 Unauthorized | The request’s authentication is either missing or incorrect |
| 403 Forbidden | The request’s authentication succeeded, but the user does not have access to the resource |
| 404 Not Found | The server could not find the resource |
| 500 Internal Server Error | The server encountered an error |

**Build your first API Specification with API Designer**
You can configure your API manually, you need put the name, URI, communication methods.
The RAML and OAS code is automatically generated.
You can declarate Data Type, properties, specify the resources.
Each one of theses things build an API Specification and at the same time you are Design your API.

**How to configure an HTTPS endpoint in Anypoint Studio**
To enable HTTPS on localhost annd CloudHub endpoint, you need generate a keystore.jks, to do this you need use JDK keytool, when you execute this command you declarate some data like Name, Last Name, location, state, country, password, alias, etc.
The key contains these information and when you configure TLS to make the connection you need this key and these data (credentials).

**How to deploy from Anypoint Studio using Maven**
Maven manages the dependencies of a project.
settings.xml file which contains global settings for all Maven executions.
pom.xml contains details about project dependencies, plugins to use during compilation and build, build task configuration, and other essential information for Maven.
