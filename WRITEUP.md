# Write-up Template
### If the site is still live, it can be viewed at [My Website](http://udacityh131.azurewebsites.net)
## Analyze, choose, and justify the appropriate resource option for deploying the app.
### Solution

I choose App Service to deploy the app
### Reason

+ App Service support python language
+ Quickly build and deploy, dont need to install the requirements
+ Easy to scaling and maintenance
+ I dont want to install software, python, or working with OS System
### Cost, Scalability, availability, workflow

+ Cost: I choose App Service because it's cheaper than VM and it has Free tier, here I chose Free tier
+ Scalability: Both the VM and the App Service have the ability to Scale in response to resource and traffic demands.
+ Availability : Both VM and App Service provide high availability, however the manner and scale of availability can vary between the two.
But our web application is simple and needs high availability, then Azure App Service might be a better choice.
+ Workflow : 
  + With Azure VMs, you must create and manage standalone virtual machines on Azure. This includes selecting and configuring the operating system, deploying applications and services, managing security, and updating the system. In this process, you have full control over your resources, but it also requires a lot of time and skill to deploy and manage virtual machines.
  + With Azure App Service, you can focus on deploying your application without having to manage virtual machines. Azure App Service provides simple environments for developing and deploying web, mobile, and API applications. You can deploy your application using tools like Git or DevOps, or upload application packages. App Service also provides features like auto-deployment, database services, and integration with popular development tools.
+ --> Here I need to deploy a simple Web application, no need to control the OS, so I choose App Service
### Assess app changes that would change your decision.

+ Although Azure App Service supports many programming languages, if our web app needs to change to a language that does not support for example "Rust", we will need to change to a virtual machine VM.
+  Need more control: When using a VM, you have greater control over every aspect of the system. You can install and configure system components, such as databases, server software, custom applications, and more. This may be necessary if you want to make more advanced customizations to your application.
+ When the amount of processing resources exceeds the necessary, the current App Service plan provides a maximum level of P5mv3 (32 vCPU, 256 GiB of memory) although it normally will not exceed this level, but if it is over the limit (processing Big Data), we can consider using a more extensible VM