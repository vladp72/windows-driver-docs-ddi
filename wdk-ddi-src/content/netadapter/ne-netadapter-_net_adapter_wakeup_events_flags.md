---
UID: NE:netadapter._NET_ADAPTER_WAKEUP_EVENTS_FLAGS
title: _NET_ADAPTER_WAKEUP_EVENTS_FLAGS
author: windows-driver-content
description: Specifies the media-independent wake-up events that a network adapter supports.
ms.assetid: 2fe56738-0b96-4dc2-a2d2-7cddc802e232
ms.author: windowsdriverdev
ms.date: 02/05/2018
ms.topic: enum
ms.keywords: _NET_ADAPTER_WAKEUP_EVENTS_FLAGS, NET_ADAPTER_WAKEUP_EVENTS_FLAGS, 
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: netadapter.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver: 1.21
req.umdf-ver:
req.ddi-compliance:
req.max-support:
req.alt-api:
req.alt-loc:
req.typenames: NET_ADAPTER_WAKEUP_EVENTS_FLAGS
topictype: 
-	apiref
apitype: 
-	HeaderDef
apilocation: 
-	netadapter.h
apiname: 
-	NET_ADAPTER_WAKEUP_EVENTS_FLAGS
product: Windows
targetos: Windows
req.product: Windows 10 or later.
---

# _NET_ADAPTER_WAKEUP_EVENTS_FLAGS enumeration

## -description

> [!WARNING]
> Some information in this topic relates to prereleased product, which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.
>
> NetAdapterCx is preview only in Windows 10, version 1803.

Specifies the media-independent wake-up events that a network adapter supports.

## -enum-fields

### -field NET_ADAPTER_WAKE_ON_MEDIA_CONNECT : 
If this flag is set, the network adapter can generate a wake-up event when it becomes connected to the networking interface.

### -field NET_ADAPTER_WAKE_ON_MEDIA_DISCONNECT : 
If this flag is set, the network adapter can generate a wake-up event when it becomes disconnected to the networking interface.

## -remarks

The **NET_ADAPTER_WAKEUP_EVENTS_FLAGS** enumeration is used to specify media-independent wake-up events in the [NET_ADAPTER_POWER_CAPABILITIES](ns-netadapter-_net_adapter_power_capabilities.md) structure.

The client driver passes an initialized **NET_ADAPTER_POWER_CAPABILITIES** structure as an input parameter value to [NetAdapterSetPowerCapabilities](nf-netadapter-netadaptersetpowercapabilities.md).

The minimum NetAdapterCx version for **NET_ADAPTER_WAKEUP_EVENTS_FLAGS** is 1.0.

## -see-also

[NDIS_PM_CAPABILITIES](../ntddndis/ns-ntddndis-_ndis_pm_capabilities.md)