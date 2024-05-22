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

![delete test items1](https://imgur.com/clLk8gD.jpg) 

![delete test items2](https://imgur.com/9npV3VU.jpg) 

The password for the executable file was copied in order to access the file.
![copy pw](https://imgur.com/0U9MDqY.jpg) 

On the virtual machine, the executeable was ran in Powershell and unlocked with the aforementioned password.
![powershell process](https://imgur.com/FFyTmeT.jpg) 

The file was successfully accessed as shown below.
![powershell complete](https://imgur.com/JZ8D66n.jpg) 

## Backup Serivce - File Recovery Successly Completed

The backup can be found in the D drive where we can see the 'Test server' and 'backup sample' are available. 
![this pc server](https://imgur.com/y2QVWQq.jpg) 

![d drive](https://imgur.com/uyo7sDP.jpg) 

The virtual machine has been disconnected and the executeable file was then unmounted.
![unmounted1](https://imgur.com/pjlX3Xg.jpg) 

![unmounted2](https://imgur.com/3PWT9p7.jpg) 

## Backup via Restore 

This portion of the project will cover the process of restoring a full virtual machine from a backup. I ran into complications during the process and I will cover how I recovered and successfully completed the restore.

![restore vm start](https://imgur.com/sUyeDFV.jpg) 

The restore configuration process is displayed below and the backup restore asset has been named 'RecoveredVM'.

![restore config](https://imgur.com/hhwdkBh.jpg) 

The configuration has been successfully completed, timestamped 5/21/2024 1:31:18 PM.

![config complete](https://imgur.com/YjHN11Z.jpg) 

I retrieved the 'RecoveredVM' virtual machine in the Resource Group component and discovered the machine did not have a public IP address.

![recoveredvm](https://imgur.com/u2VQ8fM.jpg) 

![recoveredvm no ip1](https://imgur.com/1uzNzo2.jpg) 

![recoveredvm no ip2](https://imgur.com/6DkPGO0.jpg) 

GOOOO 

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
