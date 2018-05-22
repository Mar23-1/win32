---
title: SBM\_GETSCROLLINFO message
description: The SBM\_GETSCROLLINFO message is sent to retrieve the parameters of a scroll bar.
ms.assetid: '3b43430f-b55f-43ec-8558-baf5c953064f'
keywords: ["SBM_GETSCROLLINFO message Windows Controls"]
topic_type:
- apiref
api_name:
- SBM_GETSCROLLINFO
api_location:
- Winuser.h
api_type:
- HeaderDef
---

# SBM\_GETSCROLLINFO message

The **SBM\_GETSCROLLINFO** message is sent to retrieve the parameters of a scroll bar.

Applications should not send this message directly. Instead, they should use the [**GetScrollInfo**](getscrollinfo.md) function. A window receives this message through its [*WindowProc*](https://msdn.microsoft.com/library/windows/desktop/ms633573) function. Applications which implement a custom scroll bar control must respond to these messages for the **GetScrollInfo** function to work properly.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

This parameter is not used.

</dd> <dt>

*lParam* 
</dt> <dd>

Pointer to a [**SCROLLINFO**](scrollinfo.md) structure. Before calling [**GetScrollInfo**](getscrollinfo.md), set the **cbSize** member of the structure to **sizeof**(**SCROLLINFO**), and set the **fMask** member to specify the scroll bar parameters to retrieve. Before returning, the message copies the specified parameters to the appropriate members of the structure.

The **fMask** member can be one or more of the following values.



| Value                                                                                                                                                      | Meaning                                                                             |
|------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------|
| <span id="SIF_ALL"></span><span id="sif_all"></span><dl> <dt>**SIF\_ALL**</dt> </dl>                | Combination of SIF\_PAGE, SIF\_POS, SIF\_RANGE, and SIF\_TRACKPOS.<br/>       |
| <span id="SIF_PAGE"></span><span id="sif_page"></span><dl> <dt>**SIF\_PAGE**</dt> </dl>             | Copies the scroll page to the nPage member.<br/>                              |
| <span id="SIF_POS"></span><span id="sif_pos"></span><dl> <dt>**SIF\_POS**</dt> </dl>                | Copies the scroll position to the nPos member. <br/>                          |
| <span id="SIF_RANGE"></span><span id="sif_range"></span><dl> <dt>**SIF\_RANGE**</dt> </dl>          | Copies the scroll range to the nMin and nMax members. <br/>                   |
| <span id="SIF_TRACKPOS"></span><span id="sif_trackpos"></span><dl> <dt>**SIF\_TRACKPOS**</dt> </dl> | Copies the current scroll box tracking position to the nTrackPos member.<br/> |



�

</dd> </dl>

## Return value

If the message retrieved any values, the return value is **TRUE**; otherwise, it is **FALSE**.

## Remarks

The messages that indicate scroll bar position, [**WM\_HSCROLL**](wm-hscroll.md) and [**WM\_VSCROLL**](wm-vscroll.md), provide only 16 bits of position data. However, the [**SCROLLINFO**](scrollinfo.md) structure used by **SBM\_GETSCROLLINFO**, [**SBM\_SETSCROLLINFO**](sbm-setscrollinfo.md), [**GetScrollInfo**](getscrollinfo.md), and [**SetScrollInfo**](setscrollinfo.md) provides 32 bits of scroll bar position data. You can use these messages and functions while processing either the **WM\_HSCROLL** or **WM\_VSCROLL** messages to obtain 32-bit scroll bar position data.

To get the 32-bit position of the scroll box (thumb) during a SB\_THUMBTRACK request code in a [**WM\_HSCROLL**](wm-hscroll.md) or [**WM\_VSCROLL**](wm-vscroll.md) message, send **SBM\_GETSCROLLINFO** with the SIF\_TRACKPOS value in the **fMask** member of the [**SCROLLINFO**](scrollinfo.md) structure. The message returns the tracking position of the scroll box in the **nTrackPos** member of the **SCROLLINFO** structure. This allows you to get the position of the scroll box as the user moves it. Alternatively, you can use the [**GetScrollInfo**](getscrollinfo.md) function to get the same information.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                                           |
| Minimum supported server<br/> | Windows Server�2003 \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

**Reference**
</dt> <dt>

[**GetScrollInfo**](getscrollinfo.md)
</dt> <dt>

[**SBM\_SETSCROLLINFO**](sbm-setscrollinfo.md)
</dt> <dt>

[**SCROLLINFO**](scrollinfo.md)
</dt> <dt>

[**SetScrollInfo**](setscrollinfo.md)
</dt> </dl>

�

�




