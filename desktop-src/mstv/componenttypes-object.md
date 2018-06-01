---
title: ComponentTypes Object
description: ComponentTypes Object
ms.assetid: b0a468fd-6294-4148-a727-3a4bd51df6dc
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# ComponentTypes Object

The **ComponentTypes** object represents a collection of component types.



|                           |                                            |
|---------------------------|--------------------------------------------|
| Interfaces                | [**IComponentTypes**](/previous-versions/windows/desktop/api/tuner/nn-tuner-icomponenttypes) |
| Outgoing Event Interfaces | None                                       |
| CLSID                     | CLSID\_ComponentTypes                      |



 

## Remarks

Each [Component](component-object.md) object contains one [ComponentType](componenttype-object.md) object. The **ComponentTypes** collection is used to create a list of default preferred component types for a tuning space, or a list of preferred component types on the tune request which override the default types.

## Related topics

<dl> <dt>

[Components](components.md)
</dt> <dt>

[Tuning Model Objects](tuning-model-objects.md)
</dt> </dl>

 

 



