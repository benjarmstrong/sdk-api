---
UID: NF:wuapi.IUpdate.get_Title
title: IUpdate::get_Title (wuapi.h)
description: Gets the localized title of the update.helpviewer_keywords: ["IUpdate interface [Windows Update Agent]","Title property","IUpdate.Title","IUpdate.get_Title","IUpdate::Title","IUpdate::get_Title","Title property [Windows Update Agent]","Title property [Windows Update Agent]","IUpdate interface","get_Title","wua.iupdate_title","wuapi/IUpdate::Title","wuapi/IUpdate::get_Title"]
old-location: wua\iupdate_title.htm
tech.root: Wua_Sdk
ms.assetid: 83b1bcfc-d974-4804-8ed0-1ccde335b5ac
ms.date: 12/05/2018
ms.keywords: IUpdate interface [Windows Update Agent],Title property, IUpdate.Title, IUpdate.get_Title, IUpdate::Title, IUpdate::get_Title, Title property [Windows Update Agent], Title property [Windows Update Agent],IUpdate interface, get_Title, wua.iupdate_title, wuapi/IUpdate::Title, wuapi/IUpdate::get_Title
f1_keywords:
- wuapi/IUpdate.Title
dev_langs:
- c++
req.header: wuapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional with SP3 [desktop apps only]
req.target-min-winversvr: Windows Server 2003, Windows 2000 Server with SP3 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Wuapi.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Wuguid.lib
req.dll: Wuapi.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Wuapi.dll
api_name:
- IUpdate.Title
- IUpdate.get_Title
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IUpdate::get_Title


## -description


Gets the localized title of the update.

This property is read-only.


## -parameters


## -remarks



If the <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nn-wuapi-iupdatesearcher">IUpdateSearcher</a> interface  is  created by using the <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nf-wuapi-iupdatesession-createupdatesearcher">IUpdateSession::CreateUpdateSearcher</a> method, the information  that   this property returns is for the language that is  specified by the <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nf-wuapi-iupdatesession2-get_userlocale">UserLocale</a> property. This is the <b>UserLocale</b> property  of the <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nn-wuapi-iupdatesession2">IUpdateSession2</a> interface of the session that is used to create <b>IUpdateSearcher</b>.

If a language preference is not specified by the <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nf-wuapi-iupdatesession2-get_userlocale">UserLocale</a> property of <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nn-wuapi-iupdatesession2">IUpdateSession2</a>, or if the <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nn-wuapi-iupdatesearcher">IUpdateSearcher</a> interface  is not  created by using <a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nf-wuapi-iupdatesession-createupdatesearcher">IUpdateSession::CreateUpdateSearcher</a>, the information that is returned by  this property is for the default user interface (UI) language of the user. If the default UI language of the user is unavailable, Windows Update Agent (WUA) uses the default UI language of the computer.   If the default language of the computer is unavailable, WUA uses the language  that  the provider of the  update recommends.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wuapi/nn-wuapi-iupdate">IUpdate</a>
 

 

