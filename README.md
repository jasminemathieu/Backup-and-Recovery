# Backup-and-Recovery

<div align="center">

![Azure Backup Logo](https://imgur.com/VVl1i8B.jpg)

</div>

## Introduction

The Backup and Recovery project focuses on implementing Azure Backup services and two methods for ensuring fail-proof resource and data availability. By using this approach, we can achieve cost-effective, secure, and straightforward data backup and recovery solutions for valuable cloud-stored data. The ultimate goal is to maintain high availability for resources and critical data.

### Components Used

To complete this project, we utilize the following Azure components:

    Azure Resource Groups: Organizational containers for managing Azure resources.
    Azure Virtual Machine: A scalable, flexible compute resource in the cloud.
    Azure Recovery Services Vaults: Secure storage for backup data.
    Azure Public IP Addresses: Enables communication with resources over the internet.
    Microsoft Remote Desktop: Facilitates remote access to virtual machines.

## Project Setup

1. Creating the Virtual Machine (‘backup-vm’):
   -  Set up a new virtual machine named ‘backup-vm’
   -  Within the virtual machine’s C drive, create two test items: ‘Test server’ and ‘backup sample’

![new vm items](https://imgur.com/Ta484UI.jpg)

2. Configuring Backup Services:

    - Download the backup and site recovery service from Azure’s Marketplace
    - This service ensures that data, servers, virtual machines, and applications are accessible from a replicated environment
    - Configure the first backup for the ‘backup-vm’ virtual machine in the Recovery Service Vault
    - Choose the Enhanced policy subtype to automate full backups every 4 hours daily.

![backup config complete](https://imgur.com/HbQzm8E.jpg) 

# Part 1 - File Recovery

## First Backup Service Completed
The first full backup has been successfully created in the below image as timestamped at 5/21/2024 12:18:21 PM. File Recovery was selected to complete the next step to download the executable file to retrieve the backup on the 'backup-vm' machine. 

![first backup](https://imgur.com/I35AQGf.jpg)

After the executable file download was complete, test items previously created were deleted: 'Test server' and 'backup sample'. The success of the backup configuration process will be determined by if we can make the test items available for access again.

![delete test items1](https://imgur.com/clLk8gD.jpg) 

![delete test items2](https://imgur.com/9npV3VU.jpg) 

On the virtual machine, the executable was ran in PowerShell using C# scripting. I was able to successfully unlocked the access to the executable file with the password provided in Azure.
![powershell process](https://imgur.com/FFyTmeT.jpg) 

![powershell complete](https://imgur.com/JZ8D66n.jpg) 

## Backup Service - File Recovery Successfully Completed

The backup can be found in the D drive where we can see the 'Test server' and 'backup sample' are available. The virtual machine has been disconnected and the executable file was then unmounted.

![d drive](https://imgur.com/uyo7sDP.jpg) 

![unmounted2](https://imgur.com/3PWT9p7.jpg) 

# Part 2 - Restore VM

## Backup via Restore 

This portion of the project will cover the process of restoring a full virtual machine from a backup. I ran into complications during the process, and will cover how I was able to successfully completed the restore configuration and implementation process.

![restore vm start](https://imgur.com/sUyeDFV.jpg) 

The backup restore asset has been configured as displayed below, named 'RecoveredVM'. The configuration has been successfully completed, timestamped 5/21/2024 1:31:18 PM.

![config complete](https://imgur.com/YjHN11Z.jpg) 

After unsuccessful attempts of accessing the virtual machine, I discovered it did not have a public IP address.

![recoveredvm no ip2](https://imgur.com/6DkPGO0.jpg) 

I ran into complications when assigning a public IP address to the backup restore machine 'RecoveredVM'. Due to a subscription error, I was unable to complete the process. I had to recreate the vm machine and its restore machine as reflected below to complete the process.

![ip issues](https://imgur.com/kY2L63Y.jpg) 

![take2](https://imgur.com/xgzNybr.jpg) 

From here I was able to configure a public IP address for the 'RecoveredVM' machine

![ip config2](https://imgur.com/jLdUYgz.jpg) 

The IP address configuration was complete.
![ip complete](https://imgur.com/bbxLRhQ.jpg) 

I then created inbound rules to allow RDP for the machine.

![RDP config2](https://imgur.com/grXt9DB.jpg) 

![RDP confirmed](https://imgur.com/5VOZrtJ.jpg) 

## Successful Restore Confirmation
I was able to remote into the machine and confirm the restore machine duplication was successful.

![confirm restore](https://imgur.com/ep6oO7G.jpg) 

## Conclusion
In this project, I was able to successfully configure and complete a full cloud-native backup service and machine restore to 100% data availability in Azure. Both methods prove to be powerful on-premises data protection solutions, useful in events of service disruptions, accidental deletions or corruption of data. It's equally secure, scalable, and cost-effective as it is simple to architect, highly available, and resilient.

## fin
