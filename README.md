# Secure-2--Tier-Web-Application
This project focuses on designing and deploying a secure two-tier web application infrastructure using Microsoft Azure.

## 1. Project Overview
The architecture separates the frontend web tier from the backend database tier to improve security, network isolation, and infrastructure management.

The web tier handles incoming application traffic, while the database tier operates within a private network environment.

The project demonstrates practical cloud infrastructure engineering, Linux administration, network configuration, access control, and security implementation.

## 2. Project Objectives

- Design a two-tier cloud infrastructure architecture.
- Deploy and configure Azure Virtual Machines.
- Create and configure an Azure Virtual Network.
- Implement public and private network segmentation.
- Configure secure communication between infrastructure components.
- Apply Network Security Groups to control network traffic.
- Configure secure remote administration using SSH.
- Validate network connectivity and security configurations.
- Document implementation and testing evidence.

## 3. Technologies and Tools

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud infrastructure |
| Azure Virtual Machines | Compute resources |
| Azure Virtual Network | Network connectivity |
| Azure Subnets | Network segmentation |
| Network Security Groups | Traffic filtering |
| Ubuntu Server | Linux operating system |
| SSH | Secure remote administration |
| Azure Portal | Infrastructure management |
| GitLab | Version control and project documentation |

## 4. Architecture Overview

The infrastructure consists of two primary tiers:

**Web Tier**
- Hosts the frontend web service.
- Handles incoming application traffic.
- Communicates with the backend through the private network.

**Database Tier**
- Hosts backend database services.
- Isolated from direct public internet access.
- Accepts only authorized internal traffic.

<text>Architecture diagram placeholder: Add your completed network topology here.</text>

## 5. Implementation and Configuration

### Phase 1: Azure Infrastructure and Network Design

**Objective:** Establish the foundational cloud infrastructure.

Tasks:
1. Create an Azure Resource Group.
2. Create an Azure Virtual Network.
3. Define the virtual network address space.
4. Create separate subnets for the web and database tiers.
5. Review the network topology and IP allocation.

**Screenshots 
- Resource Group overview.
  <img width="1695" height="1024" alt="Screenshot 2026-11-11 at 11 49 05 AM" src="https://github.com/user-attachments/assets/a87a6a55-4fc8-4259-99e9-e14b9377d6bb" />
- Virtual Network configuration.
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 11 55 30 AM" src="https://github.com/user-attachments/assets/c77a4092-d958-4fa6-9d39-8f89e69c89c0" />
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 11 56 04 AM" src="https://github.com/user-attachments/assets/21792fc0-414e-405f-84ca-87495264bc2b" />


### Phase 2: Web Server Deployment

**Objective:** Deploy the frontend infrastructure.

Tasks:
1. Create an Azure Linux Virtual Machine.
2. Configure the operating system and VM size.
3. Connect the VM to the web subnet.
4. Configure the required network access.
5. Establish SSH connectivity.
6. Verify that the server is operational.

**Screenshots to add:**
- Virtual Machine creation settings.
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 03 19 PM" src="https://github.com/user-attachments/assets/e0b805c3-8bbb-4385-998c-9d1ee7710c31" />
- Web VM overview.
<img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 04 20 PM" src="https://github.com/user-attachments/assets/62dbbd3b-8a15-425c-9346-37a1cbb5e550" />

### Phase 3: Database Server Deployment

**Objective:** Deploy the backend infrastructure within a private network environment.

Tasks:
1. Create a second Azure Linux Virtual Machine.
2. Configure its operating system and VM size.
3. Connect the VM to the database subnet.
4. Configure private network addressing.
5. Restrict direct external access.
6. Verify the VM's network configuration.

**Screenshots to add:**
- Database VM deployment settings.
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 09 48 PM" src="https://github.com/user-attachments/assets/d857c551-24fd-4078-85ef-c0bb30c1abed" />
- Database VM overview.
<img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 14 46 PM" src="https://github.com/user-attachments/assets/611517d9-5c36-4bea-ad2d-829541b196b5" />

### Phase 4: Network Security Configuration

**Objective:** Implement network access restrictions between the application tiers.

Tasks:
1. Review the Network Security Groups associated with each tier.
2. Configure inbound traffic restrictions.
3. Restrict database access to authorized internal sources.
4. Review SSH and application access rules.
5. Verify rule priorities and traffic direction.
6. Confirm that backend infrastructure is not directly exposed to the internet.

**Screenshots to add:**
- Web subnet security rules.
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 58 59 PM" src="https://github.com/user-attachments/assets/ceffa7de-340c-4f5a-8778-4e4779531d8e" />
- Database subnet security rules.
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 55 09 PM" src="https://github.com/user-attachments/assets/e13692ea-57c3-4bb9-b586-1ac7008f0efa" />

### Phase 5: Private Connectivity and Validation

**Objective:** Verify communication between the web and database tiers.

Tasks:
1. Connect to the web server using SSH.
2. Identify the private IP address of the database server.
3. Test connectivity between the two virtual machines.
4. Validate the network path.
5. Review firewall and NSG configurations if connectivity fails.
6. Record the results of connectivity testing.

**Screenshots:**
- SSH session on the web server.
  <img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 40 02 PM" src="https://github.com/user-attachments/assets/95558d2e-8a09-415d-af36-e905d0b65f9b" />

- Successful communication between tiers.
<img width="1710" height="1107" alt="Screenshot 2026-11-11 at 12 41 52 PM" src="https://github.com/user-attachments/assets/c0d5f462-30db-4260-89ca-5e5b13ee10d4" />


```
## 7. Expected Learning Outcomes

Upon completion, this project will demonstrate practical understanding of:

- Azure cloud infrastructure deployment.
- Linux virtual machine administration.
- Virtual network and subnet configuration.
- Public and private IP addressing.
- Network Security Group administration.
- Secure remote server access.
- Network segmentation.
- Infrastructure security and troubleshooting.
- Cloud architecture documentation.

## 9. Author

**Nadia Kroduah**

Cloud and Network Engineering | Azure Infrastructure | Linux Administration

