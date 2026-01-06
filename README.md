# Azure IaC Bicep Demo

Deploy a scalable, secure Azure infrastructure using Bicep with CI/CD via GitHub Actions. This demo includes a hub-and-spoke network, NSGs, a VM Scale Set, Azure Bastion, and governance with tagging and policies.

## Architecture

- Hub VNet with Azure Bastion for secure access (no public IPs)
- Spoke VNet for workloads with NSGs and route control
- VM Scale Set behind a load balancer in the spoke
- Azure Monitor diagnostics and Log Analytics
- Governance: mandatory tagging and policy assignment

## Tech stack

- Azure: VNets, NSGs, Bastion, VMSS, Load Balancer, Log Analytics, Policy
- IaC: Bicep modules with parameterization
- Automation: GitHub Actions (CI), Azure CLI
- Optional: PowerShell helper scripts

## Repo structure

