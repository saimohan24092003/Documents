# SAP BTP (Business Technology Platform)

SAP BTP is a cloud based Paas that Integrates tools for application development, data management, analytics, and automation.

## SAP BTP Topography:
![SAP BTP Topography](https://github.com/saimohan24092003/Documents/blob/4f8494d61ecfc7e533bb984bbcce8ed8382797b5/assets/sap-topography.svg)
End User can use browser/mobile app to access the BTP cloud app. 

Main BTP cloud Box (Centre) – SAP Integration Suite

CPI (Cloud Platform Integration) – Connects different system automatically. (e.g., It will connect SAP System like SAP BTP, SAP S/4 HANA, SuccessFactors with non-SAP systems like Salesforce, Workday).  
API Management – Control app APIs securely.  
SAP Event Mesh – Shares real-time events (data) between apps.

## SAP Extension and Automation

Here we can build and automate the custom app on top of SAP Systems without changing the core code.

Process Automation – No-code bots/workflows for repetitive task  
Apps (App development) – Build custom business app using low-code and deploy that to CF (Cloud Foundry), ABAP (SAP Style), Kyma (Microservice).  
Work Zone – It’s like personlaized Dashboard – everyone see their own task in one dashboard.  

(Manager: Sales KPIs + Team approvals  
  Worker:  Shift tasks + Inventory check  
  IT:      System alerts + New tickets)

## Data and Analytics - Stores and analyses data

SAP Data Warehouse Cloud – Clean and reports big data.  
SAP HANA Cloud – Super fast DB (Database)

## Foundation

Alert Notification – Sends warning (email/SMS)  
Feature Toggle – Turns app features on/off safely  
Transport – Moves code between test/production

## Connectivity (Bottom)

Connectivity Service – Manages secure links between BTP and outside system.  
Destination Service – Stores connection details (like address/password) for app to use.  
Identification Authentication Service (IAS) – Single login (like SSO) for users/apps.  
Cloud Connectors – Safe tunnel from BTP to On-premises server 

## External Cloud (Top)

Other public clouds (AWS/Azure) connect to BTP

## Private Cloud/On-Premise (Right Side)

Company's internal S/4HANA systems behind firewall. Cloud Connector links BTP to internal systems.
