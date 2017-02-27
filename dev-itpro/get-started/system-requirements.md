---
title: System requirements
description: This topic lists the system requirements for the current version of Microsoft Dynamics 365 for Operations.
author: sericks007
manager: AnnBe
ms.date: 2016-02-25 22 - 43 - 40
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User, Developer, IT Pro
ms.search.scope: Core
ms.custom: 55651
ms.assetid: e564d51d-42d3-47c5-b388-93b8219c692a
ms.search.region: Global
ms.author: sericks
ms.dyn365.ops.intro: 01-08-2016
ms.dyn365.ops.version: Platform update 2
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 1f8bc1ff3561c47a8b2f4d6203de699551dc40cc
ms.lasthandoff: 02/22/2017


---

# <a name="system-requirements"></a>System requirements

This topic lists the system requirements for the current version of Microsoft Dynamics 365 for Operations.

<a name="supported-web-browsers"></a>Supported web browsers
----------------------

The Microsoft Dynamics 365 for Operations web application can run in any of the following web browsers that run on the specified operating systems:

-   Microsoft Edge (latest publicly available version) on Windows 10
-   Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7
-   Google Chrome (latest publicly available version) on Windows 10, Windows 8.1, Windows 8, Windows 7, or Google Nexus 10 tablet
-   Apple Safari (latest publicly available version) on Mac OS X 10.10 (Yosemite), 10.11 (El Capitan) or 10.12 (Sierra), or Apple iPad

To find the latest release for each web browser, go to the software manufacturer’s website. **Notes:**

-   To capture images that are generated from Task Recorder and include them in Microsoft Word documents, you must have a Chrome extension installed. For instructions about how to install the extension, see [Screenshot Extension setup](task-recorder.md#screenshot-extension-setup).
-   The Workflow Editor is started as a ClickOnce application. Only Microsoft Edge and Internet Explorer (on a supported version of Microsoft Windows) support ClickOnce applications. The Workflow Editor ClickOnce application requires a 64-bit compatible operating system.
-   The Report Designer for Financial reporting is started as a ClickOnce application. It requires a 64-bit compatible operating system. If you’re using Chrome, you must install a ClickOnce extension in order to download the report designer client. If you’re using Chrome with the incognito mode, make sure that the ClickOnce extension is also enabled for incognito mode.

### <a name="supported-web-browsers-for-retail-cloud-pos"></a>Supported web browsers for Retail Cloud POS

Retail Cloud POS for Dynamics 365 for Operations can run in any of the following web browsers that run on the specified operating systems:

-   Microsoft Edge (latest publicly available version) on Windows 10
-   Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7
-   Chrome (latest publicly available version) on Windows 10, Windows 8.1, or Windows 7

## <a name="network-requirements"></a>Network requirements
-   Dynamics 365 for Operations is designed for networks with latency of less than 150 milliseconds (ms). This is the latency from a browser client to the Microsoft Azure data center that hosts Dynamics 365 for Operations. We recommend that you test network latency at <http://www.azurespeed.com>.
-   Bandwidth requirements for Dynamics 365 for Operations depend on your scenario. Most typical scenarios require a bandwidth of more than 50 kilobytes per second (KBps). However, for scenarios that have high payload requirements, such as workspaces or scenarios that involve extensive customization, more bandwidth is recommended.

In general, Dynamics 365 for Operations is optimized for the Internet. The number of round trips from a browser client to the Azure data center is very small, and the whole payload is compressed. **Warning:** Don't compute bandwidth requirements from a client location by multiplying the number of users by the minimum bandwidth requirements. The concurrent usage of a given location is very difficult to calculate. For customers who are concerned about bandwidth requirements, use a preview version of Dynamics 365 for Operations.

## <a name="net-framework-requirements"></a>.NET Framework requirements
Dynamics 365 for Operations requires .NET Framework version 4.6.2 for all click-once applications, such as the document routing agent. For installation instructions, see [Installing the .NET Framework](https://msdn.microsoft.com/en-us/library/5a4x27ek(v=vs.110).aspx).

## <a name="supported-microsoft-office-applications"></a>Supported Microsoft Office applications
-   To run the Microsoft Excel and Word add-ins, you must have Microsoft Office 2016 for Windows or Mac installed. For more details about version requirements, see [Office integration troubleshooting](office-integration-troubleshooting.md).
-   To view documents that are generated by the Export to Excel or Export to Word functionality, you must have Microsoft Office 2007 or later installed.

## <a name="retail-modern-pos-requirements"></a>Retail Modern POS requirements
### <a name="supported-operating-systems"></a>Supported operating systems

-   Retail Modern POS is a 32-bit application, but it will run on both x86 and x64 architectures.
-   Retail Modern POS is supported only on Windows 10 Pro, Enterprise, and Enterprise Long Term Servicing Branch (LTSB) editions.

### <a name="minimum-system-requirements"></a>Minimum system requirements

-   The minimum supported resolution is 1280 × 1024.
-   The computer that Retail Modern POS runs on must meet these requirements:
    -   It must have, at a minimum, a dual-core processor that runs at no less than 2 gigahertz (GHz).
    -   It must have, at a minimum, 3 gigabytes (GB) of RAM.
    -   It must have Internet access.

## <a name="retail-hardware-station-requirements"></a>Retail hardware station requirements
### <a name="supported-operating-systems"></a>Supported operating systems

-   Retail hardware station is a 32-bit application, but it will run on both x86 and x64 architectures.
-   Retail hardware station is supported on the following operating systems:
    -   Windows 7 Professional, Enterprise, and Ultimate editions **Note:** Windows 7 is supported only if Internet Explorer 11 is manually installed on the system.
    -   Windows 8.1 Update 1 Professional, Enterprise, and Embedded editions
    -   Windows 10 Pro, Enterprise, and Enterprise LTSB editions

### <a name="minimum-system-requirements"></a>Minimum system requirements

The computer must meet all system requirements for installing and using the following items:

-   Internet Information Services (IIS)
-   Third-party hardware

## <a name="retail-store-scale-unit-requirements"></a>Retail Store Scale Unit requirements
### <a name="supported-operating-systems"></a>Supported operating systems

-   Retail Store Scale Unit is a 32-bit application, but it will run on both x86 and x64 architectures.
-   Retail Store Scale Unit is supported on the following operating systems:
    -   Windows 7 Professional, Enterprise, and Ultimate editions
    -   Windows 8.1 Update 1 Professional, Enterprise, and Embedded editions
    -   Windows 10 Pro, Enterprise, and Enterprise LTSB editions

### <a name="minimum-system-requirements"></a>Minimum system requirements

-   4 GB of RAM
-   1.6 GHz peak CPU speed per core (Two cores are the minimum.)
-   At least 10 GB of free space (The channel database can require a large amount of space.)

### <a name="recommended-system-requirements"></a>Recommended system requirements

-   6 GB of RAM
-   2.4 GHz i7 (or equivalent) peak CPU speed per core (Four cores are recommended.)
-   At least 10 GB of free space (The channel database can require a large amount of space.)

## <a name="requirements-for-development-on-local-vms"></a>Requirements for development on local VMs
For information about the requirements for development on local virtual machines (VMs), see [VM running on-premises](access-instances.md#vm-running-on-premises).

<a name="see-also"></a>See also
--------

[Get an evaluation copy of Dynamics 365 for Operations](get-evaluation-copy.md)


