---
Description: 'The get\_Rate method retrieves the playback rate. This method implements the IMediaPosition::get\_Rate method.'
ms.assetid: '216cbcef-4874-4565-abb0-8c8bf67fe23c'
title: 'CPosPassThru.get\_Rate method'
---

# CPosPassThru.get\_Rate method

The `get_Rate` method retrieves the playback rate. This method implements the [**IMediaPosition::get\_Rate**](imediaposition-get-rate.md) method.

## Syntax


```C++
HRESULT get_Rate(
  �double *pdRate
);
```



## Parameters

<dl> <dt>

*pdRate* 
</dt> <dd>

Pointer to a variable that receives the playback rate.

</dd> </dl>

## Return value

Returns the **HRESULT** value from the connected pin.

## Requirements



|                    |                                                                                                                                                                                            |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Ctlutil.h (include Streams.h)</dt> </dl>                                                                                   |
| Library<br/> | <dl> <dt>Strmbase.lib (retail builds); </dt> <dt>Strmbasd.lib (debug builds)</dt> </dl> |



## See also

<dl> <dt>

[**CPosPassThru Class**](cpospassthru.md)
</dt> </dl>

�

�



