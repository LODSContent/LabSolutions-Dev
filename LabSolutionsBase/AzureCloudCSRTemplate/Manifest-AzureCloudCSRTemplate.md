## Lab Profile Manifest

### Cloud Settings

#### Azure Cloud CSR
>[+] Cloud Configuration
>
| Item | Detail |
|:---------|:---------|
| Platform | **Azure** |
| User | +++@lab.CloudPortalCredential(User1).Username+++ |
| Password | +++@lab.CloudPortalCredential(User1).Password+++ |
| Resource Group | **@lab.CloudResourceGroup(ResourceGroup1).Name**|


## Resource Templates
>[+] For Azure cloud labs, Resource Templates are implemented through Azure Resource Manager (ARM) Templates. 
>
>There are no ARM Templates in this base profile to deploy resources. Learn more about the types of resources you can deploy using [ARM Templates](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/overview) in this profile. 


## Access Control Policies
>[+] For Azure cloud labs, Access Control Policies are implemented through Azure Policy. 
>
>The only policy on this base profile is a **Deny All** policy that prevents access to all resources. Learn more about the types of [Azure policies](https://learn.microsoft.com/en-us/azure/governance/policy/overview) you can implement to allow access to Azure resources. 

## Life Cycle:
There are no Life Cycle settings in this lab profile.

## Virtual Machines:
There are no virtual machine settings in this lab profile.

## Networks:
There are no network settings in this lab profile.

## Cloud Resources:
This is a base cloud template with no resources deployed.
