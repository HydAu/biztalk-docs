---
title: "Get batch activation status text xml | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "managed-reference"
ms.assetid: 2160bea5-5e8e-434a-adf5-01ff5620924c
caps.latest.revision: 2
author: "tordgladnordahl"
ms.author: "tonordah"
manager: "anneta"
---
# Get batch activation status: text/xml
## Get batch activation status

  Response Content Type: **text/xml**

Request
---
Response Class (Status 200)

string

Parameters
---


Parameter|Value|Description|Parameter Type|Data Type 
---------|---------|---------|---------|---------
senderParty|(required)|The sender of the agreement.|path|string| 
receiverParty|(required)|The receiver of the agreement.|path|string| 
agreementName|(required)|The agreement name.|path|string| 
batchName|(required)|The batch name.|path|string| 
 
