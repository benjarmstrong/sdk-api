---
UID: NI:genericusbfnioctl.IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT
title: IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT (genericusbfnioctl.h)
description: This I/O control code (IOCTL) is sent by a user-mode service or application to issue an IN direction transfer on the endpoint that corresponds to the specified pipe ID in the input buffer.helpviewer_keywords: ["IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT","IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT control","IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT control code [Buses]","buses.ioctl_genericusbfn_transfer_in_append_zero_pkt","genericusbfnioctl/IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT"]
old-location: buses\ioctl_genericusbfn_transfer_in_append_zero_pkt.htm
tech.root: usbref
ms.assetid: 9EA139CD-2B00-4B03-AB0D-AE8FB66B687B
ms.date: 12/05/2018
ms.keywords: IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT, IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT control, IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT control code [Buses], buses.ioctl_genericusbfn_transfer_in_append_zero_pkt, genericusbfnioctl/IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT
f1_keywords:
- genericusbfnioctl/IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT
dev_langs:
- c++
req.header: genericusbfnioctl.h
req.include-header: GenericUsbFnIoctl.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
- GenericUsbFnIoctl.h
api_name:
- IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IOCTL_GENERICUSBFN_TRANSFER_IN_APPEND_ZERO_PKT IOCTL


## -description


This  I/O control code (IOCTL) is sent by a user-mode service or application to issue an IN direction transfer on the endpoint that corresponds to the specified pipe ID in the input buffer. A zero-length packet is automatically appended after the data in the output buffer is successfully sent and the transfer payload size is a multiple of the endpoint's maximum packet size. This should be used on the last I/O request that corresponds to a Universal Serial Bus (USB) transfer. 


## -ioctlparameters




### -input-buffer

A <b>USBFNPIPEID</b> that specifies the ID of the pipe to conduct the transfer on.


### -input-buffer-length

The size of a <b>USBFNPIPEID</b>.


### -output-buffer

The data to send to the host.


### -output-buffer-length

The size of the output buffer in bytes.


### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block

<b>Irp-&gt;IoStatus.Status</b> is set to STATUS_SUCCESS if the request is successful. Otherwise, <b>Status</b> to the appropriate error condition as a <a href="https://docs.microsoft.com/windows-hardware/drivers/kernel/ntstatus-values">NTSTATUS</a> code. 


## -remarks



If this I/O control code (IOCTL) is being called synchronously, set the <i>lpOverlapped</i> parameter to NULL. If this IOCTL is called asynchronously, assign the <i>lpOverlapped</i> parameter to a pointer to an <a href="https://docs.microsoft.com/windows/desktop/api/minwinbase/ns-minwinbase-overlapped">OVERLAPPED</a> structure that contains a handle to an event object. The event objects signal when the operation is completed.

The return value is a BOOL value that indicates success or failure of the operation. TRUE indicates success, FALSE otherwise.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/ioapiset/nf-ioapiset-deviceiocontrol">DeviceIoControl</a>



<a href="https://docs.microsoft.com/windows/desktop/api/genericusbfnioctl/ni-genericusbfnioctl-ioctl_genericusbfn_transfer_in">IOCTL_GENERICUSBFN_TRANSFER_IN</a>



<a href="https://docs.microsoft.com/windows/desktop/api/genericusbfnioctl/ni-genericusbfnioctl-ioctl_genericusbfn_transfer_out">IOCTL_GENERICUSBFN_TRANSFER_OUT</a>
 

 

