---
title: <metadata>
ms.date: 03/30/2017
ms.assetid: d09653eb-e355-4c73-b87b-28f93d56480d
ms.openlocfilehash: c0c9848d073c799e1f97dd79b375848dfab71e99
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61763901"
---
# <a name="metadata"></a>\<metadata>
指定可以处理服务元数据的方式。  
  
 \<system.ServiceModel>  
\<client>  
  
## <a name="syntax"></a>语法  
  
```xml  
<system.serviceModel>
  <client>
    <metadata>
      <policyImporters>
        <policyImporter type="string" />
      </policyImporters>
      <wsdlImporters>
        <wsdlImporter type="string" />
      </wsdlImporters>
    </metadata>
  </client>
</system.serviceModel>
```  
  
## <a name="attributes-and-elements"></a>特性和元素  
 下列各节描述了特性、子元素和父元素。  
  
### <a name="attributes"></a>特性  
 无。  
  
### <a name="child-elements"></a>子元素  
  
|元素|描述|  
|-------------|-----------------|  
|[\<policyImporters>](../../../../../docs/framework/configure-apps/file-schema/wcf/policyimporters.md)|指定用于控制有关绑定的自定义策略断言的导入的所有策略导入程序。 策略导入程序用于搜索有关绑定功能的自定义策略断言，并附加一个实现断言所需功能的自定义绑定元素。|  
|[\<wsdlImporters>](../../../../../docs/framework/configure-apps/file-schema/wcf/wsdlimporters.md)|指定可导入带有 WS-Policy 附件的 Web 服务描述语言 (WSDL) 1.1 元数据的所有 WSDL 导入程序。 WSDL 导入程序可用于导入元数据并将这些信息转换为各种表示协定和终结点信息的类。 它可以有选择地导入协定和终结点信息以及公开任何导入错误的属性，并接受与导入和转换过程相关的类型信息。 它还支持导入某些绑定信息和属性，这些信息和属性提供了对任何策略文档、WSDL 文档、WSDL 扩展和 XML 架构文档的访问。|  
  
### <a name="parent-elements"></a>父元素  
  
|元素|描述|  
|-------------|-----------------|  
|[\<client>](../../../../../docs/framework/configure-apps/file-schema/wcf/client.md)|client 节定义客户端可以连接的终结点的列表。|  
  
## <a name="see-also"></a>请参阅

- <xref:System.ServiceModel.Configuration.MetadataElement>
- <xref:System.ServiceModel.Configuration.PolicyImporterElementCollection>
- <xref:System.ServiceModel.Configuration.WsdlImporterElementCollection>
- <xref:System.ServiceModel.Description.MetadataImporter>
- <xref:System.ServiceModel.Description.WsdlImporter>
- [WCF 客户端配置](../../../../../docs/framework/wcf/feature-details/client-configuration.md)
- [客户端](../../../../../docs/framework/wcf/feature-details/clients.md)
