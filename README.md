# university
A template for a website of unviersity

References:

https://www.bu.edu/academics/cas/courses/cas-ma-577/

examples/virtual-machines/linux/basic-password/main.tf

https://careers.bcg.com/job/BCG1US10031495EXTERNALENUS/Visiting-Software-Engineer--internship-?userId=ncdh5q8q3k27u6hehf1ks6lbdl&utm_source=phenom&utm_medium=email&utm_campaign=5fb63de1c9e77c000683a343-1663339841-JobAlertsubscriptionCampaignWeeklyEnglish(US)

-
Azure Infrastructure Fundamentals
Lesson Overview
Play Video
Course outline highlight lesson 2: Azure Infrastructure Fundamentals.
Welcome to lesson 2! In this lesson we will cover Azure Infrastructure Fundamentals. Specifically, we will learn:

What the various IaaS resource types are that we can deploy.
How to use the in-portal wizard to deploy a virtual machine.
How to do virtual networking and load balancing, which will be critical for our project at the end of the course.
How to use Azure Monitor to optimize virtual machine performance and cost.
How to use Azure Active Directory for role-based access controls, users, and service principals.
How to use the Azure CLI (instead of the portal) to deploy resources.
When to use Azure portal vs. Azure CLI.
-
Azure Infrastructure Fundamentals
Udacity Cloud Lab are the on-demand-labs that provide you access to the Azure cloud services without having you set up your own Azure account.

Students can opt in to use Udacity Cloud Lab to create and manage Azure resources (say VMs, databases, or any other) for the exercise and project in this program. The Cloud Lab eliminates the time and complexity involved in setting up and managing an Azure account. However, there are several restrictions and resource constraints when using this Cloud Lab, as described below.

Accessing the Cloud Lab and Azure credentials
Udacity Cloud Lab will generate a pair of temporary credentials for you to use on the Azure Portal https://portal.azure.com/ . Here are the steps:

Click on the ACCESS LAB button. Wait until the Cloud Lab loads. It could take up to 10 minutes to load.
You can expand the right collapsible pane to copy the Azure login credentials available in the Lab Environment tab. Use those credentials to log into the Azure Portal in a separate browser tab.
Tip: Access the Cloud Labs from an incognito browser to have a seamless experience.

Choose to skip the two-factor authentication when prompted.

Choose to skip the two-factor authentication when prompted
Choose to skip the two-factor authentication when prompted

Getting Help
If you have a technical problem while loading your VM or permission issues, you can send an email to Udacity Support at udacity-labsupport@udacity.com. Please be sure to send your message from the email you used to enroll in the Nanodegree program.

Please copy the below text into your email and fill out the following information:

Subject Line: Error in [Lab name]
Timestamp and Timezone
Brief description of what you were doing when the issue occurred
Screenshots
The udacity-labsupport@udacity.com email is specifically for Azure lab support. Please review the following options to get the right support you need from the Udacity team.

Review the Udacity FAQ - Your question may have already been answered! Search through our FAQ first.
Submit a question via Knowledge Hub - Knowledge Hub is where you can ask questions specific to the course or Nanodegree you’re enrolled in. This is mainly to get that one on one feedback from mentors in a way similar to the real world using Stack Overflow.
Submit a support ticket - If your question/issue can’t be answered in the FAQ or Knowledge Hub, you can submit a support ticket to escalate to the correct Udacity team. If you are an enterprise customer, please use the following link.
Submit feedback directly in the classroom - If you find an issue with a piece of content on a lesson page, you can use the “SEND FEEDBACK” button at the top right of the classroom screen. You’ll be given the option to choose which part of the page has the issues and provide more details for the Udacity maintenance team to review.
Important Considerations/Restrictions
Session duration: Each cloud lab has a fixed session duration (a few hours), shown on the classroom lab page. The lab will shut down and clean up all resources after the session ends, meaning, you will lose all your resources in the temporary Azure account. Note that we do not preserve the resources after the session ends; therefore, try finishing the exercises built on each other in one stretched attempt. After the session ends, you will have to refresh the classroom lab page, regenerate a fresh new cloud lab, and start over from scratch. You can track the session time as shown in the snapshot below.
Cloud Lab - Remaining session time
Cloud Lab - Remaining session time

New session - After your session expires, you can start a new session by refreshing the Cloud lab classroom page, you will get a new pair of temporary Azure credentials.
Idle timeout: We monitor your classroom lab page activities and automatically delete the "idle" lab after a specific duration of inactivity. Therefore, we recommend accessing the Azure portal (https://portal.azure.com) within the lab, not on a separate browser tab.
You will not be able to create additional Resource Groups. There is one resource group already created for you named cloud-demo-XXXXXX. There might be instructions present in your classroom to create a Resource Group, but you should use the existing Resource Group instead.
Backup - Preserve your steps/commands to create the resources. It will help to replicate the environment in the new session.
Parallel access - We have put a cap on the maximum number of parallel connections allowed per user to curb any potential abuse.
Resource group - You will not be able to create resource groups. Instead, you have to use the eixsting resource group. Udacity cloud lab offers a shared subscription among multiple learners, and each learner is given a pre-created resource group within that shared subscription.
Cloud Lab - Predefined Resource Group
Cloud Lab - Predefined Resource Group

Active Directory: You will not be able to create Active Directory resources. This is not a requirement for any project/exercise.
Virtual Machine type:
When you create a new Virtual Machine, make sure to choose allowed size and disk-type, otherwise, the Azure portal may trigger a "Validation failed" error message.

VM Size: You are permitted to use any of the sizes mentioned-below while creating a Virtual machine:

Standard_B1s
Standard_B2s
Standard_B2ms
Standard_DS1_v2
Standard_DS2_v2
Standard_D2s_v3
OS Disk Type: Change the default disc type from "Premium SSD" to "Standard HDD"

Cloud Lab - Changing the default disc type from "Premium SSD" to "Standard HDD"
Cloud Lab - Changing the default disc type from "Premium SSD" to "Standard HDD"

Log Analytics: You will not be able to create Log Analytics workspace resources. Instead, you will get a pre-created Log Analytics workspace in your account. You can use the existing Log Analytics workspace for your exercises, wherever applicable. See the snapshot below.
The pre-created Log Analytics workspace in your account.
The pre-created Log Analytics workspace in your account.

Use the Resource ID of the existing Log Analytics workspace for your exercises, wherever applicable.
Use the Resource ID of the existing Log Analytics workspace for your exercises, wherever applicable.

General: For each service, select the "Free" or the "Standard" pricing tier. Use a sensible and meaningful naming convention for all your resources. Use a consistent location, say East US 2, for the all resources/services. These are the consumption-based service and you will be charged based only on actual usage.
If you are not familiar with Azure, you can ignore the restriction points above. You will learn about them while doing the hands-on.

-
Azure Infrastructure Fundamentals
Intro to Infrastructure as a Service
Infrastructure as a Service (IaaS) consists of many resource types, including:

Storage
Compute
Networking
Databases
…and more!

In this course, we explore just a handful of these resource types.

Infrastructure as a Service (IaaS) vs. Platform as a Service (Paas)
Play Video
Note: We do not explore Platform as a Service (PaaS) offerings in this course, but you should be aware that things like Azure App Service can save a lot of time in app deployment, at an additional cost.

QUIZ QUESTION
Which of the following are benefits of Platform as a Service (PaaS) over Infrastructure as a Service (IaaS)?

(Select all that apply.)

Ease of Configuration


Less Expensive

Minimal Development


Scalability

SUBMIT
Resource Groups
Play Video
QUIZ QUESTION
Which of the following is FALSE?


Resource groups can contain many resources


Management groups can contain many subscriptions

One subscription can be in many management groups


Subscriptions can contain many resource groups

SUBMIT
Virtual Machines and Virtual Networks
Play Video
QUIZ QUESTION
Which of the following are configurable options for virtual machines?

(Select all that apply.)

CPU

Memory

Storage

Operating System


Brand of RAM

Region


Description
Resource Type
An emulation of a computer system.

Virtual Machine

A block of IP addresses which can be assigned. /24 by default

Virtual Network

A virtualized representation of a computer network interface that allows a virtual machine to communicate

Network Interface Card

A device that distributes network traffic over a number of servers

Load Balancer

A logical subdivision of an IP network.

Subnet

Other Resources You Should Know
Although we do not use storage accounts or databases in this course, they are items that we may be asked to deploy. So for the purposes of this course, all we need is to be aware of these resource types and know where to find information about them when we are asked to deploy them.

Storage Accounts and Blob Storage
Storage accounts are general purpose storage in Azure that provide a scalable object store. Storage accounts provide highly available, scalable, and secure storage for all kinds of objects. In Azure, storage services consist of:

Azure Blobs
Azure Files
Azure Queues
Azure Tables
Azure Disks
Azure Disks are storage volumes for virtual machines, and you'll normally only see them in that context. If you'd like to learn more, the other four types of storage accounts are detailed in the Azure documentation, but one important type of storage account you should be aware of is Blob Storage.

Blob Storage
Blob Storage is the general purpose storage solution in Azure. It's designed for storing and serving unstructured data such as images, text, or other files.

More detail can be found in the Blob Storage Documentation

SQL Servers
SQL servers are the most common type of database server, and Azure offers regular SQL databases as well as fully managed instances. You can also run SQL Server on an Azure virtual machine! SQL servers are a powerful way to store, serve, and manage structured data.

More detail can be found in the Azure SQL Documentation

-
Azure Infrastructure Fundamentals
Deploying Your First Resource
Replay
Mute
Loaded: 100.00%
Remaining Time -0:00
1xPlayback Rate
Captions
Picture-in-Picture

Fullscreen
QUIZ QUESTION
Just to make sure we have things straight before we move forward in our virtual machine configuration, which of the following are mandatory configuration items for a virtual machine?

(Select all that apply.)

Hint: Four of these items are necessary to deploy a virtual machine. We've only covered these items so far in our walkthrough above, but think about what Azure cannot assume for you.

VM Image


Disk Type

Region

Resource Group


Network Security Group

Virtual Machine Size

SUBMIT
Replay
Mute
93%
Loaded: 100.00%
Remaining Time -0:00
1xPlayback Rate
Captions
Picture-in-Picture

Fullscreen
Now it's your turn!
Using the Azure Portal, go in and set up a new Virtual Machine in a new Resource Group with a new Virtual Network. The nice thing about using the portal is that all of the required fields are put on a single page, and if you want to select existing resources, it will provide them in a nice drop-down. Of course, it might be hard to do this for say, 20 or 30 virtual machines, which is why later on, we'll deploy our infrastructure as code. You should deploy a virtual machine using Ubuntu 18.04-LTS and consider the VM size options. Then, using the Public IP that is assigned, SSH into your VM and poke around.

Don't forget to destroy the virtual machine when you're done!

Follow the instructions below to deploy your first resource in Azure

Task List

Log in to Azure


Click "Create a Resource"


Click on the icon for "Ubuntu 18.04-LTS"


Fill in the required fields


Follow the rest of the instructions in the wizard


Deploy your virtual machine!


(Optional) Log in to your virtual machine using SSH or RDP


Destroy your virtual machine

QUIZ QUESTION
How many resources, total, were deployed when you deployed your virtual machine?


One


Two


Six

Seven

SUBMIT
Microsoft Learn
Follow and complete the Microsoft Learn links below for additional training that will help you be more effective developing on Microsoft Azure, and help you prepare for the Microsoft Azure Developer Associate certification exam.

Monitor the health of your Azure virtual machine by collecting and analyzing diagnostic data
-
Azure Infrastructure Fundamentals
Intro to Virtual Networking
Virtual networking allows you to create software-defined networks to place virtual machines and network interface cards on. Some critical concepts in virtual networking include:

Ensuring non-overlapping address space for virtual networks
Planning ahead for subnet size
Having fewer large vNets with many subnets is better than many smaller vNets with similarly sized subnets
The Azure documentation on virtual networks is helpful, and also contains information on DNS, VNet peering, and more advanced virtual networking concepts.

-
Azure Infrastructure Fundamentals
Introduction to Load Balancing
Load balancing is a critical component of deploying high availability systems. Load Balancers can:

Balance internal and external traffic to virtual machines
Increase availability of virtual machines
Provide valuable metrics through Azure monitor
In the video, we mention the OSI model, which is a way of thinking about networking technology. Application gateways operate at a higher layer of the OSI model, so they are able to gain context about the application itself. Standard load balancers operate at a lower layer of the OSI model, so they have less context to make decisions. You won't need to know about the OSI model for this course but if you want to learn more about the OSI model, you can check out the Wikipedia page.

You can also write health probes to allow a Load Balancer to detect the status of the virtual machine at the endpoint.

-
Azure Infrastructure Fundamentals
Azure Monitor
Azure Monitor is a tool you can use to—as the name implies—monitor key metrics. It's also where log aggregation and service health are.

Our focus is going to be on optimizing virtual machines, but if you want to check out other features in more detail, you can have a look at the Azure Monitor Documentation.

We're most often concerned with CPU utilization, but Azure Monitor can also help with disk utilization. If you have an application that writes files to disk, you may fill up your OS disk quite quickly. In general, applications should try to write to some kind of external storage - either a blob storage or some other data disk.

For more information, check out the Azure documentation for an Introduction to Azure managed disks

-
Azure Infrastructure Fundamentals
Azure Active Directory
Azure Active Directory is Microsoft's cloud-based identity and access management solution. It is primarily used by IT admins to control access to Azure resources and provision users. Let's check it out!


Tenants are organization-level, and typically are best thought of as "one per company"—that is, everyone with an @microsoft.com email would have an @microsoft.com account in the active directory tenant.

One option for managing Azure Active Directory is to use Azure AD sync to ensure that your on-premises active directory is the same as the one in the cloud. This can allow us to unify everything under one identity.

App developers may also use Azure AD to implement single sign on, as described in the documentation.


Directories can have groups, which can be in other groups, each of which has numerous users. This allows inheritance of permissions. This is vital for permissions management and ensuring that permissions that are granted don't get "lost in the shuffle" by making management complicated.

The Service Principal requires and works through an app registration within the tenant. It is defined by a single application object, which provides access on behalf of the application, not a user. We will revisit this in future lessons, as it allows us to take advantage of the principle of least privilege.

Microsoft Learn
Follow and complete the Microsoft Learn links below for additional training that will help you be more effective developing on Microsoft Azure, and help you prepare for the Microsoft Azure Developer Associate certification exam.

Create Azure users and groups in Azure Active Directory
Authenticate apps to Azure services by using service principals and managed identities for Azure resources
-
Azure Infrastructure Fundamentals
Tour of Azure Active Directory
-
Azure Infrastructure Fundamentals
Azure Command Line Interface
Now you know the fundamentals of Azure infrastructure! But working in the portal can be really cumbersome, and so we want to explore using the official Azure Command-Line Interface (CLI) as well.

In this next video, I'll walk you through the same exercises we did before in the portal, but using the CLI. Then, you'll tackle two new tasks using the CLI.

Before getting started, ensure you have the Azure CLI installed and have logged into your Azure account by entering the command az login at your machine's terminal.


Note: For now we are exploring the portal and CLI, but in later lessons, we're going to also cover Terraform, which is an amazing tool for writing Infrastructure as Code.

PS C:\Users\chanhen> az group create --name udacity-cli-rg --location eastus
{
  "id": "/subscriptions/9f8c8075-22c6-437f-a041-2396efb4e277/resourceGroups/udacity-cli-rg",
  "location": "eastus",
  "managedBy": null,
  "name": "udacity-cli-rg",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null,
  "type": "Microsoft.Resources/resourceGroups"
}
PS C:\Users\chanhen> az vm create --resource-group udacity-cli-rg --name udacity-cli-vm --image UbuntuLTS --generate-ssh-keys --output json --verbose
SSH key files 'C:\Users\chanhen\.ssh\id_rsa' and 'C:\Users\chanhen\.ssh\id_rsa.pub' have been generated under ~/.ssh to allow SSH access to the VM. If using machines without permanent storage, back up your keys to a safe location.
It is recommended to use parameter "--public-ip-sku Standard" to create new VM with Standard public IP. Please note that the default public IP used for VM creation will be changed from Basic to Standard in the future.
{
  "fqdns": "",
  "id": "/subscriptions/9f8c8075-22c6-437f-a041-2396efb4e277/resourceGroups/udacity-cli-rg/providers/Microsoft.Compute/virtualMachines/udacity-cli-vm",
  "location": "eastus",
  "macAddress": "00-22-48-23-70-72",
  "powerState": "VM running",
  "privateIpAddress": "10.0.0.4",
  "publicIpAddress": "20.169.180.158",
  "resourceGroup": "udacity-cli-rg",
  "zones": ""
}
Command ran in 41.934 seconds (init: 1.441, invoke: 40.493)
PS C:\Users\chanhen> ssh 20.169.180.158
The authenticity of host '20.169.180.158 (20.169.180.158)' can't be established.
ECDSA key fingerprint is SHA256:fPPVgitwu21/ZpHy4wEw0gWQ8017HDPuEwFMR52/Nps.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '20.169.180.158' (ECDSA) to the list of known hosts.
Welcome to Ubuntu 18.04.6 LTS (GNU/Linux 5.4.0-1091-azure x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Sat Sep 24 04:11:03 UTC 2022

  System load:  0.2               Processes:           114
  Usage of /:   4.8% of 28.89GB   Users logged in:     0
  Memory usage: 5%                IP address for eth0: 10.0.0.4
  Swap usage:   0%

0 updates can be applied immediately.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

chanhen@udacity-cli-vm:~$ ifconfig
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.0.0.4  netmask 255.255.255.0  broadcast 10.0.0.255
        inet6 fe80::222:48ff:fe23:7072  prefixlen 64  scopeid 0x20<link>
        ether 00:22:48:23:70:72  txqueuelen 1000  (Ethernet)
        RX packets 1926  bytes 1962560 (1.9 MB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 971  bytes 248448 (248.4 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 5920  bytes 440686 (440.6 KB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 5920  bytes 440686 (440.6 KB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

chanhen@udacity-cli-vm:~$ logout
Connection to 20.169.180.158 closed.
PS C:\Users\chanhen> az vm show --name udacity-cli-vm --resource-group udacity-cli-rg
{
  "additionalCapabilities": null,
  "applicationProfile": null,
  "availabilitySet": null,
  "billingProfile": null,
  "capacityReservation": null,
  "diagnosticsProfile": null,
  "evictionPolicy": null,
  "extendedLocation": null,
  "extensionsTimeBudget": null,
  "hardwareProfile": {
    "vmSize": "Standard_DS1_v2",
    "vmSizeProperties": null
  },
  "host": null,
  "hostGroup": null,
  "id": "/subscriptions/9f8c8075-22c6-437f-a041-2396efb4e277/resourceGroups/udacity-cli-rg/providers/Microsoft.Compute/virtualMachines/udacity-cli-vm",
  "identity": null,
  "instanceView": null,
  "licenseType": null,
  "location": "eastus",
  "name": "udacity-cli-vm",
  "networkProfile": {
    "networkApiVersion": null,
    "networkInterfaceConfigurations": null,
    "networkInterfaces": [
      {
        "deleteOption": null,
        "id": "/subscriptions/9f8c8075-22c6-437f-a041-2396efb4e277/resourceGroups/udacity-cli-rg/providers/Microsoft.Network/networkInterfaces/udacity-cli-vmVMNic",
        "primary": null,
        "resourceGroup": "udacity-cli-rg"
      }
    ]
  },
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "chanhen",
    "allowExtensionOperations": true,
    "computerName": "udacity-cli-vm",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "enableVMAgentPlatformUpdates": false,
      "patchSettings": {
        "assessmentMode": "ImageDefault",
        "automaticByPlatformSettings": null,
        "patchMode": "ImageDefault"
      },
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDWSsyvCnCvtSVio+OGJYxXNi6k22zY4Mr2lT1nQiVrnfS75+zyZ8NdGtORL5gbuFw6Vudxuo01ytOQS/l1IKcyMvwH0QqKY4QSfS5p0bKOSlUqXV6qvfzt/RGyQw76qgIKLNhD1GPOcVCbwr8NC/4d7GizaFDWWX7BsJ20q+cxvG9OkisRIIkxo2WjefS3LAsZzXxqQdvUO1D/Fh4cLBEkUca9a3L1FixEdYPNblIaLYH/ZnwyAnTA6yJJg5KnITNcLqJ/jeagj0v07GJLLlL991ki+K8iNLuTDT8RaYb0CpWC384bs7fL7ISR9Q5S7xHOAQ99Sb2ALaJv4YJAYOvr",
            "path": "/home/chanhen/.ssh/authorized_keys"
          }
        ]
      }
    },
    "requireGuestProvisionSignal": true,
    "secrets": [],
    "windowsConfiguration": null
  },
  "plan": null,
  "platformFaultDomain": null,
  "priority": null,
  "provisioningState": "Succeeded",
  "proximityPlacementGroup": null,
  "resourceGroup": "udacity-cli-rg",
  "resources": null,
  "scheduledEventsProfile": null,
  "securityProfile": null,
  "storageProfile": {
    "dataDisks": [],
    "imageReference": {
      "communityGalleryImageId": null,
      "exactVersion": "18.04.202209210",
      "id": null,
      "offer": "UbuntuServer",
      "publisher": "Canonical",
      "sharedGalleryImageId": null,
      "sku": "18.04-LTS",
      "version": "latest"
    },
    "osDisk": {
      "caching": "ReadWrite",
      "createOption": "FromImage",
      "deleteOption": "Detach",
      "diffDiskSettings": null,
      "diskSizeGb": 30,
      "encryptionSettings": null,
      "image": null,
      "managedDisk": {
        "diskEncryptionSet": null,
        "id": "/subscriptions/9f8c8075-22c6-437f-a041-2396efb4e277/resourceGroups/udacity-cli-rg/providers/Microsoft.Compute/disks/udacity-cli-vm_disk1_f302ee6295594c7a9bb0e62255ad946d",
        "resourceGroup": "udacity-cli-rg",
        "securityProfile": null,
        "storageAccountType": "Premium_LRS"
      },
      "name": "udacity-cli-vm_disk1_f302ee6295594c7a9bb0e62255ad946d",
      "osType": "Linux",
      "vhd": null,
      "writeAcceleratorEnabled": null
    }
  },
  "tags": {},
  "timeCreated": "2022-09-24T04:09:32.628330+00:00",
  "type": "Microsoft.Compute/virtualMachines",
  "userData": null,
  "virtualMachineScaleSet": null,
  "vmId": "c71fd1ce-7932-49a3-9259-13a002fd0e32",
  "zones": null
}
PS C:\Users\chanhen> az vm delete
(--resource-group --name | --ids) are required
PS C:\Users\chanhen> az vm delete --resource-group udacity-cli-rg --name udacity-cli-vm
Are you sure you want to perform this operation? (y/n): y
PS C:\Users\chanhen>

-
Azure Infrastructure Fundamentals
Edge Case: Using the Portal vs. CLI
Most of your work will be in command line and Terraform, but portal can also be helpful in some situations. Specifically, the graphical and visual capabilities of the portal allow the user to:

See and understand hard-to-visualize resource states and other complex issues
Identify hard-to-see resource relationships
Additionally, we will use the portal to access the Azure Monitor and especially the Azure Security Center, which we will learn about soon!


-
Azure Infrastructure Fundamentals
Lesson Review
In this lesson we covered Azure Infrastructure Fundamentals. Specifically, we learned:

What the various IaaS resource types are that we can deploy.
We compared IaaS to PaaS and talked about the trade offs between cost and time.
How to use the in-portal wizard to deploy a virtual machine.
How to do virtual networking and load balancing, which will be critical for our project at the end of the course. In particular, we did a deep dive into load Balancers, looking at front and back end address pools and how to work with numerous VMs. This allows you to be able to provide high availability application delivery.
How to use Azure Monitor to optimize virtual machine performance and cost.
How to use Azure Active Directory for role-based access controls, users, and service principals.
How to use the Azure CLI (instead of the portal) to deploy resources.
When to use Azure portal vs. Azure CLI. Specifically, we saw that the portal has an advantage anytime we need graphical format, but this is at the expense of speed.
It's a great start! Now, we are ready to dive into security next!

=
Azure Security Best Practices
Tour of Azure Security Center
Microsoft Defender for Cloud is the core of security in Azure. It's a tool for security posture management and threat protection across your hybrid and multi-cloud workloads.

Defender for Cloud provides the tools needed to harden your resources, track your security posture, protect against cyber attacks, and streamline security management. Because it's natively integrated, deployment of Defender for Cloud is easy, providing you with simple auto provisioning to secure your resources by default.

Previously, Microsoft Defender for Cloud was called Azure Security Center, so if you’re searching for resources and see that term, some of that information may still be relevant but dated. There are three primary aspects of Defender for Cloud:

Continuous assessment - Generates a secure score showing the current status. Higher score infers a lower risk level.
Secure the resources - Provides security recommendations having a detailed remediation steps.
Defend the resources - Generates Security alerts for threats to the resources and workloads.
Three primary aspects of Defender for Cloud. Courtesy: [Microsoft docs](https://docs.microsoft.com/en-us/azure/defender-for-cloud/media/defender-for-cloud-introduction/defender-for-cloud-expanded-assess.png)
Three primary aspects of Defender for Cloud. Courtesy: Microsoft docs

Defender for Cloud's sample overview page. Courtesy: [Microsoft docs](https://docs.microsoft.com/en-us/azure/defender-for-cloud/media/get-started/overview.png#lightbox)
Defender for Cloud's sample overview page. Courtesy: Microsoft docs


-
Azure Security Best Practices
Intro to Azure Policy
Azure Policies are vital for the DevOps expert. In addition to providing technical security, policies also give us ways to provide consistency in enforcing industry and business standards and compliance. Let's have a look.

Some key points to remember about Azure Policies are:

They give us a way to manage costs by restricting specific resources.
Because of the policy-enabled secure architecture, we can determine the scope, source, and solution of problems more quickly.
Through policy-enabled configuration management, unexpected or even unwanted configuration changes can be prevented.
Custom Policy Definitions
Azure policies are written in JSON, and can be deployed in the portal or in the CLI. Policies have two modes: indexed, which evaluates only resource types that support tags and locations, and all, which evaluates resource groups, subscriptions, and all resource types. The rules themselves follow a simple if-then structure, where if the conditions in the policy rule are met, the effect specified in the "then" block occurs.

When in doubt, consult the Azure Policy definition structure in the Azure documentation.

Microsoft Learn
Follow and complete the Microsoft Learn links below for additional training that will help you be more effective developing on Microsoft Azure, and help you prepare for the Microsoft Azure Developer Associate certification exam.

Apply and monitor infrastructure standards with Azure Policy
-
Azure Security Best Practices
Creating a Custom Policy

-
-
-
-
-
-
-
-
