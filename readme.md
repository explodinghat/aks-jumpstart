From: https://gmusumeci.medium.com/deploying-terraform-infrastructure-using-azure-devops-pipelines-step-by-step-d58b68fc666d

Pre-reqs:

- Azure Subscription: If we don’t have an Azure subscription, we can create a free account at https://azure.microsoft.com before we start.
- Azure Service Principal: is an identity used to authenticate to Azure. Below are the instructions to create one.
- Azure Remote Backend for Terraform: we will store our Terraform state file in a remote backend location. We will need a Resource Group, Azure Storage Account and a Container. We can create the Remote Backend in advance (more info below) or let the Release Pipeline create one. (see https://github.com/explodinghat/tf-remotestate-jumpstart for walkthrough on this)
- Azure DevOps Account: we need an Azure DevOps account because is a separate service from the Azure cloud.
