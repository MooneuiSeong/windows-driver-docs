---
title: GUIDType (ServiceInfo)
description: GUIDType (ServiceInfo)
ms.assetid: a08d4c7c-c282-4870-b836-6788ffa2d088
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# GUIDType (ServiceInfo)

The GUIDType XML simple type specifies a GUID.

``` syntax
<xs:simpleType name="GUIDType">
  <xs:restriction base="xs:string">
    <xs:pattern value="[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}" />
  </xs:restriction>
</xs:simpleType>
```

## <span id="Patterns"></span><span id="patterns"></span><span id="PATTERNS"></span>Patterns


The GUIDType simple type is a **xs:string** that is restricted by the following pattern:

-   \[0-9a-fA-F\]{8}-\[0-9a-fA-F\]{4}-\[0-9a-fA-F\]{4}-\[0-9a-fA-F\]{4}-\[0-9a-fA-F\]{12}

 

 





