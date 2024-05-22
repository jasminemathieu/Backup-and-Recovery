# Backup-and-Recovery

![Azure Backup Logo](https://imgur.com/eNx24Bw.jpg)

## Introduction

This project covers the implementation of Azure Backup services. This service provides a cost effective, secure and simple solution to back up and recover valuebale data stored in the cloud. The result will be the high availablilty of valueable resources.

### Components used to complete this project:

- Azure Resource Groups
- Microsoft Remote Desktop

## Setup
We begin this project with the creation of a new virtual machine 'backup-vm'
![New VM Creation](https://imgur.com/J8OrCHq.jpg) 

Two new test items were created in the virtual machine's C drive, 'Test server' and 'backup sample'. 
![new vm items](https://imgur.com/Ta484UI.jpg)

![backup in marketplace](https://imgur.com/yqvzmIa.jpg) 

### New User Configuration Check
As observed in the below image, globalreaderjohn's assigned role has been successfully implemented as the user is unable to make password changes for other users. 

![Confirmation of successful assignment](.jpg)

## Assigning Subscription-level Role
In this section of the project, subreaderjane was assigned a subscription-level role as a reader. 

![Assign reader role](.jpg)

![Assign reader role2](.jpg)

![Assign reader role4](.jpg) 

### Subscription-level Role Assignment Check
As shown below while signed in under subreaderjane's account, the assigned role has been successfully implemented as marked under the "My role" column. 

![Confirmation of role assignment](.jpg) 

## Assigning Resource Group-level Contributor Permissions

Resource group 'Permissions Tester' has been created in this section. In Access Control (IAM), found within the Subscription component, we are able to add the Privileged administrator role of a Contributor to user rgcontributordave.

![resource group](.jpg)

![assigning group](.jpg)

![assigning group2](.jpg)

### Resource Group-level Contributor Permissions Assignment Check

The below two images are references to indicate the Resource Group-level Contributor role was correctly configured. The top image reflects all resource groups under the admin account. The second image documents the only one resource group, Permissions Tester, that was assigned to rgcontributordave. 

![confirm correct rg assignment](.jpg) 

![confirm correct rg assignment2](.jpg) 


## Conclusion
System administrator key skills include system maintenance and health monitoring, thus ensuring that their company's computers, servers, and internet are always available. This includes setting up and maintaining the system and installing, debugging, and evaluating a new technology for their businesses.
