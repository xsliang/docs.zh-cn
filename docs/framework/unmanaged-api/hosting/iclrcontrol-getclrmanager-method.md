---
title: ICLRControl::GetCLRManager 方法
ms.date: 03/30/2017
api_name:
- ICLRControl.GetCLRManager
api_location:
- mscoree.dll
api_type:
- COM
f1_keywords:
- ICLRControl::GetCLRManager
helpviewer_keywords:
- GetCLRManager method [.NET Framework hosting]
- ICLRControl::GetCLRManager method [.NET Framework hosting]
ms.assetid: 8a11bfa4-cbb0-4082-82b5-f9fba66c93f5
topic_type:
- apiref
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 09079c8847b7cb995d97a4577d03982602bbadfa
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61969892"
---
# <a name="iclrcontrolgetclrmanager-method"></a>ICLRControl::GetCLRManager 方法
到任何主机可用于配置公共语言运行时 (CLR) 管理器类型的实例获取的接口指针。  
  
## <a name="syntax"></a>语法  
  
```  
HRESULT GetCLRManager (  
    [in]  REFIID  riid,  
    [out] void  **ppObject  
);  
```  
  
## <a name="parameters"></a>参数  
 `riid`  
 [in]`IID`要返回的管理器类型。 以下`IID`支持值。  
  
- IID_ICLRDebugManager:指定的`ppObject`的类型将为[ICLRDebugManager](../../../../docs/framework/unmanaged-api/hosting/iclrdebugmanager-interface.md)。  
  
- IID_ICLRErrorReportingManager:指定的`ppObject`的类型将为[ICLRErrorReportingManager](../../../../docs/framework/unmanaged-api/hosting/iclrerrorreportingmanager-interface.md)。  
  
- IID_ICLRGCManager:指定的`ppObject`的类型将为[ICLRGCManager](../../../../docs/framework/unmanaged-api/hosting/iclrgcmanager-interface.md)。  
  
- IID_ICLRHostProtectionManager:指定的`ppObject`的类型将为[ICLRHostProtectionManager](../../../../docs/framework/unmanaged-api/hosting/iclrhostprotectionmanager-interface.md)。  
  
- IID_ICLROnEventManager:指定的`ppObject`的类型将为[ICLROnEventManager](../../../../docs/framework/unmanaged-api/hosting/iclroneventmanager-interface.md)。  
  
- IID_ICLRPolicyManager:指定的`ppObject`的类型将为[ICLRPolicyManager](../../../../docs/framework/unmanaged-api/hosting/iclrpolicymanager-interface.md)。  
  
- IID_ICLRTaskManager:指定的`ppObject`的类型将为[ICLRTaskManager](../../../../docs/framework/unmanaged-api/hosting/iclrtaskmanager-interface.md)。  
  
 `ppObject`  
 [out]请求管理器中或为空，如果请求无效的管理器类型的接口指针。  
  
## <a name="return-value"></a>返回值  
  
|HRESULT|描述|  
|-------------|-----------------|  
|S_OK|该方法成功返回。|  
|HOST_E_CLRNOTAVAILABLE|CLR 尚未加载到进程中，或处于不能运行托管的代码或已成功处理调用的状态。|  
|HOST_E_TIMEOUT|呼叫已超时。|  
|HOST_E_NOT_OWNER|调用方不拥有该锁。|  
|HOST_E_ABANDONED|事件已取消时被阻塞的线程或纤程正在等待它。|  
|E_FAIL|发生未知的灾难性故障。 方法返回 E_FAIL 后，CLR 不再在进程中使用。 对托管方法的后续调用返回 HOST_E_CLRNOTAVAILABLE。|  
|E_NOINTERFACE|不支持的接口类型。|  
  
## <a name="requirements"></a>要求  
 **平台：** 请参阅[系统需求](../../../../docs/framework/get-started/system-requirements.md)。  
  
 **标头：** MSCorEE.h  
  
 **库：** 包含为 MSCorEE.dll 中的资源  
  
 **.NET Framework 版本：**[!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]  
  
## <a name="see-also"></a>请参阅

- [ICLRControl 接口](../../../../docs/framework/unmanaged-api/hosting/iclrcontrol-interface.md)
- [IHostControl 接口](../../../../docs/framework/unmanaged-api/hosting/ihostcontrol-interface.md)
