---
UID: NF:fltkernel.FltSetIoPriorityHintIntoCallbackData
title: FltSetIoPriorityHintIntoCallbackData function
author: windows-driver-content
description: The FltSetIoPriorityHintIntoCallbackData routine is used by a minifilter driver to set the I/O priority information in callback data.
old-location: ifsk\fltsetiopriorityhintintocallbackdata.htm
tech.root: ifsk
ms.assetid: 25aba58b-654b-4492-9c54-83c53987342a
ms.date: 04/16/2018
ms.keywords: FltApiRef_p_to_z_2d697ab8-c8ef-47f5-bfed-d0a82a61a1ef.xml, FltSetIoPriorityHintIntoCallbackData, FltSetIoPriorityHintIntoCallbackData routine [Installable File System Drivers], fltkernel/FltSetIoPriorityHintIntoCallbackData, ifsk.fltsetiopriorityhintintocallbackdata
ms.topic: function
req.header: fltkernel.h
req.include-header: FltKernel.h
req.target-type: Universal
req.target-min-winverclnt: Available starting with Windows Vista.
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
req.lib: FltMgr.lib
req.dll: Fltmgr.sys
req.irql: "<= DISPATCH_LEVEL"
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	fltmgr.sys
api_name:
-	FltSetIoPriorityHintIntoCallbackData
product:
- Windows
targetos: Windows
req.typenames: 
---

# FltSetIoPriorityHintIntoCallbackData function


## -description


The <b>FltSetIoPriorityHintIntoCallbackData</b> routine is used by a minifilter driver to set the I/O priority information in callback data.


## -parameters




### -param Data [in]

A pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff544620">FLT_CALLBACK_DATA</a> structure that represents an I/O operation. This parameter is required and cannot be <b>NULL</b>. 


### -param PriorityHint [in]

The <a href="https://msdn.microsoft.com/library/windows/hardware/ff550594">IO_PRIORITY_HINT</a> enumeration value to set for the I/O operation in the callback data pointed to by <i>Data</i>.


## -returns



If this is a fast IO operation, the <b>FltSetIoPriorityHintIntoCallbackData</b> routine returns STATUS_SUCCESS.  

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_INVALID_PARAMETER</b></dt>
</dl>
</td>
<td width="60%">
The value of the <i>PriorityHint</i> parameter is invalid. This is an error code. 

</td>
</tr>
</table>
 




## -remarks



This routine is NONPAGED and can be called from paging I/O paths.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff544620">FLT_CALLBACK_DATA</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff541766">FltApplyPriorityInfoThread</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff543065">FltGetIoPriorityHint</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff543068">FltGetIoPriorityHintFromCallbackData</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff543074">FltGetIoPriorityHintFromFileObject</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff543080">FltGetIoPriorityHintFromThread</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff544354">FltRetrieveIoPriorityInfo</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff544530">FltSetIoPriorityHintIntoFileObject</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff544534">FltSetIoPriorityHintIntoThread</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550594">IO_PRIORITY_HINT</a>
 

 

