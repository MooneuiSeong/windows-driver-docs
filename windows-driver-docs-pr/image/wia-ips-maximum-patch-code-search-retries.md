---
title: WIA\_IPS\_MAXIMUM\_PATCH\_CODE\_SEARCH\_RETRIES
description: The WIA\_IPS\_MAXIMUM\_PATCH\_CODE\_SEARCH\_RETRIES property describes the maximum number of retries the reader attempts if no patch code can be found when patch code detection is enabled.
ms.assetid: F6CBEC7E-B44D-4524-9F75-8CBF413FCAF6
keywords: ["WIA_IPS_MAXIMUM_PATCH_CODE_SEARCH_RETRIES Imaging Devices"]
topic_type:
- apiref
api_name:
- WIA_IPS_MAXIMUM_PATCH_CODE_SEARCH_RETRIES
api_location:
- Wiadef.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# WIA\_IPS\_MAXIMUM\_PATCH\_CODE\_SEARCH\_RETRIES


The **WIA\_IPS\_MAXIMUM\_PATCH\_CODE\_SEARCH\_RETRIES** property describes the maximum number of retries the reader attempts if no patch code can be found when patch code detection is enabled.

## <span id="ddk_wia_ipa_depth_si"></span><span id="DDK_WIA_IPA_DEPTH_SI"></span>


Property Type: VT\_I4

Valid Values: WIA\_PROP\_RANGE

Access Rights: Read/Write

Remarks
-------

This property is required for all Patch Code Reader items. The property can be implemented to support a range containing one single value, including 0 (no retries).

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Header</p></td>
<td>Wiadef.h (include Wiadef.h)</td>
</tr>
</tbody>
</table>

 

 





