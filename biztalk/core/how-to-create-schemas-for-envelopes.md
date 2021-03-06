---
title: "How to Create Schemas for Envelopes | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: ae1c991c-447f-497e-803c-1cb8cad2846b
caps.latest.revision: 7
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# How to Create Schemas for Envelopes
After creating an XML message schema as described in [Creating Schemas for XML Messages](../core/how-to-create-schemas-for-xml-messages.md), set the [Envelope](../core/envelope-node-property-of-all-schemas.md) property of the **Schema** node to **Yes**. Depending on certain characteristics of your envelope schema, such as whether there are multiple root nodes, you will need to set several other envelope-specific properties. For more information, see [Envelope Schemas](../core/envelope-schemas.md).  
  
 The body XPath property of the envelope points to the element that contains the document elements. The actual element where the XPath points to does not belong to the document.  
  
## See Also  
 [Managing Schemas Within Projects](../core/managing-schemas-within-projects.md)