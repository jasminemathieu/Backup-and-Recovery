# Backup-and-Recovery

![Azure Backup Logo](https://imgur.com/GI2Y8rr.jpg)

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

# Part 1: File Recovery
This part of the project will focus on creating a robust backup system and ensuring successful file recovery as shown in the following steps:

1. Backup Creation: We’ve successfully completed the first full backup, timestamped at 5/21/2024 12:18:21 PM. This initial backup is crucial for data safety.

2. Executable File Download: After creating the backup, we downloaded it as an executable file. This file will help us retrieve the backup on the ‘backup-vm’ machine.
 
![first backup](https://imgur.com/I35AQGf.jpg)

3. Test Items Deletion: As part of our testing process, we intentionally deleted test items (‘Test server’ and ‘backup sample’). Our goal now is to recover these deleted files.

![delete test items1](https://imgur.com/clLk8gD.jpg) 

![delete test items2](https://imgur.com/9npV3VU.jpg) 

4. Recovery Process: On the virtual machine, we executed the downloaded executable using PowerShell and C# scripting. Successfully unlocking access to the executable file using the provided Azure password was a critical step.

![powershell process](https://imgur.com/FFyTmeT.jpg) 

![powershell complete](https://imgur.com/JZ8D66n.jpg) 

5. Backup Verification: The backup is stored in the D drive. We can confirm that ‘Test server’ and ‘backup sample’ are available. Additionally, we disconnected the virtual machine and unmounted the executable file.

![d drive](https://imgur.com/uyo7sDP.jpg) 

![unmounted2](https://imgur.com/3PWT9p7.jpg) 

With these steps completed, our Backup Service - File Recovery is now successfully configured.

# Part 2: Restore VM
In this section of the project, we delve into the process of restoring a full virtual machine from a backup. Despite encountering complications, I successfully completed the restore configuration and implementation. Let’s break it down:

1. Initial Configuration:
   - The backup restore asset, named ‘RecoveredVM,’ was configured (as shown in the image below) and timestamped at 5/21/2024 1:31:18 PM.
   - However, attempts to access the virtual machine failed due to the absence of a public IP address.

![restore vm start](https://imgur.com/sUyeDFV.jpg) 

![config complete](https://imgur.com/YjHN11Z.jpg) 

2. Addressing IP Issues:
 - I encountered challenges while assigning a public IP address to the backup restore machine.
 - Subscription errors hindered the process, leading me to recreate both the VM and its restore machine (as reflected in the images below).

![recoveredvm no ip2](https://imgur.com/6DkPGO0.jpg) 

![ip issues](https://imgur.com/kY2L63Y.jpg) 

![take2](https://imgur.com/xgzNybr.jpg) 

3. Successful IP Configuration:
   - Eventually, I configured a public IP address for the ‘RecoveredVM’ machine (as seen in the image below).

![ip config2](https://imgur.com/jLdUYgz.jpg) 

![ip complete](https://imgur.com/bbxLRhQ.jpg) 

4. Inbound Rules for RDP:
   - To ensure remote desktop access, I created inbound rules.
   - Confirming successful restore machine duplication with a remote access to the duplicate machine validated my efforts (see confirmation images below).

![RDP config2](https://imgur.com/grXt9DB.jpg) 

![RDP confirmed](https://imgur.com/5VOZrtJ.jpg) 

![confirm restore](https://imgur.com/ep6oO7G.jpg) 

## Conclusion
This project demonstrates the power of cloud-native backup services and machine restoration in Azure. Whether facing service disruptions, accidental deletions, or data corruption, these solutions provide robust on-premises data protection. They combine security, scalability, cost-effectiveness, and architectural simplicity.

