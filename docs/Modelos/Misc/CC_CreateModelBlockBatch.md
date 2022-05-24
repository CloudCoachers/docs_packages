---
layout: default
title: CC_CreateModelBlockBatch
parent: Modelos
nav_order: 2
---

# CC_CreateModelBlockBatch

`APIVERSION: 52`

`STATUS: ACTIVE`

## Constructors

### `CC_CreateModelBlockBatch(Id modelId, Id blockId)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---

## Fields

### `CLASS_NAME` → `string`

### `inputDefinitions` → `List<Input_Definition__mdt>`

### `modelBlock` → `Model_Block__mdt`

### `modelId` → `Id`

### `modelList` → `List<sObject>`

### `namespacePrefix` → `String`

### `queryDataSource` → `String`

---

## Methods

### `start(Database.BatchableContext bc)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `execute(Database.BatchableContext bc, List<sObject> listsObjects)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `finish(Database.BatchableContext bc)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---
