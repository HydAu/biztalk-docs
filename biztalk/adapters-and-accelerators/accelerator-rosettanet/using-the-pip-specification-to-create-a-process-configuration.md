---
title: "Using the PIP Specification to Create a Process Configuration | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server-2013"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "PIPs, PIP settings"
  - "PIPs, PIP secifications"
  - "process configuration, PIPs"
  - "PIPs, process configuration"
ms.assetid: 64f0f5fb-f880-4ef1-95d7-2575b8d0bcff
caps.latest.revision: 4
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Using the PIP Specification to Create a Process Configuration
After you download a Partner Interface Process (PIP) from the RosettaNet organization (from RosettaNet.org), the download package includes a PIP specification document. This document contains guidance on what settings to use when you create a process configuration in the [!INCLUDE[btaBTARNNoVersion](../../includes/btabtarnnoversion-md.md)] Management Console.  
  
## How PIP Settings Map to the PIP Specification  
 The following table describes how PIP settings map to information in the RosettaNet PIP specification.  
  
|Process Configuration setting|Information in the PIP specification|  
|-----------------------------------|------------------------------------------|  
|Process Code|Subheading on the title page, for example, "PIP3A4"|  
|Version|PIP Version Identifier subheading on the title page, for example, "02.02.00"|  
|Process name|Subheading on the title page, for example, "Request Purchase Order"|  
|Description (General tab)|Section 3.1, Business Process Definition|  
|Non-Repudiation Required|Table 3-3: Business Activity Performance Controls|  
|Time to Acknowledge (Seconds)|Table 3-3: Business Activity Performance Controls|  
|Is Authorization Required?|Table 3-3: Business Activity Performance Controls|  
|Is Persistent Confidentiality Required|(No reference from the PIP specification)|  
|Is Secure Transport Required?|Table 4-3: Message Exchange Controls|  
|Is Single Action|Section 4.3, Business Transaction Dialog Specification|  
|Non-Repudiation of Origin and Content|Table 3-3: Business Activity Performance Controls|  
|Retry Count|Table 3-3: Business Activity Performance Controls|  
|Time to Perform|Table 3-3: Business Activity Performance Controls|  
|Name|Table 3-3: Business Activity Performance Controls (Activity Name)|  
|Type|(No reference from the PIP specification - for future use)|  
|Description (Initiator and Response tabs)|Table 3-4: PIP Business Documents|  
|Name (Initiator and Response tabs)|Table 3-4: PIP Business Documents|  
|Role (Initiator and Response tabs)|Table 3-1: Partner Role Descriptions|  
|Role Description (Initiator and Response tabs)|Table 3-1: Partner Role Descriptions|  
|Role Type (Initiator and Response tabs)|Table 3-1: Partner Role Descriptions|  
|Service|Table 4-1: Network Component Specification|  
|Service Classification|Table 4-1: Network Component Specification|  
  
## See Also  
 [How to Create or Edit a Process Configuration](../../adapters-and-accelerators/accelerator-rosettanet/how-to-create-or-edit-a-process-configuration.md)