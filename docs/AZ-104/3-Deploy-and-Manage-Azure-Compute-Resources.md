# Section 3: Deploy and Manage Azure Compute Resources (20-25%)

## 1. Configure Virtual Machines for High Availability and Scalability

### Deploy and Configure Scale Sets
- **Azure Virtual Machine Scale Sets (VMSS)**:
  - Purpose and benefits
  - Automatic scaling capabilities
  - Load balancing integration
- **Scaling Options**:
  - Manual scaling
  - Automatic scaling based on metrics
  - Schedule-based scaling
- **Configuration**:
  - Instance count limits
  - Scaling policies
  - Health monitoring

### Configure Azure Disk Encryption
- **Encryption Types**:
  - Azure Disk Encryption (ADE)
  - Server-Side Encryption (SSE)
- **Key Management**:
  - Azure Key Vault integration
  - Key encryption key (KEK)
  - BitLocker for Windows
  - DM-Crypt for Linux

### Implement Availability Sets and Zones
- **Availability Sets**:
  - Fault domains
  - Update domains
  - Configuration best practices
- **Availability Zones**:
  - Cross-zone deployment
  - Zone-redundant services
  - Disaster recovery planning

### Configure VM Size and Scaling
- **VM Sizes**:
  - General purpose
  - Compute optimized
  - Memory optimized
  - Storage optimized
  - GPU
- **Scaling Considerations**:
  - Vertical scaling (resize)
  - Horizontal scaling
  - Auto-scaling rules

## 2. Automate Deployment and Configuration of VMs

### Modify Azure Resource Manager (ARM) Templates
- **Template Structure**:
  - Parameters
  - Variables
  - Resources
  - Outputs
- **Template Functions**:
  - String functions
  - Array functions
  - Deployment functions
- **Best Practices**:
  - Parameterization
  - Linked templates
  - Template validation

### Automate Configuration Management
- **Desired State Configuration (DSC)**:
  - Configuration scripts
  - Node configuration
  - Pull servers
- **Custom Script Extensions**:
  - Script deployment
  - Parameter passing
  - Error handling
- **Configuration Management Tools**:
  - Azure Automation State Configuration
  - Chef, Puppet integration

### Deploy VMs using Azure CLI and PowerShell
- **Azure CLI**:
  - VM creation commands
  - Configuration options
  - Resource management
- **PowerShell**:
  - Azure PowerShell modules
  - VM deployment cmdlets
  - Automation scripts

## 3. Create and Configure Containers and Web Apps

### Create and Configure Azure App Service Plans
- **App Service Plans**:
  - Pricing tiers
  - Scaling options
  - Features by tier
- **Configuration**:
  - Resource allocation
  - Auto-scaling rules
  - Deployment slots

### Configure Networking for App Service
- **Network Integration**:
  - VNet integration
  - Hybrid connections
  - App Service Environment
- **Security**:
  - SSL/TLS configuration
  - IP restrictions
  - Authentication options

### Implement Azure Container Instances (ACI)
- **Container Deployment**:
  - Container groups
  - Resource allocation
  - Networking options
- **Configuration**:
  - Environment variables
  - Volume mounts
  - Container registry integration

### Configure Container Settings and Scaling
- **Container Settings**:
  - Image source
  - Resource limits
  - Restart policies
- **Scaling Options**:
  - Manual scaling
  - Auto-scaling
  - Container groups

## Best Practices and Considerations

1. **High Availability**:
   - Use availability sets or zones
   - Implement load balancing
   - Configure auto-scaling
   - Regular backup strategy

2. **Security**:
   - Enable disk encryption
   - Use managed identities
   - Implement network security
   - Regular security updates

3. **Performance**:
   - Choose appropriate VM sizes
   - Monitor performance metrics
   - Optimize application code
   - Use caching where appropriate

4. **Cost Management**:
   - Right-size VMs
   - Use auto-scaling
   - Implement scheduling
   - Monitor resource usage

## Common PowerShell and Azure CLI Commands

```powershell
# Create a VM
New-AzVM -ResourceGroupName "ResourceGroup1" `
         -Name "VM1" `
         -Location "eastus" `
         -Size "Standard_DS2_v2" `
         -Image "Win2019Datacenter"

# Create a scale set
New-AzVmss -ResourceGroupName "ResourceGroup1" `
           -VMScaleSetName "ScaleSet1" `
           -Location "eastus" `
           -VirtualNetworkName "Vnet1" `
           -SubnetName "Subnet1" `
           -PublicIpAddressName "Pip1" `
           -LoadBalancerName "LB1" `
           -UpgradePolicyMode "Automatic"

# Deploy container instance
New-AzContainerGroup -ResourceGroupName "ResourceGroup1" `
                     -Name "Container1" `
                     -Image "mcr.microsoft.com/azure-cli" `
                     -OsType Linux `
                     -DnsNameLabel "container1"
```

```bash
# Create a VM
az vm create \
    --resource-group ResourceGroup1 \
    --name VM1 \
    --image UbuntuLTS \
    --admin-username azureuser \
    --generate-ssh-keys

# Create a scale set
az vmss create \
    --resource-group ResourceGroup1 \
    --name ScaleSet1 \
    --image UbuntuLTS \
    --upgrade-policy-mode automatic \
    --admin-username azureuser \
    --generate-ssh-keys

# Deploy container instance
az container create \
    --resource-group ResourceGroup1 \
    --name Container1 \
    --image mcr.microsoft.com/azure-cli \
    --dns-name-label container1 \
    --ports 80
```

## Monitoring and Troubleshooting

1. **Monitoring Tools**:
   - Azure Monitor
   - Application Insights
   - Log Analytics
   - VM insights

2. **Common Issues**:
   - Connectivity problems
   - Performance bottlenecks
   - Scaling issues
   - Deployment failures

3. **Troubleshooting Steps**:
   - Check VM status
   - Review diagnostic logs
   - Monitor performance metrics
   - Verify network connectivity

## ARM Template Example

```json
{
    "$schema": "https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#",
    "contentVersion": "1.0.0.0",
    "parameters": {
        "vmName": {
            "type": "string",
            "metadata": {
                "description": "Name for the Virtual Machine"
            }
        }
    },
    "variables": {
        "vmSize": "Standard_DS2_v2"
    },
    "resources": [
        {
            "type": "Microsoft.Compute/virtualMachines",
            "apiVersion": "2021-03-01",
            "name": "[parameters('vmName')]",
            "location": "[resourceGroup().location]",
            "properties": {
                "hardwareProfile": {
                    "vmSize": "[variables('vmSize')]"
                },
                "osProfile": {
                    "computerName": "[parameters('vmName')]",
                    "adminUsername": "azureuser",
                    "adminPassword": "Password1234!"
                },
                "storageProfile": {
                    "imageReference": {
                        "publisher": "MicrosoftWindowsServer",
                        "offer": "WindowsServer",
                        "sku": "2019-Datacenter",
                        "version": "latest"
                    }
                }
            }
        }
    ]
}
```