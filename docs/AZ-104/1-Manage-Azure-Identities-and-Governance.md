# Section 1: Manage Azure Identities and Governance (15-20%)

## 1. Manage Azure Active Directory (Azure AD) Objects

### Create and Manage Users and Groups

#### User Accounts
- **Creation Methods**:
  - Azure Portal: Create individual user accounts with required fields (name, username, password)
  - Azure CLI & PowerShell: Create users programmatically
  - Bulk Import: Import multiple users using CSV files
- **User Properties**:
  - Profile Settings: Configure job title, department, contact information
  - Password Management: Set initial passwords, enforce policies, enable self-service password reset (SSPR)
- **Guest Users**:
  - B2B Collaboration: Invite external users
  - Access Management: Control guest user permissions

#### Groups
- **Group Types**:
  - Security Groups: Manage member and computer access to shared resources
  - Microsoft 365 Groups: Provide collaboration capabilities
- **Group Management**:
  - Creation and Deletion: Via portal, CLI, or PowerShell
  - Membership Management: Add/remove members and owners
- **Dynamic Membership**:
  - Rules: Create groups with dynamic membership rules
  - Use Cases: Automate group membership

### Manage Licenses in Azure AD
- **Assigning Licenses**:
  - Individual Assignment: Direct license assignment to users
  - Group-Based Licensing: Assign licenses to groups
- **License Management**:
  - Monitoring Usage: Track allocation and usage
  - Reallocation: Remove and reassign licenses
- **Service Plans**:
  - Enable/Disable Services: Customize available services within a license

### Configure Azure AD Join and Device Settings
- **Azure AD Join**:
  - Device Enrollment: Join devices to Azure AD
  - Management: Enable/disable joined devices
- **Device Settings**:
  - Device Registration: Configure registration settings
  - Conditional Access: Implement device compliance policies
- **Hybrid Azure AD Join**:
  - Integration: Configure hybrid join with on-premises AD
  - Prerequisites: Azure AD Connect setup

## 2. Manage Role-Based Access Control (RBAC)

### Create Custom Roles
- **Role Definitions**:
  - JSON Templates: Define roles using JSON
  - Permissions: Specify granular permissions
- **Creation Methods**:
  - Azure Portal: Use Custom Roles interface
  - PowerShell & CLI: Create roles programmatically

### Assign RBAC Roles
- **Role Assignment Scope**:
  - Scopes: Management group, subscription, resource group, resource
  - Inheritance: Understanding permission inheritance
- **Assignment Methods**:
  - Azure Portal: Use Access Control (IAM)
  - PowerShell & CLI: Use role assignment commands
- **Principals**:
  - Users and Groups: Assign roles to individuals or groups
  - Service Principals: Assign roles to applications

### Interpret Access Assignments
- **Effective Permissions**:
  - Access Evaluation: Use "Check Access" feature
  - Permission Sources: Direct, group membership, inheritance
- **Troubleshooting Access**:
  - Deny Assignments: Identify blocking assignments
  - Policy Conflicts: Recognize policy restrictions

## 3. Manage Subscriptions and Governance

### Configure Azure Policies
- **Policy Components**:
  - Definitions: Templates for policy rules
  - Assignments: Apply policies to scopes
  - Parameters: Make policies flexible
- **Built-in Policies**:
  - Common Scenarios: Tag usage, allowed locations
- **Custom Policies**:
  - Creation: Write custom definitions
  - Testing: Validate policies
- **Policy Effects**:
  - Deny: Block non-compliant resources
  - Audit: Log non-compliance
  - Append: Add settings to resources
  - DeployIfNotExists: Deploy related resources

### Implement Resource Locks
- **Lock Levels**:
  - ReadOnly: Allow read operations only
  - Delete: Prevent deletion
- **Application Scope**:
  - Inheritance: Locks inherit down the resource hierarchy
- **Management**:
  - Creating Locks: Via portal or PowerShell
  - Removing Locks: Require appropriate permissions

### Manage Resource Groups and Subscriptions
- **Resource Groups**:
  - Organization: Group related resources
  - Lifecycle Management: Delete groups and contents
- **Subscription Management**:
  - Creation: Set up new subscriptions
  - Access Control: Assign permissions
  - Billing: Monitor costs and budgets
- **Tags**:
  - Metadata Assignment: Apply tags for organization
  - Tag Policies: Enforce tagging rules

### Use Azure Blueprints for Standardization
- **Blueprint Components**:
  - Artifacts: Role assignments, policies, templates
  - Versions: Track changes
- **Deployment**:
  - Assignment: Apply to subscriptions
  - Locking: Prevent modification
- **Lifecycle Management**:
  - Updates: Manage blueprint assignments
  - Drift: Monitor and correct deviations

## Best Practices and Considerations

1. **Identity Management**:
   - Follow least privilege principle
   - Implement strong password policies
   - Enable MFA for all users
   - Regular access reviews

2. **Governance**:
   - Use management groups for hierarchical organization
   - Implement consistent naming conventions
   - Apply appropriate resource locks
   - Regular policy compliance reviews

3. **Cost Management**:
   - Monitor subscription costs
   - Use tags for cost allocation
   - Set up budgets and alerts
   - Regular license optimization

## Common PowerShell and Azure CLI Commands

```powershell
# Create a new user
New-AzureADUser -DisplayName "John Doe" -UserPrincipalName "john@contoso.com"

# Assign RBAC role
New-AzRoleAssignment -SignInName "john@contoso.com" -RoleDefinitionName "Contributor"

# Create a custom role
New-AzRoleDefinition -InputFile "customrole.json"

# Create a resource lock
New-AzResourceLock -LockName "LockName" -LockLevel CanNotDelete -ResourceGroupName "ResourceGroup1"
```

```bash
# Create a new user (Azure CLI)
az ad user create --display-name "John Doe" --user-principal-name "john@contoso.com"

# Assign RBAC role
az role assignment create --assignee "john@contoso.com" --role "Contributor"

# Create a policy assignment
az policy assignment create --name "require-tag" --policy "require-tag-on-resource"

# Create a resource lock
az lock create --name "LockName" --resource-group "ResourceGroup1" --lock-type CanNotDelete
``` 