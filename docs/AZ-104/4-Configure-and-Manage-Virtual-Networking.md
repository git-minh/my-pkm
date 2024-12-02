# Section 4: Configure and Manage Virtual Networking (25-30%)

## 1. Implement and Manage Virtual Networking

### Create and Configure Virtual Networks (VNets)
- **VNet Basics**:
  - Address space planning
  - Subnet design
  - Network security
- **Configuration**:
  - VNet peering
  - DNS settings
  - Service endpoints
- **Best Practices**:
  - IP addressing scheme
  - Subnet sizing
  - Network segmentation

### Configure Private and Public IP Addresses
- **Private IP Addressing**:
  - Static vs dynamic allocation
  - IP address ranges
  - Subnet assignment
- **Public IP Addressing**:
  - SKU types (Basic/Standard)
  - Assignment methods
  - IPv6 support
- **IP Configuration**:
  - DNS settings
  - Routing
  - Network interfaces

### Configure Network Security Groups (NSGs) and Application Security Groups (ASGs)
- **NSG Rules**:
  - Inbound/outbound rules
  - Priority settings
  - Default rules
- **ASG Configuration**:
  - Group creation
  - Member assignment
  - Rule association
- **Security Best Practices**:
  - Rule organization
  - Logging and monitoring
  - Regular audits

### Implement VNet Peering and Service Chaining
- **VNet Peering**:
  - Local vs global peering
  - Gateway transit
  - Network access
- **Service Chaining**:
  - User-defined routes
  - Network virtual appliances
  - Traffic flow

## 2. Configure Name Resolution

### Configure Azure DNS
- **DNS Zones**:
  - Public DNS zones
  - Private DNS zones
  - Record management
- **DNS Records**:
  - Record types (A, AAAA, CNAME, etc.)
  - TTL settings
  - Alias records
- **DNS Settings**:
  - Custom domain names
  - DNS resolution
  - Integration with other services

### Integrate Custom DNS Servers
- **Custom DNS Configuration**:
  - DNS server setup
  - VNet DNS settings
  - Forwarding rules
- **Hybrid DNS**:
  - On-premises integration
  - Conditional forwarding
  - Split-horizon DNS

### Configure Private and Public DNS Zones
- **Private DNS Zones**:
  - Zone creation
  - VNet links
  - Auto-registration
- **Public DNS Zones**:
  - Zone delegation
  - Record sets
  - DNS policies

## 3. Secure Access to Virtual Networks

### Implement Azure Virtual Network NAT
- **NAT Gateway**:
  - Configuration
  - IP address management
  - Scaling options
- **NAT Rules**:
  - Outbound connectivity
  - IP address assignment
  - Port management

### Configure VPN Gateways
- **Gateway Types**:
  - Point-to-Site (P2S)
  - Site-to-Site (S2S)
  - VNet-to-VNet
- **VPN Configuration**:
  - Gateway SKUs
  - Routing
  - Authentication
- **Connection Types**:
  - IPsec/IKE
  - OpenVPN
  - SSTP

### Implement Azure ExpressRoute and Direct Access
- **ExpressRoute**:
  - Circuit provisioning
  - Peering configuration
  - Routing domains
- **Direct Access**:
  - Azure Bastion
  - Just-in-time access
  - Private Link

## 4. Configure Load Balancing

### Configure Azure Load Balancer (Layer 4)
- **Load Balancer Types**:
  - Public Load Balancer
  - Internal Load Balancer
- **Configuration**:
  - Frontend IP
  - Backend pools
  - Health probes
  - Load balancing rules
- **Advanced Features**:
  - Session persistence
  - Outbound rules
  - HA ports

### Implement Application Gateway (Layer 7)
- **Components**:
  - Frontend IP configurations
  - Backend pools
  - Listeners
  - Rules
- **Features**:
  - SSL termination
  - URL-based routing
  - Web Application Firewall (WAF)
- **Configuration**:
  - Health probes
  - Session affinity
  - Autoscaling

### Configure Traffic Manager and Front Door
- **Traffic Manager**:
  - Routing methods
  - Endpoint monitoring
  - DNS configuration
- **Front Door**:
  - WAF policies
  - Caching
  - URL-based routing
- **Integration**:
  - Multi-region deployment
  - Backend health monitoring
  - SSL management

## 5. Monitor and Troubleshoot Virtual Networking

### Use Network Watcher for Diagnostics
- **Network Watcher Tools**:
  - Connection Monitor
  - IP flow verify
  - Next hop
  - Packet capture
- **Diagnostic Features**:
  - NSG flow logs
  - VPN diagnostics
  - Traffic Analytics

### Monitor On-Premises Connectivity
- **Monitoring Tools**:
  - ExpressRoute monitoring
  - VPN monitoring
  - Connection metrics
- **Diagnostics**:
  - Connectivity testing
  - Performance monitoring
  - Troubleshooting

### Troubleshoot External Networking
- **Common Issues**:
  - DNS resolution
  - Routing problems
  - Security rules
- **Tools and Techniques**:
  - Network performance monitor
  - Log Analytics
  - Azure Monitor

## Best Practices and Considerations

1. **Network Design**:
   - Plan IP addressing carefully
   - Implement proper segmentation
   - Consider future growth
   - Document network architecture

2. **Security**:
   - Use NSGs effectively
   - Implement least privilege
   - Regular security audits
   - Monitor network traffic

3. **Performance**:
   - Choose appropriate SKUs
   - Monitor bandwidth usage
   - Implement proper routing
   - Use load balancing effectively

4. **Monitoring**:
   - Enable diagnostic logging
   - Set up alerts
   - Regular performance reviews
   - Track network metrics

## Common PowerShell and Azure CLI Commands

```powershell
# Create a VNet
New-AzVirtualNetwork -ResourceGroupName "ResourceGroup1" `
                     -Location "eastus" `
                     -Name "VNet1" `
                     -AddressPrefix "10.0.0.0/16"

# Create an NSG
New-AzNetworkSecurityGroup -ResourceGroupName "ResourceGroup1" `
                          -Location "eastus" `
                          -Name "NSG1"

# Create a load balancer
New-AzLoadBalancer -ResourceGroupName "ResourceGroup1" `
                   -Name "LB1" `
                   -Location "eastus" `
                   -FrontendIpConfiguration $frontendIP `
                   -BackendAddressPool $backendPool
```

```bash
# Create a VNet
az network vnet create \
    --resource-group ResourceGroup1 \
    --name VNet1 \
    --address-prefix 10.0.0.0/16

# Create an NSG
az network nsg create \
    --resource-group ResourceGroup1 \
    --name NSG1

# Create a load balancer
az network lb create \
    --resource-group ResourceGroup1 \
    --name LB1 \
    --frontend-ip-name FrontEndIP \
    --backend-pool-name BackEndPool
```

## Troubleshooting Guide

1. **Connectivity Issues**:
   - Verify NSG rules
   - Check routing tables
   - Validate DNS resolution
   - Test network connectivity

2. **Performance Problems**:
   - Monitor bandwidth usage
   - Check for bottlenecks
   - Validate load balancer health
   - Review network metrics

3. **Security Concerns**:
   - Audit NSG rules
   - Review network logs
   - Check for unauthorized access
   - Validate security policies

4. **DNS Issues**:
   - Verify DNS settings
   - Check record configuration
   - Test name resolution
   - Review DNS logs