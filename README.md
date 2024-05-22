# Backup-and-Recovery

![Azure Backup Logo](https://imgur.com/eNx24Bw.jpg)

## Introduction

This project covers the implementation of Azure Backup services and two methods of creating fail proof resource and data availability. This method provides a cost effective, secure and simple solution to back up and recover valueable data stored in the cloud. The result will be the high availablilty of resources and data.

### Components used to complete this project:

- Azure Resource Groups
- Azure Virtual Machine
- Azure Recovery Services Vaults
- Azure Public IP Addresses
- Microsoft Remote Desktop

## Setup

We begin this project with the creation of a new virtual machine 'backup-vm'

![New VM Creation](https://imgur.com/J8OrCHq.jpg) 

Two new test items were created in the virtual machine's C drive, 'Test server' and 'backup sample'. 
![new vm items](https://imgur.com/Ta484UI.jpg)

## Configuring Backup Services

The backup and site recovery service was implemented for Azure's marketing place in the effort to provide a cloud backup solution for data and ensure servers, virtual machines, and apps can easily fail over to a replicated environment and continue working.

![backup in marketplace](https://imgur.com/yqvzmIa.jpg) 

![](https://imgur.com/umayheb.jpg)

As observed in the below image, globalreaderjohn's assigned role has been successfully implemented as the user is unable to make password changes for other users. 

![Assign reader role2](https://imgur.com/CSv5EoM.jpg)

![Confirmation of successful assignment](https://imgur.com/NN4ft2U.jpg)

In this section of the project, subreaderjane was assigned a subscription-level role as a reader. 

![Assign reader role2](https://imgur.com/zDvU54U.jpg)

![Assign reader role4](https://imgur.com/HbQzm8E.jpg) 

### New User Configuration Check

### Subscription-level Role Assignment Check
As shown below while signed in under subreaderjane's account, the assigned role has been successfully implemented as marked under the "My role" column. 

![Confirmation of role assignment](https://imgur.com/mD9MRR3.jpg) 

## Assigning Resource Group-level Contributor Permissions

Resource group 'Permissions Tester' has been created in this section. In Access Control (IAM), found within the Subscription component, we are able to add the Privileged administrator role of a Contributor to user rgcontributordave.

![resource group](https://imgur.com/biy8lOE.jpg)

![assigning group](https://imgur.com/I35AQGf.jpg)

![assigning group2](https://imgur.com/VVrfpz2.jpg)

### Resource Group-level Contributor Permissions Assignment Check

The below two images are references to indicate the Resource Group-level Contributor role was correctly configured. The top image reflects all resource groups under the admin account. The second image documents the only one resource group, Permissions Tester, that was assigned to rgcontributordave. 

![confirm correct rg assignment](https://imgur.com/JJc32w8.jpg) 

![confirm correct rg assignment2](https://imgur.com/clLk8gD.jpg) 

![confirm correct rg assignment](https://imgur.com/9npV3VU.jpg) 

![confirm correct rg assignment2](https://imgur.com/0U9MDqY.jpg) 

![confirm correct rg assignment](https://imgur.com/FFyTmeT.jpg) 

![confirm correct rg assignment2](https://imgur.com/RzMOGby.jpg) 

![confirm correct rg assignment](https://imgur.com/JZ8D66n.jpg) 

![confirm correct rg assignment2](https://imgur.com/y2QVWQq.jpg) 

![confirm correct rg assignment](https://imgur.com/uyo7sDP.jpg) 

![confirm correct rg assignment2](https://imgur.com/pjlX3Xg.jpg) 

![confirm correct rg assignment](https://imgur.com/3PWT9p7.jpg) 

![confirm correct rg assignment2](https://imgur.com/sUyeDFV.jpg) 

![confirm correct rg assignment](https://imgur.com/hhwdkBh.jpg) 

![confirm correct rg assignment2](https://imgur.com/YjHN11Z.jpg) 

![confirm correct rg assignment2](https://imgur.com/u2VQ8fM.jpg) 

![confirm correct rg assignment](https://imgur.com/1uzNzo2.jpg) 

![confirm correct rg assignment2](https://imgur.com/6DkPGO0.jpg) 

![confirm correct rg assignment](https://imgur.com/9yrEbSF.jpg) 

![confirm correct rg assignment2](https://imgur.com/3zhNJj2.jpg) 

![confirm correct rg assignment](https://imgur.com/wuBs00M.jpg) 

![confirm correct rg assignment2](https://imgur.com/NDCOkIn.jpg) 

![confirm correct rg assignment](https://imgur.com/iVhRTr2.jpg) 

![confirm correct rg assignment](https://imgur.com/dkvsrQW.jpg) 

![confirm correct rg assignment2](https://imgur.com/5rru1Cm.jpg) 

![confirm correct rg assignment](https://imgur.com/6B3uxiK.jpg) 

![confirm correct rg assignment2](https://imgur.com/YJfbEOW.jpg) 

![confirm correct rg assignment](https://imgur.com/qOmki3q.jpg) 

![confirm correct rg assignment](https://imgur.com/kEV6hto.jpg) 

![confirm correct rg assignment2](https://imgur.com/rOdtJxg.jpg) 

![confirm correct rg assignment](https://imgur.com/kY2L63Y.jpg) 

![confirm correct rg assignment2](https://imgur.com/pr2QEhw.jpg) 

![confirm correct rg assignment](https://imgur.com/cYi6Ato.jpg) 

![confirm correct rg assignment](https://imgur.com/OtnhbfZ.jpg) 

![confirm correct rg assignment2](https://imgur.com/xgzNybr.jpg) 

![confirm correct rg assignment](https://imgur.com/Jg0wPv3.jpg) 

![confirm correct rg assignment2](https://imgur.com/jLdUYgz.jpg) 

![confirm correct rg assignment](https://imgur.com/bbxLRhQ.jpg) 

![confirm correct rg assignment](https://imgur.com/MEm7v7o.jpg) 

![confirm correct rg assignment2](https://imgur.com/grXt9DB.jpg) 

![confirm correct rg assignment](https://imgur.com/5VOZrtJ.jpg) 

![confirm correct rg assignment2](https://imgur.com/xnPY4cZ.jpg) 

![confirm correct rg assignment](https://imgur.com/ep6oO7G.jpg) 

## Conclusion
System administrator key skills include system maintenance and health monitoring, thus ensuring that their company's computers, servers, and internet are always available. This includes setting up and maintaining the system and installing, debugging, and evaluating a new technology for their businesses.
