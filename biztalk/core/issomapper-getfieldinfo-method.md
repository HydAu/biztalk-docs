---
title: "ISSOMapper.GetFieldInfo Method | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: bc2a5698-f01c-44d0-b20d-6518d7b1090b
caps.latest.revision: 5
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# ISSOMapper.GetFieldInfo Method
The **GetFieldInfo** method retrieves the field information for an application.  
  
## Syntax  
  
```cpp#  
  
HRESULT GetFieldInfo(  
BSTR bstrApplicationName,  
SAFEARRAY labels,  
SAFEARRAY flags  
);  
```  
  
```vb  
  
Sub GetFieldInfo(  
bstrApplicationName As String,  
labels As String  
flags As Long  
)  
```  
  
#### Parameters  
 `bstrApplicationName`  
 [in]  String that specifies the application name. This parameter cannot be NULL, an empty string, or contain spaces. Application names are not case-sensitive, but case will be preserved. For example, ABC, abc, and AbC are considered to be the same application.  
  
 `bstrApplicationName`  
 [in]  String that specifies the application name. This parameter cannot be NULL, an empty string, or contain spaces. Application names are not case-sensitive, but case will be preserved. For example, ABC, abc, and AbC are considered to be the same application.  
  
 `labels`  
 [out]  String array that returns the field labels.  
  
 `labels`  
 [out]  String array that returns the field labels.  
  
 `flags`  
 [out]  Long integer array that returns the field flags.  
  
 `flags`  
 [out]  Long array that returns the field flags.  
  
## Return Value  
 This method returns an HRESULT indicating whether it completed successfully. For more details, see the Error Values section.  
  
 Not applicable.  
  
## Error Values  
 This method returns an HRESULT containing one of the values in the following table.  
  
 This method indicates errors by setting the **Number** property of the global **Err** object to one of the values in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|S_OK|The method succeeded.|  
|E_ACCESSDENIED|Access is denied to the caller.|  
|E_FAIL|The application is disabled.|  
|E_INVALIDARG|An invalid parameter was detected.|  
  
## Remarks  
 The field information will only be returned if the application is currently enabled. An application cannot be enabled unless its field information is complete.  
  
## Requirements  
 **Platforms:**  [!INCLUDE[btsPlatformsComApis](../includes/btsplatformscomapis-md.md)]  
  
## See Also  
 [ISSOMapper Interface (COM)](../core/issomapper-interface-com.md)   
 [ISSOMapper Members](../core/issomapper-members.md)   
 [Programming with Enterprise Single Sign-On](../core/programming-with-enterprise-single-sign-on.md)