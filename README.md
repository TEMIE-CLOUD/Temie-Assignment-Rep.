# Temie-Assignment-Rep.
CLOUD ENGINEER
Hosting a Simple Web Application on Azure**  

*I. Introduction* 

To host a simple web application, I would use Azure App Service. It is a managed platform that simplifies building, deploying, and scaling web applications. 

*II. Cost Considerations* 

To save money, I would: - Start with the free tier of Azure App Service. 
- Store static content in Azure Blob Storage. 
- Automatically adjust resources based on demand using autoscaling. 
- Use Azure’s cost management tools to monitor and reduce expenses. 

*III. Scalability Considerations* 

To ensure the web application can handle an increasing number of users, I would: 
- Design a scalable architecture with Azure App Service plans. 
- Enable autoscaling to adjust resources based on demand. 
- Use Azure’s content delivery network (CDN) to globally distribute content. 
- ⁠- Implement traffic load balancing across multiple instances. 

*IV. Security Considerations* 

To secure the web application, I would:
- Use Azure Active Directory (AAD) for user authentication and authorization. 
- Encrypt data both in transit and at rest. 
- ⁠- Implement network security groups (NSGs) and Azure Firewall to control access. 
- ⁠- Monitor security incidents using Azure’s monitoring and logging tools.

V. Conclusion

In summary, my approach to hosting a simple web application on azure involves:

* Using Azure App Service for a managed platform 
* Saving cost with cost-effective services and auto scaling 
* Scaling up with a scalable architecture and load balancing 
* Security my app with AAD, encryption and monitoring.
* ![JPEG image 2](https://github.com/user-attachments/assets/d5b16c13-a63c-4170-a607-c13427c89417)
![JPEG image](https://github.com/user-attachments/assets/3c493886-303b-481d-a924-7a4734633c1e)
![JPEG image 3](https://github.com/user-attachments/assets/8dd7da26-2572-4e39-acd2-09344bc1ca1d)
![JPEG image 4 (1)](https://github.com/user-attachments/assets/07c06bd4-8b1b-4ec0-9a02-df9f0a569029)

Assignment 3:
 Configuring a Virtual Network with Subnets and Azure Storage Setup
Introduction:
This assignment focuses on deploying and configuring a secure virtual network with two subnets in Microsoft Azure. The goal is to ensure that the virtual machines (VMs) deployed in different subnets can communicate with each other. Additionally, it involves setting up an Azure Storage Account, creating a blob container, and demonstrating file upload and download operations.
This guide provides a step-by-step explanation of both the scenario-based objectives and practical tasks required to complete the assignment, with details on the configuration and verification process.
Virtual Network Configuration
A Virtual Network (VNet) was created with the following details:
•	VNet Name: MyVirtualNetwork
•	Address Space: 10.0.0.0/16
•	Region: East US
•	Resource Group: RG.Ass3
Subnet Configurations
Two subnets were created within the Virtual Network:
•	Subnet1: 10.0.1.0/24, named Subnet1
•	Subnet2: 10.0.2.0/24, named Subnet2
These subnets will host the virtual machines, enabling communication between them within the same virtual network.
VM Deployments
Two Virtual Machines (VMs) were deployed, one in each subnet:
•	VM1:
o	Name: vm01
o	Subnet: Subnet1
o	Private IP Address: 10.0.1.4

•	VM2:
o	Name: newvm02
o	Subnet: Subnet2
o	Private IP Address: 10.0.2.5
Communication Verification
In order to verify communication between the two VMs, an inbound rule was added to the Windows Defender Firewall on each VM, allowing ICMPv4 (ping) traffic.
•	Ping Tests:
o	Ping tests were conducted between VM1 and VM2 using their private IP addresses.
o	The tests were successful, confirming that the VMs in different subnets could communicate effectively.

Azure Storage Account Configuration
An Azure Storage Account was set up to demonstrate file management operations. The details of the storage account configuration are as follows:
•	Storage Account Name: storageass03t
•	Region: East US
•	Replication Type: Locally Redundant Storage (LRS)
Blob Container Creation
A blob container was created within the storage account to store files:
•	Blob Container Name: newcontainer3
File Upload/Download
A file transfer operation was successfully demonstrated:
•	File Uploaded: download (3) jjif
•	The file was uploaded to the blob container newcontainer3 and subsequently downloaded to verify successful file transfer between local storage and the Azure blob container.





Conclusion
In this assignment, I configured a virtual network with two subnets, deployed VMs into each subnet, ensured communication between the VMs, and set up an Azure Storage Account. A blob container was created, and file upload/download operations were successfully tested, showcasing the fundamental aspects of Azure networking and storage solutions.

References
1.	Microsoft Azure. (n.d.). Virtual Network documentation. Retrieved from https://learn.microsoft.com/en-us/azure/virtual-network/
2.	Microsoft Azure. (n.d.). Azure Virtual Machines documentation. Retrieved from https://learn.microsoft.com/en-us/azure/virtual-machines/
3.	Microsoft Azure. (n.d.). Network security overview. Retrieved from https://learn.microsoft.com/en-us/azure/virtual-network/security-overview
4.	Microsoft Windows. (n.d.). Create an inbound ICMPv4 rule in Windows Firewall. Retrieved from https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-firewall/create-inbound-icmpv4
5.	Microsoft Azure. (n.d.). Azure Storage documentation. Retrieved from https://learn.microsoft.com/en-us/azure/storage/
6.	Microsoft Azure. (n.d.). Azure Blob Storage overview. Retrieved from https://learn.microsoft.com/en-us/azure/storage/blobs/
