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

Two new test items were created in the virtual machine's C drive, 'Test server' and 'backup sample' as reflected in the below image.
![new vm items](https://imgur.com/Ta484UI.jpg)

## Configuring Backup Services

The backup and site recovery service was downlaoded from Azure's Marketplace. The backup and site recovery service provides a cloud solution that ensures data, servers, virtual machines, and applications can be easily accessible from a replicated environment. 

![backup in marketplace](https://imgur.com/yqvzmIa.jpg) 

![downloading backup service](https://imgur.com/umayheb.jpg)

![review and create backup service](https://imgur.com/CSv5EoM.jpg)

Below displays the configuration process of the first backup for virtual machine 'backup-vm' in the Recovery Service Vault.
![config backup for vm](https://imgur.com/NN4ft2U.jpg)

The Enhanced policy sub type was choosen to automate a full backup every 4 hours daily.
![backup config selection](https://imgur.com/zDvU54U.jpg)

![backup config complete](https://imgur.com/HbQzm8E.jpg) 

## First Backup Service Completed
The first full backup has been successfully created in the below image as timestamped at 5/21/2024 12:18:21 PM. File Recovery was selected to complete the next step to download the executeable file to retrieve the backup on the 'backup-vm' machine. 

![first backup](https://imgur.com/I35AQGf.jpg)

![exec file gen](https://imgur.com/VVrfpz2.jpg)

![exec dl](https://imgur.com/JJc32w8.jpg) 

After the executeable file download was complete, test items previously created were deleted: 'Test server' and 'backup sample'. The success of the backup configuration process will be determined by if we can make the test items available for access again.

![confirm correct rg assignment2](https://imgur.com/clLk8gD.jpg) 

![confirm correct rg assignment](https://imgur.com/9npV3VU.jpg) 

The password for the executable file was copied to 
![confirm correct rg assignment2](https://imgur.com/0U9MDqY.jpg) 

![confirm correct rg assignment](https://imgur.com/FFyTmeT.jpg) 

![confirm correct rg assignment2](https://imgur.com/RzMOGby.jpg) 

![confirm correct rg assignment](https://imgur.com/JZ8D66n.jpg) 

## 123
![confirm correct rg assignment2](https://imgur.com/y2QVWQq.jpg) 

![confirm correct rg assignment](https://imgur.com/uyo7sDP.jpg) 

![confirm correct rg assignment2](https://imgur.com/pjlX3Xg.jpg) 

![confirm correct rg assignment](https://imgur.com/3PWT9p7.jpg) 

![confirm correct rg assignment2](https://imgur.com/sUyeDFV.jpg) 

##efg
![confirm correct rg assignment](https://imgur.com/hhwdkBh.jpg) 

![confirm correct rg assignment2](https://imgur.com/YjHN11Z.jpg) 

![confirm correct rg assignment2](https://imgur.com/u2VQ8fM.jpg) 

![confirm correct rg assignment](https://imgur.com/1uzNzo2.jpg) 

##hijk
![confirm correct rg assignment2](https://imgur.com/6DkPGO0.jpg) 

![confirm correct rg assignment](https://imgur.com/9yrEbSF.jpg) 

![confirm correct rg assignment2](https://imgur.com/3zhNJj2.jpg) 

![confirm correct rg assignment](https://imgur.com/wuBs00M.jpg) 

## lmno
![confirm correct rg assignment2](https://imgur.com/NDCOkIn.jpg) 

![confirm correct rg assignment](https://imgur.com/iVhRTr2.jpg) 

![confirm correct rg assignment](https://imgur.com/dkvsrQW.jpg) 

![confirm correct rg assignment2](https://imgur.com/5rru1Cm.jpg) 

![confirm correct rg assignment](https://imgur.com/6B3uxiK.jpg) 

## pqrs
![confirm correct rg assignment2](https://imgur.com/YJfbEOW.jpg) 

![confirm correct rg assignment](https://imgur.com/qOmki3q.jpg) 

![confirm correct rg assignment](https://imgur.com/kEV6hto.jpg) 

![confirm correct rg assignment2](https://imgur.com/rOdtJxg.jpg) 

![confirm correct rg assignment](https://imgur.com/kY2L63Y.jpg) 

## 456 
![confirm correct rg assignment2](https://imgur.com/pr2QEhw.jpg) 

![confirm correct rg assignment](https://imgur.com/cYi6Ato.jpg) 

![confirm correct rg assignment](https://imgur.com/OtnhbfZ.jpg) 

![confirm correct rg assignment2](https://imgur.com/xgzNybr.jpg) 

![confirm correct rg assignment](https://imgur.com/Jg0wPv3.jpg) 

## jasmine
![confirm correct rg assignment2](https://imgur.com/jLdUYgz.jpg) 

![confirm correct rg assignment](https://imgur.com/bbxLRhQ.jpg) 

![confirm correct rg assignment](https://imgur.com/MEm7v7o.jpg) 

![confirm correct rg assignment2](https://imgur.com/grXt9DB.jpg) 

## mother
![confirm correct rg assignment](https://imgur.com/5VOZrtJ.jpg) 

![confirm correct rg assignment2](https://imgur.com/xnPY4cZ.jpg) 

![confirm correct rg assignment](https://imgur.com/ep6oO7G.jpg) 

## Conclusion
System administrator key skills include system maintenance and health monitoring, thus ensuring that their company's computers, servers, and internet are always available. This includes setting up and maintaining the system and installing, debugging, and evaluating a new technology for their businesses.
