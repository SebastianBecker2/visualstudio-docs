---
title: "IScriptEntry::SetSignature | Microsoft Docs"
ms.custom: ""
ms.date: "01/18/2017"
ms.prod: "windows-script-interfaces"
ms.reviewer: ""
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "IScriptEntry.SetSignature"
apilocation: 
  - "scrobj.dll"
helpviewer_keywords: 
  - "IScriptEntry::SetSignature"
ms.assetid: 8513587d-9df2-4621-afe7-56eacbb5e688
caps.latest.revision: 11
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IScriptEntry::SetSignature
Sets type information for an `IScriptEntry` function object.  
  
## Syntax  
  
```  
HRESULT SetSignature(  
   ITypeInfo          *pti  
   ULONG              iMethod  
);  
```  
  
#### Parameters  
 `pti`  
 [in] The type information.  
  
 `iMethod`  
 [in] The method index in the `ITypeInfo` object.  
  
## Return Value  
 An `HRESULT`. Possible values include, but are not limited to, those in the following table.  
  
|Value|Description|  
|-----------|-----------------|  
|`S_OK`|The method succeeded.|  
  
## Remarks  
 You set type information by using `IScriptEntry::SetSignature` or [IScriptNode::CreateChildHandler](../../winscript/reference/iscriptnode-createchildhandler.md). Type information can also be generated by the entry based on the internal function representation.  
  
## See Also  
 [IScriptEntry Interface](../../winscript/reference/iscriptentry-interface.md)