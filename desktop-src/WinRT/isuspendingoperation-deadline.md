﻿---
Description: 'Gets the time remaining before a delayed app suspending operation continues.'
ms.assetid: 'A90347F3-75CB-4EEB-930D-30882F43D192'
title: 'ISuspendingOperation::Deadline property'
---

# ISuspendingOperation::Deadline property

Gets the time remaining before a delayed app suspending operation continues.

This property is read/write.

## Syntax


```C++
HRESULT put_Deadline();

HRESULT get_Deadline(
  [out, retval] DateTime *value
);
```



## Property value

The time remaining before a delayed app suspending operation continues.

## Requirements



|                                     |                                                                                                         |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8<br/>                                                                                    |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                                          |
| Header<br/>                   | <dl> <dt>Windows.ApplicationModel.h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Windows.ApplicationModel.idl</dt> </dl> |



## See also

<dl> <dt>

[**ISuspendingOperation**](isuspendingoperation.md)
</dt> </dl>

 

 



