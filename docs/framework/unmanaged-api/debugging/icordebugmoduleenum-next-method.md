---
title: "ICorDebugModuleEnum::Next Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ICorDebugModuleEnum.Next"
apilocation: 
  - "mscordbi.dll"
apitype: "COM"
f1_keywords: 
  - "ICorDebugModuleEnum::Next"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ICorDebugModuleEnum::Next method [.NET Framework debugging]"
  - "Next method, ICorDebugModuleEnum interface [.NET Framework debugging]"
ms.assetid: 9ff3fcd6-38fe-41f8-bfd3-f0ab6c7d77ca
caps.latest.revision: 10
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# ICorDebugModuleEnum::Next Method
Gets the number of "ICorDebugModule" instances specified by `celt` from the enumeration, starting at the current position.  
  
## Syntax  
  
```  
HRESULT Next (  
    [in]  ULONG celt,  
    [out, size_is(celt), length_is(*pceltFetched)]  
        ICorDebugModule *modules[],  
    [out] ULONG *pceltFetched  
);  
```  
  
#### Parameters  
 `celt`  
 [in] The number of `ICorDebugModule` instances to be retrieved.  
  
 `modules`  
 [out] An array of pointers, each of which points to an `ICorDebugModule` object.  
  
 `pceltFetched`  
 [out] Pointer to the number of `ICorDebugModule` instances actually returned. This value may be null if `celt` is one.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorDebug.idl, CorDebug.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## See Also  
 