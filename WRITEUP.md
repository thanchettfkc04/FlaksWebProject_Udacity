# Write-up Template

## Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
### Solution
I choose App Service to deploy the app
### Reason
+ App Service support python language
+ Quickly build and deploy, dont need to install the requirements
+ Easy to scaling and maintenance
+ I dont want to install software, python, or working with OS System
### Cost, Scalability, availability, workflow
+ Cost: App Service is cheaper than VM
+ Scalability, availability : In terms of scalability and availability, both are rated equally
+ Workflow : While working with VM, we need to install environment, necessary libraries, software and then deploy, with App Service, we can use CI/CD with Github
### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
+ If the app uses another language not supported by App Service, I will use VM
+  If one day we need to control the whole operating system, we will need to change to VM
+ If the resources we need to use exceed the resources App Service can provide, we need to change to a VM