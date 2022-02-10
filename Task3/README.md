# Microservice App Structure and Management

**List of Environment/Repo:**
- Azure Env
- On Premise Env
- GitHub/Azure Repo
- Azure DevOps
- Selenium/Robot Framework For Test Automation
- Zabbix For Service Monitoring

**List of Components:**
1. Azure App Gateway
2. Azure Kubernetes
3. Virtual Network
4. On Premise Virtual Network
5. Network Peering
6. SQL DB With EndPoint
7. Network Security Group in Azure
8. Pipelines in Azure DevOps/Jenkins
9. Terraform Files for Infrastructure As A Code
10. Azure Key Vault for secure files
11. Azure VPN Gateway

**Implementation:**
We Will Installed Zabbix for Server/Service Monitoring.

Terraform Files (Modular Wise / single tf file) will be Implemented for Infrastructure Deployment.

Infra Pipeline will be set In Azure DevOps. Here we will use Azure DevOps.

After All components deployed in Azure Env Then we will Go for Virtual Network Peering.

In Azure, Azure Kubernetes will be implemented and Ingress Controller will be installed within AKS
Database Server will be Implemented in Azure With End Point.

Application could be build through Azure DevOps.
- If we use Azure DevOps we could Deploy through Release Pipeline.

Test Automation script could be written in Robot Framework / Selenium For Sanity Testing.

We Will create indexes/index pattern in ELK and Discovery Rule in Zabbix to finish setUp.

**Access Services:**
We will use FrontEnd IP in Azure Application Gateway and User will use this IP to access the Application/Services.
In backend Pool of Azure Application Gateway, All Microservice VM IP will be added.



