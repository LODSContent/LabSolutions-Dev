:::module(module=Environment)

### Environment

| Item | Detail |
| :--- | :--- |
| **Description** | AWS cloud environment using a customer provided subscription pool. |
| **Software/Configuration** | Default AWS configuration. |
| **Platform/Fabric** | AWS |
|  |  |

>[!note] *This template is provided "as-is," without any express or implied warranty. In no event shall the author be held liable for any damages arising from the use of this template.*

:::


:::module(module=Access&#32and&#32Credentials)

### Access and Credentials

| Item | Detail |
| :--- | :--- |
| User | ++@lab.CloudPortalCredential(User1).Username++ |
| Password | ++@lab.CloudPortalCredential(User1).Password++ |
|  |  |

:::


:::module(module=Software&#32and&#32Updates)

### Software and Updates

| Software Product | Install Date or Version | Configuration Notes |
| :--- | :--- | :--- |
| None | | No software or resources included with this template.
| | |

:::


:::module(module=Skillable&#32Optimizations)

### Skillable Optimizations

For more information, see the [Optimization](https://docs.skillable.com/docs/skillable-virtual-machine-optimization-recommendations) documentation.

:::


:::module(module=Software&#32Licensing)

### Software Licensing

Skillable can optionally provide license activation for certain operating systems or software under Microsoft's SPLA program. If you do not have an agreement with Skillable under this program or with Microsoft directly, all other licensing is the responsibility of the user of this template. 

For more information, see the [Windows licensing](https://docs.skillable.com/docs/windows-licensing) documentation.

:::


:::module(module=Using&#32this&#32Template)


## Using this Template

>[+]How do I activate Microsoft Windows?
>
>Activating Windows for labs can be achieved one of three ways depending on your use cases:
>
>1. Rearm:  When the software environment is complete.  Opening an administrative command or PowerShell prompt and using the command `slmgr -rearm` will reset the Windows activation clock.  
>1. Use a Multiple Activation Key (MAK): You can add your own Microsoft Windows Product Key to license the Windows software.  This can be added using the Activation tool in Settings
>1. Using a Skillable License:  Skillable can activate and license the Windows VM automatically.  If you have already signed up for a SPLA agreement just ensure the production copies of the Lab Profiles are saved to your **<companyname> - Production - SPLA** organization.  This will automatically license the Windows VM for you.  If you do not have a SPLA agreement, please see the Software Licensing section.

>[+]Any restrictions on the software I can install and use?
>
>Any software that meets Skillable's lab software usage policy and does not contravene the [Terms and Conditions](https://www.skillable.com/company/legal-and-security/terms-and-conditions/) may be installed.

>[+]How do I modify, add content to the environment?
>
>The environment can be modified just like a normal Windows system. Adding software can be achieved in several ways. The size of the application may impact the method you choose. Here are the options, in preferred order to minimize negative impact on the VM's performance:
>
> 1. For applications less than 2GB, use the **Load Files** on the Settings menu 
> 1. For applications greater than 2GB, upload an ISO file into the Skillable storage using the Skillable [Manage Storage tool](https://labondemand.com/Storage) on the Studio Admin page 
> 1. The VM has Internet access, the application can be downloaded from the Internet, best for small applications (few MB's), also use InPrivate/Incognito browsing to leave a minimum browser impact in the VM
>
> If you make any changes to the environment, they are not saved until **committed**. 

>[+]Operating system updates and patches
>
>To ensure optimal performance, Windows software updating (including applications) using the Windows Update service is disabled. This environment and its applications were updated based on the published date unless otherwise noted in the [software and updates](#software-and-updates) section.
>
>If you wish to install additional updates you may do so manually, or enable Windows Update by reversing the instructions in the [Skillable optimization documentation](https://docs.skillable.com/docs/skillable-virtual-machine-optimization-recommendations) .
>
>If you enable Windows Update, it is highly recommended that you follow the same instructions to disable it before committing changes to the lab.

>[+] Committing changes to the Lab Profile
>
> If you have made changes to the environment and those changes need to persist, they have to be committed (saved).  If the running lab is ended without saving all modifications to the environment will be lost.
>
>To commit/save the changes, from the Settings menu, choose the **Commit Changes** option and follow the instructions.




<br>
> [!knowledge] For more information, review the documentation on [Template Gallery](https://docs.skillable.com/docs/template-gallery)

:::

:::module(module=Scoring&#32this&#32Template)

### Scoring this Template

Skillable labs offer robust capabilities to validate user performance in software environments through a feature called Automated Activities. For detailed information with examples can be reviewed on our [Validating Skills](https://docs.skillable.com/docs/pbt-overview) documentation page.

In Windows-based environments, we recommend using PowerShell as the scripting language. Skillable also provides tools including the Scripting Copilot and Script Library to get you started.

- Skillable Copilot:  Enables you to use AI to create the script for you
- The Script Library: Contains customizable example scripts to streamline script creation.

:::
