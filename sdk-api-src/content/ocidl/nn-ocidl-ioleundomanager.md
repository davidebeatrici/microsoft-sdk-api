---
UID: NN:ocidl.IOleUndoManager
title: IOleUndoManager (ocidl.h)
description: The IOleUndoManager interface enables containers to implement multi-level undo and redo operations for actions that occur within contained controls.
helpviewer_keywords: ["IOleUndoManager","IOleUndoManager interface [COM]","IOleUndoManager interface [COM]","described","_ole_ioleundomanager","com.ioleundomanager","ocidl/IOleUndoManager"]
old-location: com\ioleundomanager.htm
tech.root: com
ms.assetid: 0f507506-3589-4d5b-b1b3-010bce9ae42f
ms.date: 12/05/2018
ms.keywords: IOleUndoManager, IOleUndoManager interface [COM], IOleUndoManager interface [COM],described, _ole_ioleundomanager, com.ioleundomanager, ocidl/IOleUndoManager
req.header: ocidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: OCIdl.idl
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
 - IOleUndoManager
 - ocidl/IOleUndoManager
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - OCIdl.h
api_name:
 - IOleUndoManager
---

# IOleUndoManager interface


## -description

The <b>IOleUndoManager</b> interface enables containers to implement multi-level undo and redo operations for actions that occur within contained controls.

## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IOleUndoManager</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IOleUndoManager</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IOleUndoManager</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-add">Add</a>
</td>
<td align="left" width="63%">
Adds a simple undo unit to the collection.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-close">Close</a>
</td>
<td align="left" width="63%">
Closes the specified parent undo unit.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-discardfrom">DiscardFrom</a>
</td>
<td align="left" width="63%">
Instructs the undo manager to discard the specified undo unit and all undo units below it on the undo or redo stack.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-enable">Enable</a>
</td>
<td align="left" width="63%">
Enables or disables the undo manager.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-enumredoable">EnumRedoable</a>
</td>
<td align="left" width="63%">
Creates an enumerator object that the caller can use to iterate through a series of top-level undo units from the redo stack.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-enumundoable">EnumUndoable</a>
</td>
<td align="left" width="63%">
Creates an enumerator object that the caller can use to iterate through a series of top-level undo units from the undo stack.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-getlastredodescription">GetLastRedoDescription</a>
</td>
<td align="left" width="63%">
Retrieves the description for the top-level undo unit that is on top of the redo stack.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-getlastundodescription">GetLastUndoDescription</a>
</td>
<td align="left" width="63%">
Retrieves the description for the top-level undo unit that is on top of the undo stack.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-getopenparentstate">GetOpenParentState</a>
</td>
<td align="left" width="63%">
Retrieves state information about the innermost open parent undo unit.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-open">Open</a>
</td>
<td align="left" width="63%">
Opens a new parent undo unit, which becomes part of its containing unit's undo stack.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-redoto">RedoTo</a>
</td>
<td align="left" width="63%">
Instructs the undo manager to invoke undo actions back through the redo stack, down to and including the specified undo unit.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-undoto">UndoTo</a>
</td>
<td align="left" width="63%">
Instructs the undo manager to perform actions back through the undo stack, down to and including the specified undo unit.

</td>
</tr>
</table>

## -remarks

The control must create an undo unit with the <a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nn-ocidl-ioleundounit">IOleUndoUnit</a> interface or a parent undo unit with the <a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nn-ocidl-ioleparentundounit">IOleParentUndoUnit</a> interface derived from <b>IOleUndoUnit</b>. Both of these interfaces perform the undo action and the parent undo unit additionally can contain nested undo units.

The undo manager provides a centralized undo and redo service. It manages parent undo units and simple undo units on the undo and redo stacks. Whether an object is UI-active or not, it can deposit undo units on these stacks by calling methods in the undo manager.

The centralized undo manager then has the data necessary to support the undo and redo user interface for the host application and can discard undo information gradually as the stack becomes full.

The undo manager is implemented as a service and objects obtain a pointer to <b>IOleUndoManger</b> from the <a href="https://docs.microsoft.com/previous-versions/windows/internet-explorer/ie-developer/platform-apis/cc678965(v=vs.85)">IServiceProvider</a> interface. It is usually implemented by the container. The service manages two stacks, the undo stack and the redo stack, each of which contains undo units generated by embedded objects or by the container application itself.

Undo units are typically generated in response to actions taken by the end user. An object does not generate undo actions for programmatic events. In fact, programmatic events should clear the undo stack since the programmatic event can possibly invalidate assumptions made by the undo units on the stack.

When the object's state changes, it creates an undo unit encapsulating all the information needed to undo that change. The object calls methods in the undo manager to place its undo units on the stack. Then, when the end user selects an Undo operation, the undo manager takes the top undo unit off the stack, invokes its action by calling its <a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundounit-do">IOleUndoUnit::Do</a> method, and then releases it. When an end user selects a Redo operation, the undo manager takes the top redo unit off the stack, invokes its action by calling its <b>IOleUndoUnit::Do</b> method, and then releases it.

The undo manager has three states: the base state, the undo state, and the redo state. It begins in the base state. To perform an action from the undo stack, it puts itself into the undo state, calls <a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundounit-do">IOleUndoUnit::Do</a> on the undo unit, and goes back to the base state. To perform an action from the redo stack, it puts itself into the redo state, calls <b>IOleUndoUnit::Do</b> on the undo unit, and goes back to the base state.

If the undo manager receives a new undo unit while in the base state, it places the unit on the undo stack and discards the entire redo stack. While it is in the undo state, it puts incoming units on the redo stack. While it is in the redo state, it places them on the undo stack without flushing the redo stack.

The undo manager also allows objects to discard the undo or redo stack starting from any object in either stack.

The host application determines the scope of an undo manager. For example, in one application, the scope might be at the document level; a separate undo manager is maintained for each document; and undo is managed independently for each document. However, another application maintain one undo manager, and therefore one undo scope, for the entire application.


#### Error Handling

Having an undo operation fail and leaving the document in an unstable state is something the undo manager, undo units, and the application itself all have to work together to avoid. As a result, there are certain requirements that undo units, the undo manager, and the application or component using undo must conform to.

To perform an undo, the undo manager calls <a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundounit-do">IOleUndoUnit::Do</a> on one or more undo units which can, in turn, contain more units. If a unit somewhere in the hierarchy fails, the error will eventually reach the undo manager, which is responsible for making an attempt to roll back the state of the document to what it was before the call to the last top-level unit. The undo manager performs the rollback by calling <b>IOleUndoUnit::Do</b> on the unit that was added to the redo stack during the undo attempt. If the rollback also fails, then the undo manager is forced to abandon everything and return to the application. The undo manager indicates whether the rollback succeeded, and the application can take different actions based on this, such as reinitializing components so they're in a known state.

All the steps in adding an undo unit to the stack should be performed atomically. That is, all steps must succeed or none of them should succeed.

The host application that provides the undo manager decides what action to take when undo fails. At the very least, it should inform the user of the failure. The host application will be told by the undo manager whether the undo succeeded and whether the attempted rollback succeeded. In case both the undo and rollback failed, the host application can present the user with several options, including immediately shutting down the application.

Simple undo units must not change the state of any object if they return failure. This includes the state of the redo stack or undo stack if performing a redo. They are also required to put a corresponding unit on the redo or undo stack if they succeed. The application should be stable before and after the unit is called.

Parent undo units have the same requirements as simple units, with one exception. If one or more children succeeded prior to another child's failure, the parent unit must commit its corresponding unit on the redo stack and return the failure to its parent. If no children succeeded, the parent unit should commit its redo unit only if it has made a state change that needs to be rolled back. For example, suppose a parent unit contains three simple units. The first two succeed and added units to the redo stack, but the third one failed. At this point, the parent unit commits its redo unit and returns the failure.

As a side effect, the parent unit should never make state changes that depend on the success of their children. Doing this will cause the rollback behavior to break. If a parent unit makes state changes, it should do them before calling any children. Then, if the state change fails, it should not commit its redo unit, it should not call any children, and it should return the failure to its parent.

The undo manager has one primary requirement for error handling: to attempt rollback when an undo or redo fails.


#### Non-compliant Objects

Objects that do not support multi-level undo can cause serious problems for a global undo service. Since the object cannot be relied on to properly update the undo manager, any units submitted by other objects are also suspect, because their units may rely on the state of the non-compliant object. Attempting to undo a compliant object's units may not be successful, because the state in the non-compliant object will not match.

To detect objects that do not support multi-level undo, check for the OLEMISC_SUPPORTSMULTILEVELUNDO value. An object that can participate in the global undo service sets this value.

When an object without this value is added to a user-visible undo context, the best practice is to disable the undo user interface for this context. Alternatively, a dialog could be presented to the user, asking them whether to attempt to provide partial undo support, working around the non-compliance of the new object.

In addition, non-compliant objects may be added to nested containers. In this case, the nested container needs to notify the undo manager that undo can no longer be safely supported by calling <a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nf-ocidl-ioleundomanager-enable">IOleUndoManager::Enable</a> with <b>FALSE</b>.

## -see-also

<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nn-ocidl-ioleparentundounit">IOleParentUndoUnit</a>



<a href="https://docs.microsoft.com/windows/desktop/api/ocidl/nn-ocidl-ioleundounit">IOleUndoUnit</a>

