# Azure Secure Blob Storage Lab
## Project Overview:
A hands-on Microsoft Azure lab demonstrating how to create and secure Blob Storage, use private access and temporary SAS tokens, apply Soft Delete features, perform proper resource cleanup, and review costs in Cost Management.
## Architecture
```
Resource Group: LAB-RG
|-- Storage Account: mlabstorages11
    |-- Container: labcontainer
        |-- Blob: prueba-azure.txt
```
## Lab Objectives
- Create an Azure Storage Account
- Create a Private Blob Container
- Upload a Blob
- Generate a SAS Token
- Test Secure access using SAS URL
- Enable Soft Delete for Blob Protection
- Review Costs using Azure Cost Management
## Tecnologies Used
- Microsoft Azure
- Azure Storage Account
- Azure Blob Storage
- Shared Access Signature
- Azure Soft Delete
- Azure Cost Management
## Implementation Steps
## 1. Create the Resource Group
- Resource Group: LAB-RG
- Region: East US
- Purpose: Organize all lab resources in a single logical container
## 2. Create the Storage Account
- Storage Account: mlabstorages11
- Region: East US
- Performance: Standard
- Redundancy: LRS
- Account Type: StorageV2
- Access Tier: Hot
## 3. Create the Blob Container
- Container Name: labcointainer
- Public Access Level: Private
- Purpose: Storage blobs securely without anonymous public access
## 4. Upload the Blob
- Blob Name: prueba-azure-txt
- Blob Type: Block Blob
- Upload Method: Azure Portal
- Purpose: Storage the test file inside the private container
## 5. Generate a SAS Token
- Permissions: Read
- Protocol: HTTPS only
- Expiration: Temporary
- Purpose: Provide temporary secure access to the blob without exposing the storage account key
## 6. Test Secure Access
- Test Method: Open the SAS URL in a web browser
- Result: Blob accessed successfully using the SAS URL
- Security Validation: Anonymous access remained disabled
## 7. Configure Soft Delete
- Soft Delete: Enabled
- Retention Period: 7 days
- Purpose: Protect delete blobs from accidental data loss
## 8. Clean Up Resourses
- Delete Blob: prueba-azure.txt
- Delete Container: labcontainer
- Delete Storage Account: m-labstorage11
- Final Verification: LAB-RG contains 0 Resources
- Purpose: Avoid unnesessary Azure cost after completing the lab
## Key Learnings
- Learned to configure a budget alert to prevent unexpected costs
- Learned to organize Azure resources using Resource Groups
- Learned to create and configure an Azure Storage Account
- Learned to upload and secure blobs
- Learned to generate and use a SAS token for secure temporary access
- Learned to use Soft Delete to protect data from accidental deletion
