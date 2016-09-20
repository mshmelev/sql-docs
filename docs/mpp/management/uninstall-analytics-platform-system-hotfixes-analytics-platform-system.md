---
title: "Uninstall Analytics Platform System Hotfixes (Analytics Platform System)"
ms.custom: na
ms.date: 07/27/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: c9ab596d-3f5a-48e2-bce7-c9be99b8c23b
caps.latest.revision: 21
author: BarbKess
---
# Uninstall Analytics Platform System Hotfixes (Analytics Platform System)
The following steps describe how to uninstall a previously installed Analytics Platform System hotfix.  
  
## Before You Begin  
  
### Prerequisites  
To perform these steps, you will need:  
  
-   An Analytics Platform System login with permissions to access the Admin Console to monitor the appliance.  
  
-   The Domain Administrator account to login to the *<appliance_domain>***-HST01** node.  
  
-   The Knowledge Base article number for the hotfix to uninstall.  
  
## <a name="HowToUninstallPDW"></a>To uninstall a SQL Server PDW hotfix  
  
1.  Log on to the *<appliance_domain>***-HST01** node as the Fabric Domain Administrator.  
  
2.  Use the Run as Administrator option to open a Command Prompt.  
  
3.  Change directories to `C:\PDWINST\Patches\<kbarticle>\media` where *<kbarticle>* is the Knowledge Base article number for the hotfix to uninstall.  
  
    ```  
    cd /d c:\PDWINST\Patches\<kbarticle>\media  
    ```  
  
4.  To remove the hotfix, run the following command.  
  
    ```  
    setup.exe /action="removepatch" /DomainAdminPassword="<password>"  
    ```  
  
## See Also  
[Download and Apply Microsoft Updates &#40;Analytics Platform System&#41;](../../mpp/management/download-and-apply-microsoft-updates-analytics-platform-system.md)  
[Uninstall Microsoft Updates &#40;Analytics Platform System&#41;](../../mpp/management/uninstall-microsoft-updates-analytics-platform-system.md)  
[Apply Analytics Platform System Hotfixes &#40;Analytics Platform System&#41;](../../mpp/management/apply-analytics-platform-system-hotfixes-analytics-platform-system.md)  
[Software Servicing &#40;Analytics Platform System&#41;](../../mpp/management/software-servicing-analytics-platform-system.md)  
  