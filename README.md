# Azure-learning-dev
Repo for learning Azure and testing development
Azuredeploy.azcli contains a script for deploying this Environment

### Variables (Examples)
$rg="arm-vscode" 
$location="southcentralus"

### Deployment 
az group create --name $rg --location $location
az deployment group create --resource-group $rg --template-file azuredeploy.json --parameters azuredeploy.parameters.json

### Clean up
az group delete --name $rg

## Requirements
- azcli
- powershell
- Azure Subscription

## How to Run
1) Login to Azure through VSCode (Azure: Sign in to Azure Cloud)
2) Open up the azuredeploy.azcli file
3) Make modifications to any variables
4) Run the Powershell commands in order