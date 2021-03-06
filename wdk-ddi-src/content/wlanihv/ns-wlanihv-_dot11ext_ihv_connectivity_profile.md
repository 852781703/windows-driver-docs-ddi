---
UID: NS:wlanihv._DOT11EXT_IHV_CONNECTIVITY_PROFILE
title: "_DOT11EXT_IHV_CONNECTIVITY_PROFILE"
author: windows-driver-content
description: Important  The Native 802.11 Wireless LAN interface is deprecated in Windows 10 and later.
old-location: netvista\dot11ext_ihv_connectivity_profile.htm
tech.root: netvista
ms.assetid: 56ef9b59-5dbb-4720-bae1-7af6d9dbc110
ms.date: 02/16/2018
ms.keywords: "*PDOT11EXT_IHV_CONNECTIVITY_PROFILE, DOT11EXT_IHV_CONNECTIVITY_PROFILE, DOT11EXT_IHV_CONNECTIVITY_PROFILE structure [Network Drivers Starting with Windows Vista], Native_802.11_data_types_a0d8e30b-4a72-44d2-a83a-c7b1785f2c8e.xml, PDOT11EXT_IHV_CONNECTIVITY_PROFILE, PDOT11EXT_IHV_CONNECTIVITY_PROFILE structure pointer [Network Drivers Starting with Windows Vista], _DOT11EXT_IHV_CONNECTIVITY_PROFILE, netvista.dot11ext_ihv_connectivity_profile, wlanihv/DOT11EXT_IHV_CONNECTIVITY_PROFILE, wlanihv/PDOT11EXT_IHV_CONNECTIVITY_PROFILE"
ms.topic: struct
req.header: wlanihv.h
req.include-header: Wlanihv.h
req.target-type: Windows
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating   systems.
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
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	wlanihv.h
api_name:
-	DOT11EXT_IHV_CONNECTIVITY_PROFILE
product:
- Windows
targetos: Windows
req.typenames: DOT11EXT_IHV_CONNECTIVITY_PROFILE, *PDOT11EXT_IHV_CONNECTIVITY_PROFILE
req.product: Windows 10 or later.
---

# _DOT11EXT_IHV_CONNECTIVITY_PROFILE structure


## -description


<div class="alert"><b>Important</b>  The <a href="https://msdn.microsoft.com/library/windows/hardware/ff560689">Native 802.11 Wireless LAN</a> interface is deprecated in Windows 10 and later. Please use the WLAN Device Driver Interface (WDI) instead. For more information about WDI, see <a href="https://msdn.microsoft.com/6EF92E34-7BC9-465E-B05D-2BCB29165A18">WLAN Universal Windows driver model</a>.</div><div> </div>The DOT11EXT_IHV_CONNECTIVITY_PROFILE structure specifies connectivity settings for the IHV
  profile.


## -syntax


```cpp
typedef struct _DOT11EXT_IHV_CONNECTIVITY_PROFILE {
  LPWSTR pszXmlFragmentIhvConnectivity;
} DOT11EXT_IHV_CONNECTIVITY_PROFILE, *PDOT11EXT_IHV_CONNECTIVITY_PROFILE;
```


## -struct-fields




### -field pszXmlFragmentIhvConnectivity

A pointer to the string that defines the IHV connectivity profile.

