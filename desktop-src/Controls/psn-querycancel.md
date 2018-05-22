---
title: PSN\_QUERYCANCEL notification code
description: Indicates that the user has canceled the property sheet. This notification code is sent in the form of a WM\_NOTIFY message.
ms.assetid: '4a789e08-065a-485c-87e3-f7958e2dc544'
keywords: ["PSN_QUERYCANCEL notification code Windows Controls"]
topic_type:
- apiref
api_name:
- PSN_QUERYCANCEL
api_location:
- Prsht.h
api_type:
- HeaderDef
---

# PSN\_QUERYCANCEL notification code

Indicates that the user has canceled the property sheet. This notification code is sent in the form of a [**WM\_NOTIFY**](wm-notify.md) message.


```C++
PSN_QUERYCANCEL 

    lppsn = (LPPSHNOTIFY) lParam;  
```



## Parameters

<dl> <dt>

*lParam* 
</dt> <dd>

Pointer to a [**PSHNOTIFY**](pshnotify.md) structure that contains information about the notification code. This structure contains an [**NMHDR**](nmhdr.md) structure as its first member, **hdr**. The **hwndFrom** member of this **NMHDR** structure contains the handle to the property sheet. The **lParam** member of the **PSHNOTIFY** structure does not contain any information.

</dd> </dl>

## Return value

Returns **TRUE** to prevent the cancel operation, or **FALSE** to allow it.

## Remarks

This notification code is typically sent when a user clicks the **Cancel** button. It is also sent when a user clicks the **X** button in the property sheet's upper right hand corner or presses the ESCAPE key. A property sheet page can handle this notification code to ask the user to verify the cancel operation.

To set a return value, the dialog box procedure for the page must call the [**SetWindowLong**](https://msdn.microsoft.com/library/windows/desktop/ms633591) function with DWL\_MSGRESULT set to the return value. The dialog box procedure must return **TRUE**.

## Requirements



|                                     |                                                                                    |
|-------------------------------------|------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                     |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                               |
| Header<br/>                   | <dl> <dt>Prsht.h</dt> </dl> |



�

�




