﻿---
Description: 'The ClearSourceList method of the Installer object removes all network sources from the source list.'
ms.assetid: 'a4e4beb2-a4d7-48e7-9c8d-dd1ae19fe92a'
title: 'Installer.ClearSourceList method'
---

# Installer.ClearSourceList method

The **ClearSourceList** method of the [**Installer**](installer-object.md) object removes all network sources from the source list.

## Syntax


```JScript
Installer.ClearSourceList(
  Product,
  User
)
```



## Parameters

<dl> <dt>

*Product* 
</dt> <dd>

Specifies the product code.

</dd> <dt>

*User* 
</dt> <dd>

User name for per-user installation; null or empty string for per-machine installation.

</dd> </dl>

## Return value

This method does not return a value.

## Requirements



|                    |                                                                                                                                                                                                                                                         |
|--------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Version<br/> | Windows Installer 5.0 on Windows Server 2012, Windows 8, Windows Server 2008 R2 or Windows 7. Windows Installer 4.0 or Windows Installer 4.5 on Windows Server 2008 or Windows Vista. Windows Installer on Windows Server 2003 or Windows XP<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                      |
| IID<br/>     | IID\_IInstaller is defined as 000C1090-0000-0000-C000-000000000046<br/>                                                                                                                                                                           |



## See also

<dl> <dt>

[**MsiSourceListClearAll**](msisourcelistclearall.md)
</dt> <dt>

[Source Resiliency](source-resiliency.md)
</dt> </dl>

 

 



