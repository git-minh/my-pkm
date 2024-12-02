# Section 5: Monitor and Back Up Azure Resources (10-15%)

## 1. Monitor Resources by Using Azure Monitor

### Configure and Interpret Metrics and Logs
- **Azure Monitor Metrics**:
  - Platform metrics
  - Custom metrics
  - Metric namespaces
  - Dimensional metrics
- **Log Analytics**:
  - Workspace configuration
  - Data collection
  - Log queries
  - Data retention
- **Diagnostic Settings**:
  - Resource diagnostics
  - Activity logs
  - Guest diagnostics

### Set Up Alerts and Action Groups
- **Alert Rules**:
  - Metric alerts
  - Log alerts
  - Activity log alerts
  - Smart alerts
- **Action Groups**:
  - Notification methods
  - Action types
  - Automation
- **Alert Processing**:
  - Alert states
  - Alert suppression
  - Alert history

### Monitor Azure Services and Applications
- **Application Insights**:
  - Instrumentation
  - Performance monitoring
  - Usage analytics
  - Availability tests
- **VM Insights**:
  - Performance metrics
  - Map dependencies
  - Health monitoring
- **Container Monitoring**:
  - Container insights
  - Kubernetes monitoring
  - Container logs

### Utilize Log Analytics and Workspaces
- **Workspace Configuration**:
  - Access control
  - Data sources
  - Solutions
- **Log Queries**:
  - Kusto Query Language (KQL)
  - Query optimization
  - Saved queries
- **Data Analysis**:
  - Dashboards
  - Workbooks
  - Power BI integration

## 2. Implement Backup and Recovery

### Configure and Manage Azure Backup Policies
- **Backup Components**:
  - Recovery Services vault
  - Backup policies
  - Protection groups
- **Policy Configuration**:
  - Schedule settings
  - Retention settings
  - Storage replication
- **Backup Types**:
  - VM backup
  - File and folder backup
  - Database backup
  - Application-consistent backup

### Perform Backup and Restore Operations
- **Backup Operations**:
  - On-demand backup
  - Scheduled backup
  - Monitoring backup jobs
- **Restore Operations**:
  - Full restore
  - File-level recovery
  - Cross-region restore
- **Recovery Points**:
  - Recovery point types
  - Recovery point retention
  - Recovery point consistency

### Implement Azure Site Recovery for Disaster Recovery
- **Site Recovery Components**:
  - Configuration server
  - Process server
  - Master target server
- **Replication Settings**:
  - Replication policies
  - Network mapping
  - Capacity planning
- **Failover and Failback**:
  - Test failover
  - Planned failover
  - Unplanned failover
  - Failback process

### Configure Recovery Services Vault
- **Vault Setup**:
  - Create and configure vault
  - Storage redundancy
  - Access policies
- **Security Settings**:
  - Encryption
  - RBAC
  - Soft delete
- **Monitoring and Reporting**:
  - Backup reports
  - Alert configuration
  - Usage tracking

## Best Practices and Considerations

1. **Monitoring Strategy**:
   - Define monitoring requirements
   - Set up appropriate metrics
   - Configure meaningful alerts
   - Implement proper log retention

2. **Backup Planning**:
   - Identify critical resources
   - Define RPO and RTO
   - Plan backup schedules
   - Test restore procedures

3. **Disaster Recovery**:
   - Document DR procedures
   - Regular testing
   - Update recovery plans
   - Monitor replication health

4. **Cost Management**:
   - Monitor storage usage
   - Optimize retention periods
   - Review backup policies
   - Track recovery points

## Common PowerShell and Azure CLI Commands

```powershell
# Create a Recovery Services vault
New-AzRecoveryServicesVault -ResourceGroupName "ResourceGroup1" `
                           -Name "Vault1" `
                           -Location "eastus"

# Configure backup policy
$policy = Get-AzRecoveryServicesBackupProtectionPolicy -Name "DefaultPolicy"
Enable-AzRecoveryServicesBackupProtection -ResourceGroupName "ResourceGroup1" `
                                         -Name "VM1" `
                                         -Policy $policy

# Trigger backup
Backup-AzRecoveryServicesBackupItem -Item $backupItem
```

```bash
# Create a Recovery Services vault
az backup vault create \
    --resource-group ResourceGroup1 \
    --name Vault1 \
    --location eastus

# Configure backup policy
az backup protection enable-for-vm \
    --resource-group ResourceGroup1 \
    --vault-name Vault1 \
    --vm VM1 \
    --policy-name DefaultPolicy

# Trigger backup
az backup protection backup-now \
    --resource-group ResourceGroup1 \
    --vault-name Vault1 \
    --container-name VM1 \
    --item-name VM1
```

## Monitoring and Troubleshooting Guide

1. **Common Monitoring Scenarios**:
   - Resource performance
   - Application availability
   - Security and compliance
   - Cost optimization

2. **Backup Issues**:
   - Backup failures
   - Restore failures
   - Replication issues
   - Capacity problems

3. **Alert Management**:
   - Alert configuration
   - Alert response
   - Alert remediation
   - Escalation procedures

4. **Log Analysis**:
   - Query techniques
   - Performance analysis
   - Security investigation
   - Compliance reporting

## Sample KQL Queries

```kusto
// CPU usage for all VMs
Perf
| where ObjectName == "Processor"
| where CounterName == "% Processor Time"
| summarize avg_cpu = avg(CounterValue) by Computer
| order by avg_cpu desc

// Failed backup jobs in last 24 hours
AzureBackupReport
| where OperationName == "Backup"
| where Status == "Failed"
| where TimeGenerated > ago(24h)
| project TimeGenerated, ResourceName, ErrorString

// Security events
SecurityEvent
| where EventID == 4625  // Failed logon attempts
| summarize count() by Account, Computer
| order by count_ desc
```

## Azure Monitor Workbooks

1. **Performance Monitoring**:
```json
{
    "version": "Notebook/1.0",
    "items": [
        {
            "type": "metric",
            "resourceMetadata": {
                "type": "microsoft.compute/virtualmachines"
            },
            "metrics": [
                {
                    "name": "Percentage CPU",
                    "aggregationType": "Average"
                }
            ]
        }
    ]
}
```

2. **Backup Monitoring**:
```json
{
    "version": "Notebook/1.0",
    "items": [
        {
            "type": "query",
            "content": {
                "query": "AzureBackupReport | summarize count() by Status"
            }
        }
    ]
}
```

## Disaster Recovery Plan Template

1. **Pre-Failover Checklist**:
   - Verify replication health
   - Check network connectivity
   - Validate DNS settings
   - Review application dependencies

2. **Failover Procedure**:
   - Stop applications
   - Trigger failover
   - Verify DNS updates
   - Test application functionality

3. **Post-Failover Tasks**:
   - Verify data consistency
   - Update documentation
   - Monitor performance
   - Test user access

4. **Failback Planning**:
   - Assess primary site
   - Reverse replication
   - Plan maintenance window
   - Execute failback
``` 