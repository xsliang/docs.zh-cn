---
title: 参数不能为 Nothing
ms.date: 07/20/2015
f1_keywords:
- vbrGeneral_ArgumentNullException
ms.assetid: 2abd995b-36a5-45f0-b3c1-6e0c3b31a875
ms.openlocfilehash: 38083848927ff0242ba6e0712c390a3516743967
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61977192"
---
# <a name="argument-cannot-be-nothing"></a>参数不能为 Nothing
向必须具有值的参数提供了 null 值。  
  
## <a name="to-correct-this-error"></a>更正此错误  
  
- 你可能试图在未先提供对象的实例的情况下使用对象。 在这种情况下，请使用 `New` 关键字创建实例。  
  
- 检查值是否计算正确。  
  
## <a name="see-also"></a>请参阅

- <xref:System.NullReferenceException>
