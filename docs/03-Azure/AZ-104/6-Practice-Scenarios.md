# Practice Scenarios for AZ-104

This section contains practice scenarios that simulate real-world situations you might encounter in the exam. Each scenario is designed to test your knowledge across multiple exam objectives.

## Scenario 1: Identity and Access Management

### Situation
A company is implementing Azure AD for identity management and needs to set up appropriate access controls for different departments.

### Requirements
1. Create a hierarchical structure for resource management
2. Implement role-based access control (RBAC)
3. Set up group-based licensing
4. Enable multi-factor authentication for all users

### Tasks
1. Design and implement management groups
2. Create custom RBAC roles
3. Configure group-based license assignment
4. Set up conditional access policies

### Solution Steps
```powershell
# Create management group
New-AzManagementGroup -GroupName "Enterprise" -DisplayName "Enterprise Management"

# Create custom role
$role = Get-Content -Path "customrole.json" | ConvertFrom-Json
New-AzRoleDefinition -InputFile $role

# Assign role to group
New-AzRoleAssignment -ResourceGroupName "RG1" -SignInName "group@contoso.com" -RoleDefinitionName "Custom Role"
```

## Scenario 2: Storage and Backup Implementation

### Situation
A company needs to implement a secure storage solution with appropriate backup and disaster recovery capabilities.

### Requirements
1. Set up secure storage accounts
2. Implement backup policies
3. Configure disaster recovery
4. Ensure data encryption

### Tasks
1. Create storage accounts with appropriate security
2. Set up Azure Backup
3. Configure Azure Site Recovery
4. Implement encryption at rest and in transit

### Solution Steps
```powershell
# Create storage account with encryption
New-AzStorageAccount -ResourceGroupName "RG1" `
                     -Name "securestorage" `
                     -Location "eastus" `
                     -SkuName "Standard_GRS" `
                     -EnableHttpsTrafficOnly $true

# Set up backup vault
New-AzRecoveryServicesVault -ResourceGroupName "RG1" `
                           -Name "BackupVault" `
                           -Location "eastus"
```

## Scenario 3: Virtual Network Configuration

### Situation
A company needs to set up a secure virtual network infrastructure for their Azure resources.

### Requirements
1. Create virtual networks with proper segmentation
2. Implement network security
3. Configure load balancing
4. Set up VPN connectivity

### Tasks
1. Design and implement VNet architecture
2. Configure NSGs and ASGs
3. Set up Azure Load Balancer
4. Implement VPN Gateway

### Solution Steps
```powershell
# Create VNet
$subnet = New-AzVirtualNetworkSubnetConfig -Name "Subnet1" -AddressPrefix "10.0.1.0/24"
New-AzVirtualNetwork -ResourceGroupName "RG1" `
                     -Name "VNet1" `
                     -Location "eastus" `
                     -AddressPrefix "10.0.0.0/16" `
                     -Subnet $subnet

# Create NSG
New-AzNetworkSecurityGroup -ResourceGroupName "RG1" `
                          -Location "eastus" `
                          -Name "NSG1"
```

## Scenario 4: Compute Resource Management

### Situation
A company needs to deploy and manage scalable compute resources in Azure.

### Requirements
1. Deploy virtual machines with high availability
2. Implement auto-scaling
3. Configure monitoring and alerts
4. Manage VM access and security

### Tasks
1. Create VM scale sets
2. Configure availability sets
3. Set up Azure Monitor
4. Implement just-in-time VM access

### Solution Steps
```powershell
# Create VM scale set
New-AzVmss -ResourceGroupName "RG1" `
           -VMScaleSetName "VMSS1" `
           -Location "eastus" `
           -VirtualNetworkName "VNet1" `
           -SubnetName "Subnet1" `
           -PublicIpAddressName "pip1" `
           -LoadBalancerName "LB1"

# Configure monitoring
Set-AzDiagnosticSetting -ResourceId $vmss.Id `
                        -WorkspaceId $workspace.Id `
                        -Enabled $true
```

## Scenario 5: Monitoring and Backup Strategy

### Situation
A company needs to implement comprehensive monitoring and backup solutions for their Azure resources.

### Requirements
1. Set up resource monitoring
2. Implement backup policies
3. Configure disaster recovery
4. Create alerting system

### Tasks
1. Configure Azure Monitor
2. Set up backup policies
3. Implement Azure Site Recovery
4. Create alert rules and action groups

### Solution Steps
```powershell
# Create action group
$actionGroup = Set-AzActionGroup -ResourceGroupName "RG1" `
                                -Name "AG1" `
                                -ShortName "AG1" `
                                -Receiver @{
                                    Name = "email";
                                    EmailAddress = "admin@contoso.com";
                                    UseCommonAlertSchema = $true
                                }

# Create alert rule
Add-AzMetricAlertRule -ResourceGroupName "RG1" `
                      -Name "CPUAlert" `
                      -Location "eastus" `
                      -TargetResourceId $vm.Id `
                      -MetricName "Percentage CPU" `
                      -Operator GreaterThan `
                      -Threshold 90 `
                      -WindowSize 00:05:00 `
                      -TimeAggregationOperator Average
```

## Exam Tips and Tricks

1. **Time Management**:
   - Read questions carefully
   - Note key requirements
   - Manage time per question
   - Flag difficult questions for review

2. **Question Approach**:
   - Identify the scenario context
   - Understand the problem statement
   - Consider all requirements
   - Evaluate all options before selecting an answer

3. **Key Areas to Focus**:
   - Azure AD configuration
   - Network security
   - Resource management
   - Monitoring and backup
   - Cost optimization

4. **Common Pitfalls**:
   - Not reading all requirements
   - Missing security considerations
   - Overlooking cost implications
   - Forgetting about scalability

## Practice Exercise Template

Use this template to create your own practice scenarios:

1. **Scenario Description**:
   - Background information
   - Business requirements
   - Technical constraints
   - Expected outcomes

2. **Required Tasks**:
   - List specific tasks
   - Note dependencies
   - Identify key considerations
   - Define success criteria

3. **Implementation Steps**:
   - Step-by-step instructions
   - Command examples
   - Configuration details
   - Validation steps

4. **Validation Questions**:
   - What security measures are in place?
   - How is high availability ensured?
   - What monitoring is implemented?
   - How is cost optimization achieved?

## Additional Resources

1. **Microsoft Documentation**:
   - [Azure Documentation](https://docs.microsoft.com/azure/)
   - [Azure Architecture Center](https://docs.microsoft.com/azure/architecture/)
   - [Azure CLI Documentation](https://docs.microsoft.com/cli/azure/)
   - [Azure PowerShell Documentation](https://docs.microsoft.com/powershell/azure/)

2. **Practice Labs**:
   - Microsoft Learn
   - Azure Portal
   - Azure Cloud Shell
   - Local development environment

3. **Community Resources**:
   - Azure Forums
   - Stack Overflow
   - GitHub repositories
   - Tech blogs