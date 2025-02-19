---
UID: NC:ddraw.LPDDENUMSURFACESCALLBACK
title: LPDDENUMSURFACESCALLBACK (ddraw.h)
description: Do not use. This callback function is superseded by the EnumSurfacesCallback7 function that is used with the IDirectDraw7::EnumSurfaces, IDirectDrawSurface7::EnumAttachedSurfaces, and IDirectDrawSurface7::EnumOverlayZOrders methods.
helpviewer_keywords: ["EnumSurfacesCallback","EnumSurfacesCallback callback function [DirectDraw]","LPDDENUMSURFACESCALLBACK","LPDDENUMSURFACESCALLBACK callback","ddraw/EnumSurfacesCallback","directdraw.enumsurfacescallback"]
old-location: directdraw\enumsurfacescallback.htm
tech.root: directdraw
ms.assetid: 4195C266-4F1D-4DD6-935E-78D07ACAA765
ms.date: 12/05/2018
ms.keywords: EnumSurfacesCallback, EnumSurfacesCallback callback function [DirectDraw], LPDDENUMSURFACESCALLBACK, LPDDENUMSURFACESCALLBACK callback, ddraw/EnumSurfacesCallback, directdraw.enumsurfacescallback
req.header: ddraw.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
 - LPDDENUMSURFACESCALLBACK
 - ddraw/LPDDENUMSURFACESCALLBACK
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Ddraw.h
api_name:
 - EnumSurfacesCallback
---

# LPDDENUMSURFACESCALLBACK callback function


## -description

Do not use. This callback function is superseded by the <a href="https://docs.microsoft.com/windows/desktop/api/ddraw/nc-ddraw-lpddenumsurfacescallback7">EnumSurfacesCallback7</a> function that is used with the <a href="https://docs.microsoft.com/windows/desktop/api/ddraw/nf-ddraw-idirectdraw7-enumsurfaces">IDirectDraw7::EnumSurfaces</a>, <a href="https://docs.microsoft.com/windows/desktop/api/ddraw/nf-ddraw-idirectdrawsurface7-enumattachedsurfaces">IDirectDrawSurface7::EnumAttachedSurfaces</a>, and <a href="https://docs.microsoft.com/windows/desktop/api/ddraw/nf-ddraw-idirectdrawsurface7-enumoverlayzorders">IDirectDrawSurface7::EnumOverlayZOrders</a> methods.

## -parameters

### -param Arg1

### -param Arg2

### -param Arg3

#### - lpContext [in]

A pointer to an application-defined structure to be passed to the callback function each time that the function is called.


#### - lpDDSurface [in]

A pointer to the <b>IDirectDrawSurface</b> interface for the attached surface.


#### - lpDDSurfaceDesc [in]

A pointer to a <a href="https://docs.microsoft.com/previous-versions/windows/hardware/drivers/ff550339(v=vs.85)">DDSURFACEDESC</a> structure that describes the attached surface.

## -returns

The callback function returns DDENUMRET_OK to continue the enumeration.

It returns DDENUMRET_CANCEL to stop the enumeration.

## -remarks

You can use the LPDDENUMSURFACESCALLBACK data type to declare a variable that can contain a pointer to this callback function.

