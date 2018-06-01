---
title: IVMSCSIControllerCollection Item property
description: The Item property contains the IVMSCSIController object that corresponds to the given index in this collection.
ms.assetid: 2c9d1ba9-5a3e-48a2-a876-9eb370bdc5bf
keywords:
- Item property Virtual Server
- Item property Virtual Server , IVMSCSIControllerCollection interface
- IVMSCSIControllerCollection interface Virtual Server , Item property
- Item property Virtual Server , VMSCSIControllerCollection interface
- VMSCSIControllerCollection interface Virtual Server , Item property
topic_type:
- apiref
api_name:
- IVMSCSIControllerCollection.Item
- IVMSCSIControllerCollection.get_Item
- VMSCSIControllerCollection.Item
api_location:
- VsComInterfaces.h
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IVMSCSIControllerCollection::Item property

The **Item** property contains the [**IVMSCSIController**](ivmscsicontroller.md) object that corresponds to the given index in this collection.

This property is read-only.

## Syntax


```C++
HRESULT get_Item(
  [in]  long              index,
        Long              index,
  [out] IVMSCSIController **scsiController
);
```

<span codelanguage="VisualBasic"></span>

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th>VB</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><pre><code>VMSCSIControllerCollection.Item( _
  ByVal index, _
  ByVal index, _
  ByRef scsiController _
)</code></pre></td>
</tr>
</tbody>
</table>



## Property value

The [**VMSCSIController**](ivmscsicontroller.md) object found at the given index.

This property value is read-only.

## Error codes



| Name                                                                                          | Meaning                                                                                       |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| <dl> <dt>S\_OK</dt> </dl>              | The operation was successful.<br/>                                                      |
| <dl> <dt>E\_POINTER</dt> </dl>         | The *scsiController* parameter is **NULL**.<br/>                                        |
| <dl> <dt>VM\_E\_VM\_UNKNOWN</dt> </dl> | The virtual machine cannot be found.<br/>                                               |
| <dl> <dt>DISP\_E\_BADINDEX</dt> </dl>  | The index of the requested item does not correspond to an item in this collection.<br/> |
| <dl> <dt>DISP\_E\_EXCEPTION</dt> </dl> | An unexpected error occurred.<br/>                                                      |



## Requirements



|                     |                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------|
| Product<br/>  | Microsoft Virtual Server 2005 onWindows Server 2003<br/>                                    |
| Download<br/> | Microsoft Virtual Server 2005 R2 SP1 Update onWindows Server 2008orWindows Server 2003<br/> |
| Header<br/>   | <dl> <dt>VsComInterfaces.h</dt> </dl>      |



## See also

<dl> <dt>

[**IVMSCSIControllerCollection**](ivmscsicontrollercollection.md)
</dt> </dl>

 

 




