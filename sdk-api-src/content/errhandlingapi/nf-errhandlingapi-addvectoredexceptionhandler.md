---
UID: NF:errhandlingapi.AddVectoredExceptionHandler
title: AddVectoredExceptionHandler function (errhandlingapi.h)
description: Registers a vectored exception handler.
helpviewer_keywords: ["AddVectoredExceptionHandler","AddVectoredExceptionHandler function","_win32_addvectoredexceptionhandler","base.addvectoredexceptionhandler","errhandlingapi/AddVectoredExceptionHandler"]
old-location: base\addvectoredexceptionhandler.htm
tech.root: Debug
ms.assetid: 0e956746-e6da-49d8-a534-753cb6755673
ms.date: 12/05/2018
ms.keywords: AddVectoredExceptionHandler, AddVectoredExceptionHandler function, _win32_addvectoredexceptionhandler, base.addvectoredexceptionhandler, errhandlingapi/AddVectoredExceptionHandler
req.header: errhandlingapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - AddVectoredExceptionHandler
 - errhandlingapi/AddVectoredExceptionHandler
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - Kernel32.dll
 - API-MS-Win-Core-errorhandling-l1-1-1.dll
 - KernelBase.dll
 - API-MS-Win-Core-errorhandling-l1-1-2.dll
 - API-MS-Win-DownLevel-Kernel32-l1-1-0.dll
 - MinKernelBase.dll
 - API-MS-Win-Core-ErrorHandling-L1-1-3.dll
api_name:
 - AddVectoredExceptionHandler
---

# AddVectoredExceptionHandler function

## -description

Registers a vectored exception handler.

## -parameters

### -param First

The order in which the handler should be called. If the parameter is nonzero, the handler is the first handler to be called. If the parameter is zero, the handler is the last handler to be called.

### -param Handler

A pointer to the handler to be called. For more information, see [VectoredHandler](/windows/desktop/api/winnt/nc-winnt-pvectored_exception_handler).

## -returns

If the function succeeds, the return value is a handle to the exception handler.

If the function fails, the return value is **NULL**.

## -remarks

If the *First* parameter is nonzero, the handler is the first handler to be called until a subsequent call to **AddVectoredExceptionHandler** is used to specify a different handler as the first handler.

If the *VectoredHandler* parameter points to a function in a DLL and that DLL is unloaded, the handler is still registered. This can lead to application errors.

To unregister the handler, use the [RemoveVectoredExceptionHandler function](nf-errhandlingapi-removevectoredexceptionhandler.md) function.

To compile an application that uses this function, define the _WIN32_WINNT macro as 0x0500 or later. For more information, see [Using the Windows Headers](/windows/desktop/WinProg/using-the-windows-headers).

### Examples

For an example, see [Using a Vectored Exception Handler](/windows/desktop/Debug/using-a-vectored-exception-handler).

## -see-also

[AddVectoredContinueHandler function](nf-errhandlingapi-addvectoredcontinuehandler.md), [RemoveVectoredExceptionHandler function](nf-errhandlingapi-removevectoredexceptionhandler.md), [Vectored Exception Handling](/windows/desktop/Debug/vectored-exception-handling), [VectoredHandler](/windows/desktop/api/winnt/nc-winnt-pvectored_exception_handler)
