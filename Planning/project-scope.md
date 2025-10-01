# Project Scope

## Objective

- Deploy six Ubuntu Linux virtual machines in Azure to provide core infrastructure services.
- Secure the environment using Azure Firewall, Network Security Groups, and iptables.
- Automate virtual machine provisioning, configuration, and backups with scripts.
- Integrate identity and access management via Azure Active Directory.
- Enroll servers in Microsoft Intune for policy compliance.
- Enable team collaboration and documentation through Microsoft 365 (Teams, SharePoint, Exchange)

## Deliverables 

- Creation of the following Azure resources:
  - Microsoft 365 tenant
  - SSH key pair for VM access
  - Virtual network with server and client subnets
  - Network Security Group with firewall rules
  - Static private IP addresses for each VM
  - Public IP for SSH jump-host (optional)
  - Six Ubuntu LTS VMs: rocky, darwin, adelaide, sydney, gladstone, bundaberg
- Configuration tasks:
  - Router/NAT setup on rocky
  - DHCP service on darwin
  - Apache + DokuWiki on adelaide
  - SSH hardening and audit on sydney
  - Git server and DokuWiki sync on gladstone
  - Backup scripts and schedule on bundaberg
- Integration tasks:
  - Azure AD user and group setup
  - Conditional Access policy for SSH
  - Intune device compliance profiles
  - Microsoft 365 collaboration setup
