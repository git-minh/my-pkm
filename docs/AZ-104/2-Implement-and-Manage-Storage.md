# Section 2: Implement and Manage Storage (15-20%)

## 1. Secure Storage

### Configure Network Access to Storage Accounts
- **Firewalls and Virtual Networks**:
  - Restrict network access using firewall rules
  - Configure service endpoints
  - Set up private endpoints
  - Allow trusted Azure services
- **IP Address Rules**:
  - Define allowed IP ranges
  - Configure exceptions for Azure services

### Manage Access Keys and Shared Access Signatures (SAS)
- **Access Keys**:
  - View and regenerate storage account keys
  - Implement key rotation
  - Secure key storage
- **Shared Access Signatures (SAS)**:
  - Types:
    - Account SAS
    - Service SAS
    - User Delegation SAS
  - Best Practices:
    - Limited permissions
    - Short expiration times
    - IP restrictions

### Implement Azure AD Authentication for Storage
- **Azure AD Integration**:
  - Enable Azure AD authentication
  - Configure role assignments
  - Use managed identities
- **Access Control Model**:
  - RBAC roles for storage
  - Built-in roles vs custom roles

### Configure Azure Storage Firewalls and Virtual Networks
- **Firewall Rules**:
  - Default deny all access
  - Configure exceptions
  - Monitor access attempts
- **Virtual Network Service Endpoints**:
  - Enable service endpoints
  - Configure network rules
  - Understand security benefits

## 2. Manage Storage Accounts

### Create and Configure Storage Accounts
- **Storage Account Types**:
  - General-purpose v2 (GPv2)
  - Premium storage
  - BlockBlobStorage
  - FileStorage
- **Performance Tiers**:
  - Standard
  - Premium
- **Replication Options**:
  - Locally Redundant Storage (LRS)
  - Zone-Redundant Storage (ZRS)
  - Geo-Redundant Storage (GRS)
  - Read-Access Geo-Redundant Storage (RA-GRS)
- **Access Tiers**:
  - Hot
  - Cool
  - Archive

### Generate and Manage SAS Tokens
- **Token Generation**:
  - Azure Portal
  - Azure Storage Explorer
  - PowerShell/CLI
- **Token Management**:
  - Monitor usage
  - Revoke access
  - Update permissions

### Implement Azure Storage Replication
- **Replication Types**:
  - Synchronous vs asynchronous
  - Regional vs geo-replication
- **Failover Process**:
  - Manual failover
  - Failback procedures
  - Testing failover

### Manage Storage Account Keys and Policies
- **Key Management**:
  - Regular rotation
  - Azure Key Vault integration
  - Access key policies
- **Storage Policies**:
  - Lifecycle management
  - Retention policies
  - Immutable storage

## 3. Configure Azure Files and Blob Storage

### Create and Configure Azure File Shares
- **File Share Setup**:
  - Create file shares
  - Set quotas
  - Configure permissions
- **Access Methods**:
  - SMB protocol
  - Azure Files sync
  - Mount points
- **Authentication**:
  - AD DS authentication
  - Azure AD authentication
  - Key-based auth

### Configure Azure Blob Storage
- **Blob Types**:
  - Block blobs
  - Append blobs
  - Page blobs
- **Container Management**:
  - Create containers
  - Set access levels
  - Configure metadata
- **Blob Lifecycle**:
  - Lifecycle management rules
  - Automatic tiering
  - Deletion policies

### Implement Azure Data Lake Storage Gen2
- **Features**:
  - Hierarchical namespace
  - ACL support
  - Performance optimization
- **Security**:
  - RBAC integration
  - ACL configuration
  - Encryption settings

### Manage Data by Using Azure Storage Explorer
- **Storage Explorer Features**:
  - Browse resources
  - Upload/download data
  - Manage permissions
  - Generate SAS tokens

## Best Practices and Considerations

1. **Security**:
   - Enable encryption at rest
   - Use private endpoints where possible
   - Implement least privilege access
   - Regular security audits

2. **Performance**:
   - Choose appropriate storage tiers
   - Monitor performance metrics
   - Optimize access patterns
   - Use CDN for frequently accessed content

3. **Cost Management**:
   - Implement lifecycle management
   - Monitor storage metrics
   - Use appropriate replication options
   - Regular cleanup of unused resources

## Common PowerShell and Azure CLI Commands

```powershell
# Create a storage account
New-AzStorageAccount -ResourceGroupName "ResourceGroup1" `
                     -Name "storageaccount1" `
                     -Location "eastus" `
                     -SkuName "Standard_LRS"

# Generate SAS token
$sasToken = New-AzStorageAccountSASToken -Service Blob,File,Table,Queue `
                                        -ResourceType Service,Container,Object `
                                        -Permission "racwdlup"

# Create file share
New-AzRmStorageShare -ResourceGroupName "ResourceGroup1" `
                     -StorageAccountName "storageaccount1" `
                     -Name "share1" `
                     -QuotaGiB 100
```

```bash
# Create a storage account
az storage account create --name storageaccount1 \
                         --resource-group ResourceGroup1 \
                         --location eastus \
                         --sku Standard_LRS

# Create a container
az storage container create --name container1 \
                           --account-name storageaccount1

# Create file share
az storage share create --name share1 \
                        --account-name storageaccount1 \
                        --quota 100
```

## Monitoring and Troubleshooting

1. **Monitoring Tools**:
   - Azure Monitor
   - Storage Analytics
   - Azure Storage Explorer
   - Activity logs

2. **Common Issues**:
   - Access denied errors
   - Network connectivity
   - Performance bottlenecks
   - Replication delays

3. **Troubleshooting Steps**:
   - Check access keys and SAS tokens
   - Verify network rules
   - Review storage metrics
   - Check service health