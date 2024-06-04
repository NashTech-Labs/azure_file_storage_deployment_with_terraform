# Azure File Storage Deployment with Terraform

This repository contains a Terraform configuration automates the deployment of Azure file storage resources, including storage accounts, file shares, and file uploads. By defining infrastructure as code, you can easily provision and manage Azure file storage resources in a repeatable and consistent manner.

## Prerequisites

- **Azure Subscription:** Ensure you have an active Azure subscription.
- **Terraform Installed:** Terraform installed on your local machine.

## Configuration Files

- main.tf: Contains the main Terraform configuration for creating Azure file storage resources, including storage accounts, file shares, and file uploads.

## Terraform Resources

- azurerm_resource_group: Data source to retrieve existing resource group details.
- azurerm_storage_account: Creates a storage account within the specified resource group.
- azurerm_storage_share: Creates a file share within the storage account.
- azurerm_storage_share_file: Uploads a file to the file share.

## Customization

- Adjust the variables in main.tf according to your specific requirements, such as storage account name, resource group, and file upload source.

## Usage

1. Clone this repository to your local machine.
2. Navigate to the directory containing the Terraform code.
3. Initialize the Terraform directory using the command `terraform init`.
4. Create an execution plan with `terraform plan`.
5. Apply the plan with `terraform apply`. You will be prompted to confirm the action by typing `yes`.

Remember to run `terraform destroy` when you no longer require these resources to avoid unnecessary AWS charges.