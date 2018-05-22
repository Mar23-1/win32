﻿---
Description: 'The put\_Hue method specifies the hue value on which to key. This property applies only when the key type is DXTKEY\_HUE.'
ms.assetid: '90c8c610-7ceb-479b-bb0e-d8753d0d7dac'
title: 'IDxtKey::put\_Hue method'
---

# IDxtKey::put\_Hue method

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The `put_Hue` method specifies the hue value on which to key. This property applies only when the key type is DXTKEY\_HUE.

## Syntax


```C++
HRESULT put_Hue(
  [in] int newVal
);
```



## Parameters

<dl> <dt>

*newVal* \[in\]
</dt> <dd>

The hue value on which to key. The valid range is from 0 to 360.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](http://go.microsoft.com/fwlink/p/?linkid=129787). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[**IDxtKey Interface**](idxtkey.md)
</dt> <dt>

[**IDxtKey::put\_KeyType**](idxtkey-put-keytype.md)
</dt> </dl>

 

 



