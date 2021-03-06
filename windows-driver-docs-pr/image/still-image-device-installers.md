---
title: Still Image Device Installers
author: windows-driver-content
description: Still Image Device Installers
ms.assetid: e0ea31de-063a-49a4-922f-62edb774ac76
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Still Image Device Installers


## <a href="" id="ddk-still-image-device-installers-si"></a>


Microsoft provides a class installer for still image devices, with the following features:

-   WDM PnP detection when a device is installed.

-   Installation wizard for legacy devices connected to parallel and serial ports.

-   Support for special INF file entries (see [INF Files for Still Image Devices](inf-files-for-still-image-devices.md)).

-   Support for vendor-supplied co-installer extensions. For more information, see [Writing a Co-installer](https://msdn.microsoft.com/library/windows/hardware/ff554011).

If necessary, vendors can provide customized installation programs that can be used instead of the Microsoft-supplied class installer.

 

 




