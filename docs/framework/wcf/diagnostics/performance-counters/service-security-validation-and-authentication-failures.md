---
title: 服务：Security Validation and Authentication Failures（安全验证和身份验证失败次数）
ms.date: 03/30/2017
ms.assetid: 55c98268-b1ad-459d-851b-25ef52248187
ms.openlocfilehash: ba8da3ae6be6bd089690359f19e153da1e0b54fc
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61998304"
---
# <a name="service-security-validation-and-authentication-failures"></a>服务：Security Validation and Authentication Failures（安全验证和身份验证失败次数）
计数器名称：Security Validation and Authentication Failures（安全验证和身份验证失败次数）  
  
## <a name="description"></a>描述  
 每当消息由于“Security Calls Not Authorized”（未授权的安全调用次数）计数器中未包括的安全问题而遭到拒绝时，此计数器即会递增。 此类问题包括：  
  
- 无法从消息中读取客户端令牌。  
  
- 客户端令牌身份验证失败（如密码错误）。  
  
- 签名验证失败（如消息已被篡改）。  
  
- 消息与上一条消息重复，这种情况可能在重放攻击过程中发生。  
  
- 已发生解密失败。  
  
- 消息中缺少一些必需元素（如缺少时间戳或加密的数据块）。  
  
- TLSNEGO/SPNEGO 握手过程中已发生错误。
