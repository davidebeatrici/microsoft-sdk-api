---
UID: NF:segment.IMSVidVideoRenderer2.SetAllocator
title: IMSVidVideoRenderer2::SetAllocator (segment.h)
description: The SetAllocator method specifies an allocator-presenter for the VMR. Applications can use this method to provide their own custom allocator-presenter objects.
helpviewer_keywords: ["IMSVidVideoRenderer2 interface [Microsoft TV Technologies]","SetAllocator method","IMSVidVideoRenderer2.SetAllocator","IMSVidVideoRenderer2::SetAllocator","SetAllocator","SetAllocator method [Microsoft TV Technologies]","SetAllocator method [Microsoft TV Technologies]","IMSVidVideoRenderer2 interface","mstv.imsvidvideorenderer2_setallocator","segment/IMSVidVideoRenderer2::SetAllocator"]
old-location: mstv\imsvidvideorenderer2_setallocator.htm
tech.root: mstv
ms.assetid: c73edfea-bafd-4640-9be6-45e5a2bb81ef
ms.date: 12/05/2018
ms.keywords: IMSVidVideoRenderer2 interface [Microsoft TV Technologies],SetAllocator method, IMSVidVideoRenderer2.SetAllocator, IMSVidVideoRenderer2::SetAllocator, SetAllocator, SetAllocator method [Microsoft TV Technologies], SetAllocator method [Microsoft TV Technologies],IMSVidVideoRenderer2 interface, mstv.imsvidvideorenderer2_setallocator, segment/IMSVidVideoRenderer2::SetAllocator
req.header: segment.h
req.include-header: Msvidctl.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Segment.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - IMSVidVideoRenderer2::SetAllocator
 - segment/IMSVidVideoRenderer2::SetAllocator
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - segment.h
api_name:
 - IMSVidVideoRenderer2.SetAllocator
---

# IMSVidVideoRenderer2::SetAllocator


## -description

The <b>SetAllocator</b> method specifies an allocator-presenter for the VMR. Applications can use this method to provide their own custom allocator-presenter objects.

## -parameters

### -param AllocPresent [in]

Pointer to the <b>IUnknown</b> interface of the allocator-presenter object.

### -param ID [in]

Optionally, specifies an identifier (ID) for the allocator-presenter object. The default value of -1 indicates that the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/legacy/dd695138(v=vs.85)">MSVidVideoRenderer</a> object will create an ID when it builds the filter graph. In that case, the MSVidVideoRenderer object uses the lower 32 bits of the allocator-presenter's <b>IUnknown</b> interface pointer as the ID. Note that the ID is for application use; the VMR does not use it.

## -returns

Returns an <b>HRESULT</b> value. Possible values include the following.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
</table>

## -see-also

<a href="https://docs.microsoft.com/windows/desktop/api/segment/nn-segment-imsvidvideorenderer2">IMSVidVideoRenderer2 Interface</a>

