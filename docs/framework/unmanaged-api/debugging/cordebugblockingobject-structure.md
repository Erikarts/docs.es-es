---
title: CorDebugBlockingObject (Estructura)
ms.date: 03/30/2017
api_name:
- CorDebugBlockingObject Structure
api_location:
- mscordbi.dll
api_type:
- COM
f1_keywords:
- CorDebugBlockingObject
helpviewer_keywords:
- CorDebugBlockingObject structure [.NET Framework debugging]
ms.assetid: 5944edd1-0914-4efa-aba0-d5a277c38b1a
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 49521e4b4ff5f8c364827b233759e163aca43e39
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/23/2019
ms.locfileid: "54542666"
---
# <a name="cordebugblockingobject-structure"></a>CorDebugBlockingObject (Estructura)
Define un objeto que está bloqueando un subproceso y el motivo específico que el subproceso está bloqueado.  
  
## <a name="syntax"></a>Sintaxis  
  
```  
Typedef struct CorDebugBlockingObject  
{  
ICorDebugValue pBlockingObject;  
DWORD dwTimeout;  
CorDebugBlockingReason blockingReason;  
}  CorDebugBlockingObject;  
```  
  
## <a name="members"></a>Miembros  
  
|Miembro|Descripción|  
|------------|-----------------|  
|`pBlockingObject`|El objeto en el que está bloqueando el subproceso. Este objeto es válido solo durante el tiempo que dure el estado sincronizado actual. Si dos subprocesos bloqueados en el mismo objeto dentro del mismo estado sincronizado, es posible que espera el [GetAddress](../../../../docs/framework/unmanaged-api/debugging/icordebugvalue-getaddress-method.md) método para devolver el mismo valor. Sin embargo, las interfaces pueden o no sea el equivalente de puntero.|  
|`dwTimeout`|El número de milisegundos antes de la operación de bloqueo superará el tiempo de espera o el valor infinito, lo que indica que superará el tiempo de espera. El valor de tiempo de espera especifica la longitud total de tiempo para la operación de bloqueo, no el tiempo que queda todavía.|  
|`blockingReason`|El motivo de que el subproceso está bloqueado en este objeto.|  
  
## <a name="remarks"></a>Comentarios  
  
## <a name="requirements"></a>Requisitos  
 **Plataformas:** Consulte [Requisitos del sistema](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Encabezado**: CorDebug.idl  
  
 **Biblioteca:** CorGuids.lib  
  
 **Versiones de .NET Framework:** [!INCLUDE[net_current_v40plus](../../../../includes/net-current-v40plus-md.md)]  
  
## <a name="see-also"></a>Vea también
- [Estructuras de depuración](../../../../docs/framework/unmanaged-api/debugging/debugging-structures.md)
- [Depuración](../../../../docs/framework/unmanaged-api/debugging/index.md)
