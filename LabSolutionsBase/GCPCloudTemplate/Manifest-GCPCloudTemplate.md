## Lab Profile Manifest

### Cloud Settings

#### GCP Cloud
>[+] Cloud Configuration
>
| Item | Detail |
|:---------|:---------|
| Platform | **GCP** |
| User | +++@lab.CloudPortalCredential(User1).Username+++ |
| Password | +++@lab.CloudPortalCredential(User1).Password+++ |
| Deployment Group | **@lab.CloudResourceGroup(Stack1).Name**|


#### Resource Templates
>[+] For GCP cloud labs, Resource Templates are implemented through Cloud Deployment Manager Templates. 
>
>There are no Cloud Deployment Manager Templates in this base profile to deploy resources. Learn more about the types of resources you can deploy using [Cloud Deployment Manager Templates](https://cloud.google.com/deployment-manager/docs/configuration/templates/create-basic-template) in this profile. 



#### Allow Policies
>[+] For GCP cloud labs, Allow Policies are implemented through IAM Policies. 
>
>There are no policies on this base profile, thereby denying access by default. Learn more about the types of [IAM policies](https://cloud.google.com/resource-manager/docs/access-control-org) you can implement to allow access to GCP resources. 


#### Quota
>[+] For GCP cloud labs, Quotas are implemented to set global limits on the resources that can be deployed. 
>
>There are no Quotas on this base profile. Learn more about [Cloud Quotas](https://cloud.google.com/docs/quotas) in the GCP documentation. 


### Life Cycle:
There are no Life Cycle settings in this lab profile.

### Virtual Machines:
There are no virtual machine settings in this lab profile.

### Networks:
There are no network settings in this lab profile.

### Cloud Resources:
This is a base cloud template with no resources deployed.
