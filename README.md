# Azure-Cloud-Sysadmin-Project

## Overview  
This personal project is an extension of [Cqunix-Sysadmin-Project](https://github.com/Tim-Port-Foli-Ho/Cqunix-Sysadmin-Project), replicating the internal network of cqunix project on Microsoft Azure cloud infrastuture. The system will be rebuilt using Azure Virtual Machines and relevant Azure services for security, automation, identity management, and collaboration.

The six core roles and their respecive IP address from the original design will be kept the same. Gladstone and Adelaide are modified to be more inline with Azure products to showcase cloud skills

- **Adelaide**: Azure App Service hosting internal documentation with HTTPS
- **Sydney**: Azure VM providing secure SSH access and acting as the central management jump host
- **Gladstone**: Azure DevOps Azure Repos replacing the internal Git server for source control and continuous integration
- **Bundaberg**: Azure VM running backup automation scripts storing backups via VM snapshots or Azure Storage
- **Darwin**: Azure VM running DHCP server maintaining IP address allocation with reserved static IPs
- **Rocky**: Azure VM configured as router/firewall with iptables and Azure NSGs controlling network traffic

## Scope  
- Implement the cqunix small business network on Azure using Ubuntu Linux VMs and Azure cloud services
- Manually configure the baseline Ubuntu Linux VM
- Automate VM configuration with ARM template
- Secure environment with Network Security Groups, iptables, and Azure identity management
- Utilize Azure DevOps for Git repository management and pipeline automation
- Deploy Azure App Service for hosting the company's internal web documentation
- Implement backup automation via VM snapshots and script-driven
- Integrate Azure Active Directory for VM authentication
- Use Microsoft 365 Education suite for team collaboration tools (Teams, SharePoint, Exchange)

## Assumptions  
- Basic Linux and Azure cloud knowledge expected
- Single subnet 192.168.100.0/24 maintained as per on-premises design
- Minimal size VMs used with auto-shutdowns for cost control
- Azure Firewall omitted to optimize cost; NSGs and VM iptables used instead

## Implementation Roadmap  
- Setup Azure Virtual Network (VNet) and reserve static private IP  
- Deploye and configure Rocky (router/firewall) and Darwin (DHCP) VM  
- Deploy Sydney SSH server VM and secure access
- Substitute Gladstone VM with Azure DevOps Azure Repos for Git and pipeline management
- Deploy Adelaide as an Azure App Service hosting documentation with HTTPS
- Automate backups via VM snapshots and scripts on Bundaberg VM
- Integrate Azure Active Directory authentication for VMs
- Enable Microsoft 365 Education collaboration tools
- Thoroughly test connectivity, backup, recovery, and security configurations
- Document implementation details, configurations, and user
