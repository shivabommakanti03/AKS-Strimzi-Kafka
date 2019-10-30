## Deploying Kafka using Strimzi operator on AKS using Azure Devops

## Pre-Requisites:
  1. Active Azure subscription
  2. Azure-CLI installed or access to Azure portal


## Azure-CLI Steps: Ref [https://docs.microsoft.com/en-us/azure/aks/tutorial-kubernetes-deploy-cluster].

  1. Create a resource group for your AKS to use it `az group create --name <Name of Your ResourceGroup> --location <Location>`
  2. Now, Install your Kubernetes cluster with mentioning how many nodes you want and specifying the version you want to use. `az aks create --resource-group <Your ResourceGroup> --name <Kubernetes-Cluster Name> --node-count <Number> --kubernetes-version <Version>`
  3. Install Kubernetes CLI on your local so you can connect to your cluster `az aks install-cli`
  

## Creating your Azure Devops Release pipeline.

  1. Navigate to your Azure Devops portal [https://dev.azure.com] and create new project for the release.
  2. Navigate to Repos on left panel and click on Repos and click on import repo and import repo.
  
