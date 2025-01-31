---
title: taxArea resource type
description: A tax area.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.subservice: "d365-business-central"
doc_type: resourcePageType
---

# taxArea resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a tax area resource type in Dynamics 365 Business Central.

## Methods
| Method       | Return Type  |Description|
|:---------------|:--------|:----------|
|[Get taxArea](../api/dynamics-taxarea-get.md)|taxArea|Gets a tax area object.|
|[Post taxArea](../api/dynamics-create-taxarea.md)|taxArea|Creates a tax area object.|
|[Patch taxArea](../api/dynamics-taxarea-update.md)|taxArea|Updates a tax area object.|
|[Delete taxArea](../api/dynamics-taxarea-delete.md)|none|Deletes a tax area object.|

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|id|GUID|The unique ID of the tax area. Non-editable.|
|code|string, maximum size 20| The code of the tax area.|
|displayName|string, maximum size 50| The display name of the tax area.|
|taxType|string|The tax type of the tax area.|
|lastModifiedDateTime|datetime|The last datetime the tax area was modified. Read-Only.|

## Relationships

## JSON representation

The following JSON representation shows the resource type.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "datetime"
}
```




