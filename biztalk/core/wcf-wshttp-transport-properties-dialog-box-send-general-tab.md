---
title: "WCF-WSHttp Transport Properties Dialog Box, Send, General Tab | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "bts10.adapters.wcf-wshttp.transport.send.general"
helpviewer_keywords: 
  - "WCF-WSHttp adapters, properties"
  - "properties, WCF-WSHttp adapters"
ms.assetid: 634478b3-1f5a-4ef0-bbbd-970e3e7381d3
caps.latest.revision: 18
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# WCF-WSHttp Transport Properties Dialog Box, Send, General Tab
Use the **General** tab to configure the endpoint address, the service identity, and the **SOAP Action** header for the WCF-WSHttp send port.  
  
|Use this|To do this|  
|--------------|----------------|  
|**Address (URI)**|Required. Specify the fully qualified URI for this send port. Use the **https** or the **http** scheme depending on the security configuration. **Note:**  If you specify the **https** scheme for the **Address** property, you must configure the **Security mode** property to **Transport** or **TransportWithMessageCredential**. You can use the **Security** tab to configure the **Security mode** property. <br /><br /> Maximum length: 255<br /><br /> Default value: http://localhost/|  
|**Endpoint Identity**|Optional. Specify the identity of the service that this send port expects. These settings enable this send port to authenticate the service. In the handshake process between the client and service, the Windows Communication Foundation (WCF) infrastructure will ensure that the identity of the expected service matches the values of this element. The values that can be specified for the **Endpoint identity** property differ according to the security configuration.<br /><br /> The default value is cleared.|  
|**Action**|Specify the **SOAPAction** HTTP header field for outgoing messages. This property can also be set through the message context property **WCF.Action** in a pipeline or orchestration. You can specify this value in two different ways: the single action format and the action mapping format. If you set this property in the single action format- for example, http://contoso.com/Svc/Op1- the **SOAPAction** header for outgoing messages is always set to the value specified in this property.<br /><br /> If you set this property in the action mapping format, the outgoing **SOAPAction** header is determined by the **BTS.Operation** context property. For example, if this property is set to the following XML format and the **BTS.Operation** property is set to Op1, the WCF send adapter uses http://contoso.com/Svc/Op1 for the outgoing **SOAPAction** header.<br /><br /> \<BtsActionMapping><br /><br /> \<Operation Name="Op1" Action="http://contoso.com/Svc/Op1" /><br /><br /> \<Operation Name="Op2" Action="http://contoso.com/Svc/Op2" /><br /><br /> \</BtsActionMapping><br /><br /> If outgoing messages comes from an orchestration port, orchestration instances dynamically set the **BTS.Operation** property with the operation name of the port. If outgoing messages are routed with content-based routing, you can set the **BTS.Operation** property in pipeline components.<br /><br /> Minimum length: 0<br /><br /> Maximum length: 32767<br /><br /> The default is an empty string.|  
  
## See Also  
 [The \<identity> element](http://go.microsoft.com/fwlink/?LinkID=75747)   
 [How to Configure a WCF-WSHttp Send Port](../core/how-to-configure-a-wcf-wshttp-send-port.md)   
 [WCF Adapters Property Schema and Properties](../core/wcf-adapters-property-schema-and-properties.md)   
 [Configuring Dynamic Send Ports Using WCF Adapters Context Properties](../core/configuring-dynamic-send-ports-using-wcf-adapters-context-properties.md)