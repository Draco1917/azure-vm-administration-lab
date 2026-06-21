# Azure Virtual Machine Administration Lab

## Overview

This project demonstrates the deployment and administration of a Windows Server 2022 virtual machine in Microsoft Azure. The environment includes virtual networking, security controls, public connectivity, IIS web server configuration, monitoring, and cost governance.

The goal of this project was to gain hands-on experience with core Azure administration concepts while building practical skills relevant to the AZ-104 certification and cloud engineering roles.

---

## Technologies Used

* Microsoft Azure
* Windows Server 2022
* Azure Virtual Machines
* Azure Virtual Networks
* Network Security Groups
* Public IP Addresses
* IIS Web Server
* Azure Monitor
* Azure Cost Management

---

## Architecture

![Architecture Diagram](images/architecture-diagram.png)

---

## Implementation

### Step 1 – Create Resource Group

Created a dedicated resource group named **rg-vm-lab** to logically organize and manage all resources associated with the project.

![Step 1](images/step1-resource-group.png)

---

### Step 2 – Configure Virtual Network

Configured a virtual network to provide private connectivity between Azure resources and establish the network foundation for the virtual machine environment.

![Step 2](images/step2-vnet.png)

![Step 2 Review](images/step2-vnet-review.png)

---

### Step 3 – Create Subnet

Created a subnet to provide IP addressing and separation for the Windows Server virtual machine.

![Step 3](images/step3-subnet.png)

---

### Step 4 – Create Network Security Group

Implemented network security controls using an Azure Network Security Group to manage inbound and outbound traffic.

![Step 4](images/step4-nsg.png)

---

### Step 5 – Configure Remote Desktop Access

Created an inbound rule allowing Remote Desktop Protocol traffic on TCP port 3389 to enable secure administrative access.

![Step 5](images/step5-rdp-rule.png)

---

### Step 6 – Create Public IP Address

Configured a public IP address to provide external connectivity to the virtual machine.

![Step 6](images/step6-public-ip.png)

---

### Step 7 – Deploy Windows Server 2022 Virtual Machine

Provisioned a Windows Server 2022 virtual machine and associated networking resources.

![VM Creation](images/step7-create-vm.png)

![VM Networking](images/step7-networking.png)

![Review and Create](images/step7-review.png)

---

### Step 8 – Verify Deployment

Verified successful deployment and confirmed that the virtual machine was operational.

![Step 8](images/step8-vm-overview.png)

---

### Step 9 – Connect to the Virtual Machine

Established administrative access to the server using Remote Desktop Protocol.

![Step 9](images/step9-rdp-connect.png)

---

### Step 10 – Install IIS

Installed Internet Information Services (IIS) to provide web server functionality.

![Step 10](images/step10-install-iis.png)

---

### Step 11 – Verify Local IIS Operation

Verified that the IIS default website was functioning correctly before enabling public access.

![Step 11](images/step11-iis-localhost.png)

---

### Step 12 – Configure HTTP Access

Created an inbound rule allowing HTTP traffic on TCP port 80. During testing, an additional Network Security Group created automatically by Azure was identified and configured appropriately to allow external access.

![Step 12](images/step12-http-rule.png)

---

### Step 13 – Verify Public Website Access

Verified successful public connectivity by accessing the IIS default page through the virtual machine's public IP address.

![Step 13](images/step13-iis-public.png)

---

### Step 14 – Configure Azure Monitor Alert

Implemented monitoring and alerting to improve operational awareness and resource visibility.

![Step 14](images/step14-monitor-alert.png)

---

### Step 15 – Configure Cost Management Budget

Created a monthly budget and spending alerts to demonstrate cost governance and prevent unexpected cloud costs.

![Step 15](images/step15-budget.png)

---

## Skills Demonstrated

* Azure Administration
* Windows Server 2022 Administration
* Azure Virtual Machines
* Virtual Networking
* Network Security Groups
* Public IP Configuration
* IIS Web Server Administration
* Azure Monitor
* Cost Management and Budgeting
* Troubleshooting and Problem Solving

---

## Lessons Learned

This project reinforced the importance of networking, security controls, monitoring, and cost governance when administering cloud infrastructure.

During testing, an additional Network Security Group created automatically by Azure was discovered and configured appropriately. This experience highlighted the importance of understanding Azure resource relationships and demonstrated practical troubleshooting techniques commonly encountered in cloud environments.

The project provided valuable hands-on experience with Windows Server administration and established a strong foundation for future Azure administration and cloud engineering projects.

---

## Project Outcome

The project successfully delivered a Windows Server 2022 virtual machine hosted in Microsoft Azure with secure networking, IIS web services, monitoring, and cost management capabilities.

This lab serves as a foundation for future Azure administration, identity, networking, and DevOps projects while continuing preparation for the AZ-104 certification.

---

## Live Portfolio

Portfolio Website:

(https://austinportfolio001.z13.web.core.windows.net/projects/azure/azure-vm-lab/index.html)

Main Portfolio Repository:

(https://github.com/Draco1917/azure-cloud-portfolio-platform)
