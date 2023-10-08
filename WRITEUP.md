# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
    + Cost : VM cost is higher than App Service
    + Availability : Microsoft manage underlaying hardware so App Service have high availability, VM solution provide high availability with group of VMs
    + Scalability : VM is less flexiable than App Service at small scale (auto scale hardware RAM, CPU) but VM can mutiply for larger scale
    + Workflow : Manage config, install, deploy include update OS

- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*
    + App service have full control with Azure Portal on web without ssh or remote access to the VM to start configuration
    + Cost : App Service cost is lower than Virtual Machince
    + Less effort needed to config App Service : App service support python v3.8, auto build and get dependiences and no need to download and install runtime, sdk, other configurations, ... like VM

### Assess app changes that would change your decision.
Switch to VM if:
- Migrating some existing on-premise to cloud
- If application written in language that App Service not support

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 