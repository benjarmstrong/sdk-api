---
UID: NF:faxcomex.IFaxDevice.get_RingsBeforeAnswer
title: IFaxDevice::get_RingsBeforeAnswer (faxcomex.h)
description: The IFaxDevice::get_RingsBeforeAnswer property is a number that specifies the number of rings that occur before the fax device answers an incoming fax call.helpviewer_keywords: ["IFaxDevice interface [Fax Service]","RingsBeforeAnswer property","IFaxDevice.RingsBeforeAnswer","IFaxDevice.get_RingsBeforeAnswer","IFaxDevice.put_RingsBeforeAnswer","IFaxDevice::RingsBeforeAnswer","IFaxDevice::get_RingsBeforeAnswer","IFaxDevice::put_RingsBeforeAnswer","RingsBeforeAnswer property [Fax Service]","RingsBeforeAnswer property [Fax Service]","IFaxDevice interface","_mfax_faxdevice.ringsbeforeanswer","fax._mfax_faxdevice_cpp_mfax_faxdevice_ringsbeforeanswer_cpp","fax._mfax_faxdevice_ringsbeforeanswer","faxcomex/IFaxDevice::RingsBeforeAnswer","faxcomex/IFaxDevice::get_RingsBeforeAnswer","faxcomex/IFaxDevice::put_RingsBeforeAnswer","get_RingsBeforeAnswer"]
old-location: fax\_mfax_faxdevice_cpp_mfax_faxdevice_ringsbeforeanswer_cpp.htm
tech.root: Fax
ms.assetid: VS|fax|~\fax\faxinta_n_01iq.htm
ms.date: 12/05/2018
ms.keywords: IFaxDevice interface [Fax Service],RingsBeforeAnswer property, IFaxDevice.RingsBeforeAnswer, IFaxDevice.get_RingsBeforeAnswer, IFaxDevice.put_RingsBeforeAnswer, IFaxDevice::RingsBeforeAnswer, IFaxDevice::get_RingsBeforeAnswer, IFaxDevice::put_RingsBeforeAnswer, RingsBeforeAnswer property [Fax Service], RingsBeforeAnswer property [Fax Service],IFaxDevice interface, _mfax_faxdevice.ringsbeforeanswer, fax._mfax_faxdevice_cpp_mfax_faxdevice_ringsbeforeanswer_cpp, fax._mfax_faxdevice_ringsbeforeanswer, faxcomex/IFaxDevice::RingsBeforeAnswer, faxcomex/IFaxDevice::get_RingsBeforeAnswer, faxcomex/IFaxDevice::put_RingsBeforeAnswer, get_RingsBeforeAnswer
f1_keywords:
- faxcomex/IFaxDevice.RingsBeforeAnswer
dev_langs:
- c++
req.header: faxcomex.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
req.dll: Fxscomex.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Fxscomex.dll
api_name:
- IFaxDevice.RingsBeforeAnswer
- IFaxDevice.get_RingsBeforeAnswer
- IFaxDevice.put_RingsBeforeAnswer
- IFaxDevice.get_RingsBeforeAnswer
- IFaxDevice.put_RingsBeforeAnswer
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IFaxDevice::get_RingsBeforeAnswer


## -description


The <b>IFaxDevice::get_RingsBeforeAnswer</b> property is a number that specifies the number of rings that occur before the fax device answers an incoming fax call.

This property is read/write.


## -parameters


## -remarks



This property is used only if the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-faxdevice-receivemode">ReceiveMode</a> property of the device is set to <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/faxcomex/ne-faxcomex-fax_device_receive_mode_enum">fdrmAUTO_ANSWER</a>.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-faxdevice">FaxDevice</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/faxcomex/nn-faxcomex-ifaxdevice">IFaxDevice</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/fax/-mfax-configuring-a-fax-device">Visual Basic Example</a>
 

 

