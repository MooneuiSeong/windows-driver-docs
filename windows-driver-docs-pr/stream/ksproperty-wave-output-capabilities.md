---
title: KSPROPERTY\_WAVE\_OUTPUT\_CAPABILITIES
description: The KSPROPERTY\_WAVE\_OUTPUT\_CAPABILITIES property returns a wave device's wave output capabilities.
ms.assetid: 9e5e8ed1-0d08-45b7-b683-df7ce4424c26
keywords: ["KSPROPERTY_WAVE_OUTPUT_CAPABILITIES Streaming Media Devices"]
topic_type:
- apiref
api_name:
- KSPROPERTY_WAVE_OUTPUT_CAPABILITIES
api_location:
- ksmedia.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# KSPROPERTY\_WAVE\_OUTPUT\_CAPABILITIES


The KSPROPERTY\_WAVE\_OUTPUT\_CAPABILITIES property returns a wave device's wave output capabilities.

## <span id="ddk_ksproperty_wave_output_capabilities_ks"></span><span id="DDK_KSPROPERTY_WAVE_OUTPUT_CAPABILITIES_KS"></span>


### <span id="Usage_Summary_Table"></span><span id="usage_summary_table"></span><span id="USAGE_SUMMARY_TABLE"></span>Usage Summary Table

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Get</th>
<th>Set</th>
<th>Target</th>
<th>Property descriptor type</th>
<th>Property value type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Yes</p></td>
<td><p>No</p></td>
<td><p>Pin</p></td>
<td><p>[<strong>KSPROPERTY</strong>](https://msdn.microsoft.com/library/windows/hardware/ff564262)</p></td>
<td><p>[<strong>KSWAVE_OUTPUT_CAPABILITIES</strong>](https://msdn.microsoft.com/library/windows/hardware/ff567248)</p></td>
</tr>
</tbody>
</table>

 

The property value (operation data) is a KSWAVE\_OUTPUT\_CAPABILITIES structure that describes the output capabilities of a wave device, including the maximum number of audio channels, the range of bits per sample, the range of sampling frequency, the total and active number of connections.

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
<td>Ksmedia.h (include Ksmedia.h)</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[**KSPROPERTY**](https://msdn.microsoft.com/library/windows/hardware/ff564262)

[**KSWAVE\_OUTPUT\_CAPABILITIES**](https://msdn.microsoft.com/library/windows/hardware/ff567248)

 

 






