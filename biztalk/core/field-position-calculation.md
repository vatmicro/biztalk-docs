---
title: "Field Position Calculation | Microsoft Docs"
ms.custom: ""
ms.date: "06/08/2017"
ms.prod: "biztalk-server"
ms.reviewer: ""
ms.service: "biztalk-server"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 7e315f09-f2c9-49cc-8d2f-0f4f2d48fd45
caps.latest.revision: 7
author: "MandiOhlinger"
ms.author: "mandia"
manager: "anneta"
---
# Field Position Calculation
When you use the [Positional Length](../core/positional-length-node-property-of-flat-file-schemas.md) and [Positional Offset](../core/positional-offset-node-property-of-flat-file-schemas.md) properties of the **Field Element** and **Field Attribute** nodes in your schema to define the layout of the positional records in your flat file message, the **Start Position** and **Length** columns of the **Flat File** tab in BizTalk Editor show the calculated starting positions and lengths, respectively, of the relevant fields and records.  
  
> [!NOTE]
>  The **Flat File** tab appear as an alternate tabbed view with the XSD view in BizTalk Editor when you have configured the flat file extension using the [Schema Editor Extensions](../core/schema-editor-extensions-node-property-of-all-schemas.md) property of the **Schema** node.  
  
 In general, the starting position of a particular field *N* is the starting position of the previous field, plus the length of the previous field, plus the (positional) offset you have specified for field *N*.  
  
 All field position calculation in Microsoft [!INCLUDE[btsBizTalkServerNoVersion](../includes/btsbiztalkservernoversion-md.md)] is performed automatically, on-the-fly, without any need to execute a command (as was required in previous versions of BizTalk Server).  
  
## See Also  
 [Positional Record Considerations](../core/positional-record-considerations.md)   
 [Positional Length (Node Property of Flat File Schemas)](../core/positional-length-node-property-of-flat-file-schemas.md)   
 [Positional Offset (Node Property of Flat File Schemas)](../core/positional-offset-node-property-of-flat-file-schemas.md)