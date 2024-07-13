# Azure-week7-Assignment



Steps to Complete the Assignment
1. Observing Assigned Subscriptions
Observe Subscriptions:
I logged into the Azure portal and navigated to the "Subscriptions" section.
I reviewed the details of my assigned subscriptions, including subscription ID, name, and billing information.

2. Azure Entra ID Management
Observe or Create Azure Entra ID:
I observed the existing Azure Entra ID in my personal Azure account. If not available, I created a new Azure Entra ID.
Create Test Users and Groups:
I navigated to the Azure Entra ID section and created test users and groups for further testing.

3. Role-Based Access Control (RBAC)
Assign RBAC Role to User:
I assigned an RBAC role (e.g., Contributor) to a test user and verified the permissions by logging in as the user.
Create and Assign Custom Role:
I created a custom role with specific permissions and assigned it to a test user.
I tested the custom role by logging in as the user and verifying the permissions.

4. Creating VM and VNet Using Azure CLI
Install Azure CLI:
I installed Azure CLI on my local machine following the instructions from the official documentation.
Create VM and VNet:
Using Azure CLI, I created a Virtual Network (VNet) and a Virtual Machine (VM). Commands used included:

az network vnet create --name MyVnet --resource-group MyResourceGroup --subnet-name MySubnet
az vm create --resource-group MyResourceGroup --name MyVM --image UbuntuLTS --vnet-name MyVnet --subnet MySubnet --admin-username azureuser --generate-ssh-keys

6. Creating and Assigning Policies
Create and Assign Policy at Subscription Level:
I created a policy definition and assigned it to my subscription to enforce resource management rules.
I tested the policy by creating resources and verifying compliance.

7. Managing Azure Key Vault
Create an Azure Key Vault:

I created an Azure Key Vault using the Azure portal or CLI.
I stored secrets in the Key Vault.
Configure Access Policies for Key Vault:

I configured access policies to allow specific users or applications to manage keys and secrets.
I retrieved a secret using Azure CLI:

az keyvault secret show --name MySecret --vault-name MyKeyVault

8. Creating a VM Using PowerShell
Install Azure PowerShell:
I installed Azure PowerShell module on my local machine following the official documentation.
Create VM Using PowerShell:
I created a VM using PowerShell with commands such as:

New-AzVm -ResourceGroupName "MyResourceGroup" -Name "MyVM" -Image "UbuntuLTS" -Location "EastUS" -VirtualNetworkName "MyVnet" -SubnetName "MySubnet" -SecurityGroupName "MyNSG" -PublicIpAddressName "MyPublicIp" -OpenPorts 22,80

Conclusion
By following the above steps, I successfully managed Azure subscriptions, created and managed Azure Entra ID users and groups, assigned RBAC roles, created custom roles, managed VMs and VNets using CLI and PowerShell, created and assigned policies, and managed secrets in Azure Key Vault. This assignment provided a comprehensive understanding of Azure's management and security features.

