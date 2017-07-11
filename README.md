# Introduction to the **Azure App Service** (PaaS)

This workshop is designed to help you get familiar with some of the key features and capabilities of the Azure App Service, support tooling for building, hosting and monitoring modern applications.

App Service is a platform-as-a-service (PaaS) offering of Microsoft Azure. It allows you to create web and mobile apps for any platform or device. Integrate your apps with SaaS solutions, connect with on-premises applications, and automate your business processes. Azure runs your apps on fully managed virtual machines (VMs), with your choice of shared VM resources or dedicated VMs.

## [Lab 1 - Provisioning an Azure App Service](/lab1)

* Create an App Service Environment (ASE)
* Create an Azure Web App in the ASE

## Lab 2 - Azure App Service Deployment

* Create a staging slot
* Deploy from a GitHub repo (continuous delivery)
* Add an App Authentication/Authorization with Azure AD

## Lab 3 - Visual Studio Team Services CI/CD pipeline

* Create a Visual Studio Team Services project
* Import the GitHub repository
* Switch the local git master to VSTS
* Reconnect the Web App deployment to VSTS
* Create a build plan
* Perform a slot swap

## [Lab 4 - Setting up App Insights (AI) in VS Code](/lab4)

In this lab we will walk through adding an  Application Insights framework to a sample  Node.js/Express project. We will showcase the AI/VS Code integration that will enable more agile development process by providing real-time AI telemetry (CodeLens) feedback in the IDE and the portal.