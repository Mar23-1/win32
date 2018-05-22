---
Description: VideoInfo2 Format Type
ms.assetid: 'edd2013a-f0c5-4176-ba3a-a3af719ce31d'
title: VideoInfo2 Format Type
---

# VideoInfo2 Format Type

A preview pin's preferred media type might be a type with a [**VIDEOINFOHEADER2**](videoinfoheader2.md) format. This format structure supports special features such as interlaced video and picture aspect ratios.

The VMR-7 and the VMR-9 both support [**VIDEOINFOHEADER2**](videoinfoheader2.md) directly. When you connect the VMR to the decoder, they will negotiate the best format. The older Video Renderer filter, however, does not support **VIDEOINFOHEADER2**. To use **VIDEOINFOHEADER2** format types with the Video Renderer filter, you must insert the [Overlay Mixer](overlay-mixer-filter.md) filter into the graph.

1.  Enumerate the preferred media types on the decoder filter's output pin, using the [**IPin::EnumMediaTypes**](ipin-enummediatypes.md) method.
2.  Check the first media type in the enumeration sequence.
3.  If the format type is **FORMAT\_VideoInfo2**, connect the output pin to the Overlay Mixer. Then connect the Overlay Mixer to the video renderer. (See [Video Port Pins](video-port-pins.md).)

If you do not care about these features, you do not have to use the Overlay Mixer. Connect the decoder directly to the Video Renderer, and it will connect with a [**VIDEOINFOHEADER**](videoinfoheader.md) format instead.

## Related topics

<dl> <dt>

[Advanced Capture Topics](advanced-capture-topics.md)
</dt> <dt>

[Using the Overlay Mixer in Video Capture](using-the-overlay-mixer-in-video-capture.md)
</dt> </dl>

 

 


