---
title: "Creates a business profile for a party text json | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: 8e80a7fe-972e-4172-9fbe-ad86dada0263
caps.latest.revision: 2
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Creates a business profile for a party: text/json
## Creates a business profile for a party

  Response Content Type: **text/json**


Parameters
---



Parameter|Value|Description|Parameter Type|Data Type 
---------|---------|---------|---------|---------
businessProfile|(required)|The business profile.|body|        | 
partyName|(required)|Party name.|path|string| 


Response Messages
---



HTTP Status Code|Reason|Response Model|Headers  
---------|---------|---------|---------
204|No Content |         |        | 

Example Value
---

```
{
  "Name": "string",
  "Description": "string",
  "BusinessIdentities": [
    {
      "Description": "string",
      "Qualifier": "string",
      "Value": "string",
      "Id": 0
    }
  ],
  "CustomSettings": [
    {
      "Name": "string",
      "Value": "string"
    }
  ]
}
```