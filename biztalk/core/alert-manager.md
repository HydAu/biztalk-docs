---
title: "Alert Manager | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bts06.bam.portal.alertmanager"
ms.assetid: 9a032bd2-ea99-4bc7-8ea2-b253d007c571
caps.latest.revision: 15
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Alert Manager
The alert manager allows you to view available alerts, edit alert details, and subscribe to alerts.  
  
## Alert summary  
 The **Alert Summary** area of the content frame displays a list of the configured alerts. The summary grid contains information about the alert. Clicking a row in the alert summary loads the details of the alert in the Alert Details area of the content frame. You can use this information to determine if the alert meets your needs and if you want subscribe to it. If you are an alert owner you can edit the alert and save it. The following table lists general information about the alert.  
  
|Summary Column|Contents|  
|--------------------|--------------|  
|Name|The name of the alert.|  
|Type|This can be either Aggregate or Individual.|  
|Enabled|Indicates whether the alert is active and can be raised.|  
|Priority|Indicates the severity of the issue the alert is reporting.|  
|Security|An alert is either public or private. Public alerts can be subscribed to by any user. Private alerts can only be subscribed to by alert owners.|  
|Created By|The user who created the alert.|  
|Created Date|The date and time the alert was created.|  
|Last Modified Date|The date and time the alert was last saved.|  
|Is Owner|Indicates whether you are an owner of this alert.|  
  
## Alert details  
 The **Alert Details** area of the Alert Management content frame provides details about the alert. You can use this information to decide if the alert meets your needs. You can also modify the alert from this area. The following table describes the details of an alert.  
  
|Field Name|Contents|  
|----------------|--------------|  
|Name|The name of the alert. The name of the alert is used as the subject of alerts delivered in e-mail and as the file name for alerts delivered as a file. **Note:**  Names are limited to 100 characters. Valid alert names must start with a letter. Following characters can be letters, numbers, a space (' '), or an underscore ('_'). Additionally, there cannot be two consecutive spaces in the name.|  
|Message|The text of the message that will be delivered with the alert.|  
|Priority|Indicates the severity of the issue the alert is reporting. The priority levels are high, medium, and low. For alerts delivered by e-mail this sets the importance flag on the e-mail message.|  
|Owners|The owner of the alert. The default value for the owner is the same as the creator of the alert. Multiple owners are entered as a semi-colon delimited list.|  
|Threshold area|This area of the alert details is only present for aggregation alerts.|  
|Count<br />(Aggregation alert only)|A drop-down list of comparison operations.|  
|Value<br />(Aggregation alert only)|The threshold value to which the comparison applies. The alert is sent only when the value meets the comparison criteria. The alert will not be sent again if monitoring has been reset by the condition no longer being true. An example is where the alert is set such that an order amount of greater than $1,000 is reported. As long as the order amount stays above $1,000 the alert is not sent again. If the order amount falls below $1,000 and then rises above it again, the alert is sent again.|  
|Advanced Query Button|Open the Advanced Query Editor dialog box. The Advance Query Editor uses multidimensional expressions to define the query. This is an advanced feature and should only be used by experienced users. For more information about the multidimensional expressions query language, see the OLE DB Programmer's Reference on MSDN at [http://go.microsoft.com/fwlink/?LinkId=58869](http://go.microsoft.com/fwlink/?LinkId=58869).|  
|Restrict search to the last area|This area of the alert details is only present for aggregation alerts. If the check box is selected the alert is delivered only if the threshold value is reached during the specified time period. If the checkbox is not selected, the alert is delivered when the threshold is reached, regardless of the time period involved. By default the check box is selected when there are time dimensions defined. If there are no time dimensions defined this option is not available.|  
|Based on Dimension<br />(Aggregation alert only)|Specifies a time dimension across which BAM monitors for the threshold value to be reached.|  
|Duration<br />(Aggregation alert only)|A two-part field in which there is a text field that contains a numerical value and a drop-down list specifying the units. The value of the duration must be greater than zero and equal to or less than the duration set on the aggregation when it was created.|  
|Alert Security Area|The security setting area.|  
|Allow others to see this alert and subscribe to it|A check box, that when selected, allows users with permissions to the underlying view to see and subscribe to the alert. Users can remove themselves as a subscriber at any time. Owners of the alert and Database Owners can remove a subscriber at any time.|  
  
### Subscriptions  
 The Subscriptions area of the Alert Management content frame allows you to subscribe to an alert. The following table lists the information you must supply to subscribe to an alert.  
  
|Field Name|Contents|  
|----------------|--------------|  
|User Name|The alias of the user that is subscribing to the alert. This value is automatically set to the current user.|  
|Transport|Indicates how the alert is delivered. The delivery methods are e-mail or a file.|  
|Address|Indicates where the alert will be delivered. This is an e-mail address for e-mail transport or a system-defined file location for a transport method of file. When there are multiple e-mail subscribers to an alert, a single e-mail message is sent to all subscribers allowing any subscriber to reply to all the subscribers and inform them of the resolution.|  
|Add Subscriber Button|Opens the Add Subscriber dialog box.|  
  
## See Also  
 [Search](../core/search.md)