---
UID: NI:winioctl.IOCTL_CHANGER_EXCHANGE_MEDIUM
title: IOCTL_CHANGER_EXCHANGE_MEDIUM
description: Moves a piece of media from a source element to one destination, and the piece of media originally in the first destination to a second destination.helpviewer_keywords: ["IOCTL_CHANGER_EXCHANGE_MEDIUM","IOCTL_CHANGER_EXCHANGE_MEDIUM control","IOCTL_CHANGER_EXCHANGE_MEDIUM control code","_win32_ioctl_changer_exchange_medium","base.ioctl_changer_exchange_medium","winioctl/IOCTL_CHANGER_EXCHANGE_MEDIUM"]
old-location: base\ioctl_changer_exchange_medium.htm
tech.root: devio
ms.assetid: 40550df0-9da4-4b02-bd57-23eae78c68df
ms.date: 12/05/2018
ms.keywords: IOCTL_CHANGER_EXCHANGE_MEDIUM, IOCTL_CHANGER_EXCHANGE_MEDIUM control, IOCTL_CHANGER_EXCHANGE_MEDIUM control code, _win32_ioctl_changer_exchange_medium, base.ioctl_changer_exchange_medium, winioctl/IOCTL_CHANGER_EXCHANGE_MEDIUM
f1_keywords:
- winioctl/IOCTL_CHANGER_EXCHANGE_MEDIUM
dev_langs:
- c++
req.header: winioctl.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP
req.target-min-winversvr: Windows Server 2003
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- HeaderDef
api_location:
- WinIoCtl.h
api_name:
- IOCTL_CHANGER_EXCHANGE_MEDIUM
targetos: Windows
req.typenames: 
req.redist: 
---

# IOCTL_CHANGER_EXCHANGE_MEDIUM IOCTL


## -description


Moves a piece of media from a source element to one destination, and the piece of media originally in the first destination to a second destination.

To perform this operation, call the 
<a href="https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol">DeviceIoControl</a> function with the following parameters.
<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>BOOL DeviceIoControl(
  (HANDLE) hDevice,              // handle to device
  IOCTL_CHANGER_EXCHANGE_MEDIUM, // dwIoControlCode(LPVOID) lpInBuffer,           // input buffer
  (DWORD) nInBufferSize,         // size of input buffer
  NULL,                          // lpOutBuffer0,                             // nOutBufferSize(LPDWORD) lpBytesReturned,     // number of bytes returned
  (LPOVERLAPPED) lpOverlapped    // OVERLAPPED structure
);</pre>
</td>
</tr>
</table></span></div>

## -ioctlparameters




### -input-buffer



<text></text>




### -input-buffer-length



<text></text>




### -output-buffer



<text></text>




### -output-buffer-length



<text></text>




### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block



Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [NTSTATUS Values](https://docs.microsoft.com/windows-hardware/drivers/kernel/ntstatus-values).




## -remarks



To swap two pieces of media, specify the source as the value for the second destination.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winioctl/ns-winioctl-changer_exchange_medium">CHANGER_EXCHANGE_MEDIUM</a>



<a href="https://docs.microsoft.com/windows/desktop/DevIO/device-management-control-codes">Device Management Control Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol">DeviceIoControl</a>
 

 

