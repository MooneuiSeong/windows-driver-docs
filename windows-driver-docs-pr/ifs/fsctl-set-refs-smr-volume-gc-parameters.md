---
title: FSCTL\_SET\_REFS\_SMR\_VOLUME\_GC\_PARAMETERS control code
description: The FSCTL\_SET\_REFS\_SMR\_VOLUME\_GC\_PARAMETERS control code controls the garbage collection on a Shingled Magnetic Recording (SMR) volume.
ms.assetid: 782542C4-CFC5-4BF7-AF38-3247A3AC6AB9
keywords: ["FSCTL_SET_REFS_SMR_VOLUME_GC_PARAMETERS control code Installable File System Drivers"]
topic_type:
- apiref
api_name:
- FSCTL_SET_REFS_SMR_VOLUME_GC_PARAMETERS
api_location:
- WinIoctl.h
api_type:
- HeaderDef
---

# FSCTL\_SET\_REFS\_SMR\_VOLUME\_GC\_PARAMETERS control code


The **FSCTL\_SET\_REFS\_SMR\_VOLUME\_GC\_PARAMETERS** control code controls the garbage collection on a Shingled Magnetic Recording (SMR) volume.

```ManagedCPlusPlus
BOOL
   DeviceIoControl( (HANDLE)       hDevice,         // handle to volume
                    FSCTL_SET_REFS_SMR_VOLUME_GC_PARAMETERS, // dwIoControlCode
                    (LPDWORD)      lpInBuffer,      // input buffer
                    (DWORD)        nInBufferSize,   // size of input buffer
                     NULL,     // output buffer
                     0,  // size of output buffer
                    (LPDWORD)      lpBytesReturned, // number of bytes returned
                    (LPOVERLAPPED) lpOverlapped );  // OVERLAPPED structure
```

Parameters
----------

*hDevice* \[in\]  
A handle to the device. To obtain a device handle, call the [**CreateFile**](https://msdn.microsoft.com/library/windows/desktop/aa363858) function.

*dwIoControlCode* \[in\]  
The control code for the operation. Use **FSCTL\_SET\_REFS\_SMR\_VOLUME\_GC\_PARAMETERS** for this operation.

*lpInBuffer*   
A pointer to a a caller-allocated [**REFS\_SMR\_VOLUME\_GC\_PARAMETERS**](https://msdn.microsoft.com/library/windows/hardware/mt842917) structure.

*nInBufferSize* \[in\]  
The size of the input buffer, in bytes.

*lpOutBuffer* \[out\]  
Not used with this operation; set to **NULL**.

*nOutBufferSize* \[in\]  
Not used with this operation; set to zero.

*lpBytesReturned* \[out\]  
Not used with this operation; set to **NULL**.

*lpOverlapped* \[in\]  
A pointer to an [**OVERLAPPED**](https://msdn.microsoft.com/library/windows/desktop/ms684342) structure.

If *hDevice* was opened without specifying **FILE\_FLAG\_OVERLAPPED**, *lpOverlapped* is ignored.

If *hDevice* was opened with the **FILE\_FLAG\_OVERLAPPED** flag, the operation is performed as an overlapped (asynchronous) operation. In this case, *lpOverlapped* must point to a valid [**OVERLAPPED**](https://msdn.microsoft.com/library/windows/desktop/ms684342) structure that contains a handle to an event object. Otherwise, the function fails in unpredictable ways.

For overlapped operations, [**DeviceIoControl**](https://msdn.microsoft.com/library/windows/desktop/aa363216) returns immediately, and the event object is signaled when the operation has been completed. Otherwise, the function does not return until the operation has been completed or an error occurs.

Return value
------------

If the operation completes successfully, [**DeviceIoControl**](https://msdn.microsoft.com/library/windows/desktop/aa363216) returns a nonzero value.

If the operation fails or is pending, [**DeviceIoControl**](https://msdn.microsoft.com/library/windows/desktop/aa363216) returns zero. To get extended error information, call [**GetLastError**](https://msdn.microsoft.com/library/windows/desktop/ms679360).

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Version</p></td>
<td align="left"><p>Available starting with Windows 10, version 1709.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">WinIoctl.h</td>
</tr>
</tbody>
</table>

## See also


[**DeviceIoControl**](https://msdn.microsoft.com/library/windows/desktop/aa363216)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bifsk\ifsk%5D:%20FSCTL_SET_REFS_SMR_VOLUME_GC_PARAMETERS%20control%20code%20%20RELEASE:%20%281/9/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




