---
title: 公共语言运行时中的 ETW 事件
ms.date: 03/30/2017
helpviewer_keywords:
- CLR ETW events
- ETW, common language runtime
- ETW, CLR events
ms.assetid: 5bb9b6a2-7b57-4aea-8809-32b28bc73e88
author: mairaw
ms.author: mairaw
ms.openlocfilehash: 1d059a5d4df402b309f628bf3e9393114c4cdeec
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61723181"
---
# <a name="etw-events-in-the-common-language-runtime"></a>公共语言运行时中的 ETW 事件
公共语言运行时 (CLR) 通过大量的调试和分析事件，提供有用的 Windows 事件跟踪 (ETW) 诊断信息。 CLR ETW 事件利用 Windows ETW 跟踪系统来扩充公共语言运行时所提供的现有分析和调试支持。  
  
 有关 ETW 的详细信息，请参阅 MSDN 上的[使用 ETW 改善调试和性能优化](https://go.microsoft.com/fwlink/?LinkID=161142)一文。 有关 Xperf 的详细信息，请参阅 NTDebugging 博客中的 [Windows Performance Toolkit - Xperf](https://go.microsoft.com/fwlink/?LinkID=161144)（Windows 性能工具包 - Xperf）。  
  
 在事件主题中介绍的所有事件要求 [!INCLUDE[net_v40_long](../../../includes/net-v40-long-md.md)] 或更新版本。 Windows Vista 操作系统是支持的最低客户端，而 Windows Server 2008 是支持的最低服务器。  
  
## <a name="in-this-section"></a>本节内容  
 [控制 .NET Framework 日志记录](../../../docs/framework/performance/controlling-logging.md)  
 介绍用于捕获和查看 ETW 事件的工具和命令。  
  
 [CLR ETW 提供程序](../../../docs/framework/performance/clr-etw-providers.md)  
 提供有关运行时和断开提供程序，以及如何使用它们收集 ETW 数据的信息。  
  
 [CLR ETW 关键字和级别](../../../docs/framework/performance/clr-etw-keywords-and-levels.md)  
 介绍运行时和断开提供程序的关键字，可通过这些关键字按类别筛选事件。  
  
 [CLR ETW 事件](../../../docs/framework/performance/clr-etw-events.md)  
 提供有关 CLR ETW 事件及其关键字、级别和事件数据的详细信息。  
  
## <a name="see-also"></a>请参阅

- [.NET Framework 中的 ETW 事件](../../../docs/framework/performance/etw-events.md)
