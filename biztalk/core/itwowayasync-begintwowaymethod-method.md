---
title: "ITwoWayAsync.BeginTwoWayMethod Method | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 0d8358f5-caf2-4209-b787-e490fe53d05f
caps.latest.revision: 5
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# ITwoWayAsync.BeginTwoWayMethod Method
Asynchronously processes messages incoming through the WCF request-response receive locations.  
  
> [!WARNING]
>  This topic is provided for information only. You can use this information to interpret the instances that WCF performance counters create for the WCF adapters and the auto-generated metadata for the WCF adapters. Do not rely on this information when you create applications.  
  
## Method Declaration  
  
```  
[OperationContract(AsyncPattern = true, IsOneWay = false, Action = "*", ReplyAction = "*")]  
IAsyncResult BeginTwoWayMethod(Message message, AsyncCallback callback, object state);  
```  
  
## Parameters  
 `message`  
 Message object constraining the WCF request message.  
  
 `callback`  
 Callback object indicating the method to be called when the corresponding asynchronous operation completes.  
  
 `state`  
 User-defined object that qualifies or contains information about the asynchronous operation.  
  
## Return Value  
 This method returns the status of the asynchronous operation.  
  
## See Also  
 [ITwoWayAsync.EndTwoWayMethod Method](../core/itwowayasync-endtwowaymethod-method.md)