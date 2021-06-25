# Microservice App Structure and Management
**How to Open draw.io**
Go To [https://app.diagrams.net/]
Select the io File

**List of Environment/Repo:**
- Azure Env
- On Premise Env
- GitHub/BitBucket/Azure Repo
- Azure DevOps/Jenkins
- Selenium/Robot Framework For Test Automation
- ELK for Log & Login Management
- Zabbix For Service Management

**List of Components:**
1. Azure App Gateway
2. VM With Scale Set
3. Virtual Network
4. On Premise Virtual Network
5. Network Peering
6. DB With EndPoint
7. Network Security Group in Azure
8. Pipelines in Azure DevOps/Jenkins
9. Terraform Files for Infrastructure As A Code
10. Azure Key Vault for secure files

**Implementation:**
We Will Installed ELK Stack for Log and Login Management and Zabbix for Server/Service Monitoring
Both Will be Installed in On Premise Environment.

Terraform Files (Modular Wise / single tf file) will be Implemented for Infrastructure Deployment.

Infra Pipeline will be set In Azure DevOps. Here we will use Azure DevOps.

After All components deployed in Azure Env Then we will Go for Virtual Network Peering.

In Azure, Virtual Machine ScaleSet for VM scalaibilty
Database Server will be Implemented in Azure With End Point.

Application could be build through Jenkins or Azure DevOps.
- If we use Azure DevOps we could Deploy through Release Pipeline.
- If we use Jenkins we could Deploy writing a Jenkinsfile.

Test Automation script could be written in Robot Framework / Selenium For Sanity Testing.

We Will create indexes/index pattern in ELK and Discovery Rule in Zabbix to finish setUp.

**Access Services:**
We will use FrontEnd IP in Azure Application Gateway and User will use this IP to access the Application/Services.
In backend Pool of Azure Application Gateway, All Microservice VM IP will be added.



