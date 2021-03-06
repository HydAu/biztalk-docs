---
title: "MSBTS_SendHandler.CustomCfg Property (WMI) | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 91688ee0-8715-41be-b02a-adf386e5e090
caps.latest.revision: 8
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# MSBTS_SendHandler.CustomCfg Property (WMI)
Contains the adapter-specific configuration in XML format.  
  
 *The syntax shown is language neutral.*  
  
## Syntax  
  
```  
  
string CustomCfg;  
```  
  
## Remarks  
 An empty value indicates that the adapter lacks some important information and will not function correctly.  
  
 This property is optional.  
  
 This property is read-write.  
  
 For more information about the configuring the receive location of any of the native adapters, see the following topics:  
  
-   [Configuring a File Send Handler](http://msdn.microsoft.com/library/9b0bda92-28f7-4d85-af95-3c59e83b3bb0)  
  
-   [Configuring an FTP Send Handler](http://msdn.microsoft.com/library/8d41e23f-0e7d-49b1-8698-30408e91349c)  
  
-   [Configuring an HTTP Send Handler](../core/how-to-configure-an-http-send-handler.md)  
  
-   [Configuring an SMTP Send Handler By Using BizTalk Explorer](../core/how-to-configure-an-smtp-send-handler.md)  
  
-   [Configuring a SOAP Send Handler](../core/how-to-configure-a-soap-send-handler.md)  
  
## Requirements  
 **Header:** Declared in BTSWMISchema2K.mof or BTSWMISchemaXP.mof.  
  
 **Namespace:** Included in \root\MicrosoftBizTalkServer.