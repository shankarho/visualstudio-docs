---
title: "IDebugPortSupplier2::GetPort | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: 
  - "vs-ide-sdk"
ms.topic: "conceptual"
f1_keywords: 
  - "IDebugPortSupplier2::GetPort"
helpviewer_keywords: 
  - "IDebugPortSupplier2::GetPort"
ms.assetid: d55d5055-7386-4037-bf22-4c3e434a99ca
author: "gregvanl"
ms.author: "gregvanl"
manager: douge
ms.workload: 
  - "vssdk"
---
# IDebugPortSupplier2::GetPort
Gets a port from a port supplier.  
  
## Syntax  
  
```cpp  
HRESULT GetPort(   
   REFGUID       guidPort,  
   IDebugPort2** ppPort  
);  
```  
  
```csharp  
int GetPort(   
   ref Guid        guidPort,  
   out IDebugPort2 ppPort  
);  
```  
  
#### Parameters  
 `guidPort`  
 [in] Globally unique identifier (GUID) of the port.  
  
 `ppPort`  
 [out] Returns an [IDebugPort2](../../../extensibility/debugger/reference/idebugport2.md) object that represents the port.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code. Returns `E_PORTSUPPLIER_NO_PORT` if no port exists with the given identifier.  
  
## See Also  
 [IDebugPortSupplier2](../../../extensibility/debugger/reference/idebugportsupplier2.md)   
 [IDebugPort2](../../../extensibility/debugger/reference/idebugport2.md)