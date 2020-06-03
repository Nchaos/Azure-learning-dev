# Azure-learning-dev
Repo for learning Azure and testing development

### Variables
$rg="arm-vscode"
$location="southcentralus"

### Deployment 
az group create --name $rg --location $location
az deployment group create --resource-group $rg --template-file azuredeploy.json --parameters azuredeploy.parameters.json

### Clean up
az group delete --name $rg