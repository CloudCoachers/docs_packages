---
layout: default
---
# CC_CreateModelBatch

`APIVERSION: 52`

`STATUS: ACTIVE`
## Constructors
### `CC_CreateModelBatch(sObject model)`
#### Parameters
|Param|Description|
|---|---|

### `CC_CreateModelBatch(List<sObject> models)`
#### Parameters
|Param|Description|
|---|---|

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
### `start(Database.BatchableContext bc)`
#### Parameters
|Param|Description|
|---|---|

### `execute(Database.BatchableContext bc, List<Data_Source__mdt> datasources)`
#### Parameters
|Param|Description|
|---|---|

### `finish(Database.BatchableContext bc)`
#### Parameters
|Param|Description|
|---|---|

### `getModeloDates(String yearstr, String periodstr)`

`TESTVISIBLE`
#### Parameters
|Param|Description|
|---|---|

### `static hasSObjectField(String fieldName, SObject so)`

`TESTVISIBLE`
#### Parameters
|Param|Description|
|---|---|

---
