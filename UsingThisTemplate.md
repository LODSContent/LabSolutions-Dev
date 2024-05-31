# Using this lab template

This template has been provided as a starting point for lab creation. In many cases modifications are required to meet the specific needs of your lab goals. Below are some of the details that can be used to customize the environment:

>[!knowledge] Want to learn more? Review the documentation on [Template Gallery](https://docs.skillable.com/docs/template-gallery)

## Modify Virtual Environment
Lab environments may contain Virtual Machines, Containers or Cloud settings. These can be modified either prior to copying the template, or after.

If the provided virtual machines or containers require changes/updates to, or addition/removal of software, you may perform this now. Once you have completed the updates you require, or if the virtual machines or containers do not need any software modifications, please advance to the **Save Modified Environment** section to perform tasks such as modifying hardware settings (including RAM and CPU), removing components like entire virtual machines or networks, or making changes to Cloud settings.

>[!knowledge] Want to learn more? Review the documentation on [Lab Profile](https://docs.skillable.com/docs/lab-profile) settings.

>[!NOTE] If you make changes to the virtual environment while testing the environment and do NOT want to keep them, you can choose to discard them in the next steps.

## Virtual Machine Licensing

### Windows Virtual Machines

Windows licensing will vary from template to template, and even from VM to VM within those templates. There are two versions of Windows which will have unique licensing requirements depending on your use.

- Windows Server virtual machines will not be licensed within LOD provided templates. There are two options in licensing Windows Server virtual machines:

    1. **License on your own** - This would utilize your own Windows Server licensing keys in a method that corresponds to the licensing agreement between your organization and Microsoft.

    1. **Use LODS provided licensing** - If you would like for LODS to license your Windows Server virtual machine, please submit a [Lab Services ticket](https://lod.one/support). If you have not already discussed the fees that relate to using LODS licensing with your LODS Account Representative, you should reach out to them first to discuss cost implications.
     
    > [!ALERT] This will incur charges for ALL virtual machines in a lab profile (including non-Windows machines) at a rate according to your customer contract.

- Windows 10 virtual machines will be supplied with the **Enterprise** edition of Windows. This means that virtual machines will never shut themselves down due to too much time running without a license.

    - However, these virtual machines should be licensed by you based on the licensing requirements between your organization and Microsoft.

>[!knowledge] Want to learn more? Review the documentation on [Windows licensing](https://docs.skillable.com/docs/windows-licensing) on our platform.

### Linux Virtual Machines

Distributions of Linux provided in your template will utilize open source licensing, and therefore are ready to go on launch!

## Cloud Lab Settings

For a lab that is using a cloud platform such as Azure, AWS, or Google Cloud, additional settings are required. You will need to specify a Cloud Subscription, Resource Templates, and Access Control Policies among other settings.

>[!knowledge] Want to learn more? Review the documentation on [Skillable Cloud Fabrics](https://docs.skillable.com/docs/cloud-fabric-explanation).

Azure environments will require settings such as User Accounts, Resource Groups, Resource Templates, and Access Control Policies.

>[!knowledge] Want to learn more? Review the documentation on [Azure Cloud Settings](https://docs.skillable.com/docs/cloud-slice-guide-microsoft-azure-setup).

AWS environments will require settings such as User Accounts, Stack Deployments, Resource Templates, and Access Control Policies.

>[!knowledge] Want to learn more? Review the documentation on [AWS Cloud Settings](https://docs.skillable.com/docs/enable-aws-cloud-slice-support). 

## Save Modified Environment

To permanently save this environment into your own organization, follow these steps:

1. From the lab menu in the in upper right of the navigation pane, select **Save Changes**.

1. Select whether you would like to save any changes as an update to the current lab, or create a new one.
    
>[!knowledge] Want to learn more? Review the documentation on [saving a lab profile](https://docs.skillable.com/docs/lab-profile-cloning) 
