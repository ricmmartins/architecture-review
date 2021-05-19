# Architecture Review Guidelines

> :bulb: The intent of this repository is to serve as a guidance to Azure Architecture Reviews, taking in consideration the main topics from Cloud Adoption Framework and Well-Architected Framework.

## Governance

### Availability and Resiliency

- [ ] Recommend to [enable service health alerts](https://docs.microsoft.com/en-us/azure/service-health/alerts-activity-log-service-notifications-portal).
- [ ] Recommend to [create alerts](https://docs.microsoft.com/en-us/azure/azure-monitor/alerts/alerts-overview#create-an-alert-rule) for [metrics](https://docs.microsoft.com/en-us/azure/azure-monitor/essentials/metrics-supported) on resource [limits and quotas](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-subscription-service-limits), failures, or bottlenecks.
- [ ] Recommend to [enable VM Insights](https://docs.microsoft.com/en-us/azure/azure-monitor/vm/vminsights-overview) to get pre-created dashboards and alerts for Virtual Machine resources.
- [ ] Recommend to [create support cases](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/how-to-create-azure-support-request) through the Azure portal in advanced to increase quota limits.

### Scalability and Performance

- [ ] Recommend to configure alerts to auto-scale Azure VMs either [vertically](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-vertical-scale-reprovision) or [horizontally (using VMSS)](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/virtual-machine-scale-sets-autoscale-portal).
- [ ] Recommend to keep close track of [Azure subscription limits via the quotas in the Azure portal](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/resource-manager-core-quotas-request).

### Security

- [ ] Recommend to enable Azure Security Center for subscriptions.
* Recommend to re-use pre-configured log analytics workspaces for VMs.
- [ ] Recommend to re-use pre-configured log analytics workspaces for VMs.
- [ ] Recommend to lock Azure resources critical to the infrastructure such as VNets, DNS, DCs, gateways, NVAs, ER circuits, NSGs etc.
- [ ] Recommend to enable Azure policies to enforce ruleset on Azure subscriptions in scenarios such as: 
 - [ ] Geo-compliance
* Service Curation
* Auto-tagging and tag value enforcement
- [ ] Recommend to leverage RBAC for access control. 
* Recommend to follow Least Access Priviledge and assign RBAC roles at resource group scopes.
* Recommend to prioritize built-in RBAC roles vs. custom RBAC roles.
* Recommend to keep Owner RBAC roles as high privileges assignments. 
- [ ] Recommend to audit management plane actions using the Azure Activity Log
- [ ] Recommend to use Azure Key Vault for key, secrets and certificate store and management.
- [ ] Recommend to leverage Azure Automation’s Patch management, inventory, and change tracking for VMs in-guest OS controls/monitoring.


### Management

### DevOps

---

## Networking

### Availability and Resiliency

### Scalability and Performance

### Security

### Management

### DevOps

---

## Infrastructure (Compute/Storage)

### Availability and Resiliency

### Scalability and Performance

### Security

### Management

### DevOps

---

## Identity

### Availability and Resiliency

### Scalability and Performance

### Security

### Management

### DevOps



