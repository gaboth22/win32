---
title: Calling ImmSetConversionStatus() or ImmGetConversionStatus() from Windows Store apps is not supported
description: Calling ImmSetConversionStatus() or ImmGetConversionStatus() from Windows Store apps is not supported
ms.assetid: C6F3C8E7-E07A-40C6-A257-037766C670E7
ms.topic: article
ms.date: 05/31/2018
---

# Calling ImmSetConversionStatus() or ImmGetConversionStatus() from Windows Store apps is not supported

## Platforms

<dl> Clients - windows 8.1  
Servers - Windows Server 2012 R2  
</dl>

## Description

Calling ImmSetConversionStatus() or ImmGetConversionStatus() from a Windows Store app is not supported and may cause unexpected results.

## Manifestations

At application start up, the IME mode is set to the following defaults:



|          | Software input panel | Hardware keyboard |
|----------|----------------------|-------------------|
| KOR, JPN | On                   | Off               |
| CHS, CHT | On                   | On                |



 

## Solution

Developers can control the default IME mode by specifying an input scope value for the field.

The IME mode for a specified input scope is determined by each IME. Developers cannot specify the IME mode.

## Resources

-   [InputScope Enumeration](https://msdn.microsoft.com/library/windows/desktop/ms538181(v=vs.85).aspx)
-   [ImmSetConversionStatus](https://msdn.microsoft.com/library/windows/desktop/dd318584(v=vs.85).aspx)
-   [ImmGetConversionStatus](https://msdn.microsoft.com/library/aa912903.aspx)

 

 




