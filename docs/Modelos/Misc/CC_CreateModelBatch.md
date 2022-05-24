---
layout: default
title: CC_CreateModelBatch
parent: Misc
nav_order: 2
---

# CC_CreateModelBatch

`APIVERSION: 52`

`STATUS: ACTIVE`

Batch para rellenar los datos de los modelos con los datos de la org

**Author** Oriol Farras

**Since** 2022

## Constructors

### `CC_CreateModelBatch(sObject model)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `CC_CreateModelBatch(List<sObject> models)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---

## Fields

### `CLASS_NAME` → `string`

### `READY_TO_SENT` → `string`

### `configModelo` → `AEAT_Model__mdt`

### `idsOrigins` → `Set<id>`

### `listModels` → `List<sObject>`

### `mapFieldConstants` → `Map<String,string>`

### `mapFieldSource` → `Map<String,map<string,string>>`

### `mapSources` → `Map<Id,List<SObject>>`

### `model` → `sObject`

### `namespacePrefix` → `String`

---

## Methods

### `init()`

Metodo init

### `start(Database.BatchableContext bc)`

#### Parameters

| Param | Description |
| ----- | ----------- |
| `bc`  |             |

#### Return

**Type**

Database.QueryLocator

**Description**

`Database.QueryLocator`

### `execute(Database.BatchableContext bc, List<Data_Source__mdt> datasources)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `finish(Database.BatchableContext bc)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `getModeloDates(String yearstr, String periodstr)`

`TESTVISIBLE`

#### Parameters

| Param       | Description |
| ----------- | ----------- |
| `yearstr`   |             |
| `periodstr` |             |

#### Return

**Type**

List&lt;String&gt;

**Description**

`List&lt;String&gt;`

### `static hasSObjectField(String fieldName, SObject so)`

`TESTVISIBLE`

#### Parameters

| Param       | Description |
| ----------- | ----------- |
| `fieldName` |             |
| `so`        |             |

#### Return

**Type**

boolean

**Description**

`boolean`

---
