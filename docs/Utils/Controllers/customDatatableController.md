---
layout: default
title: customDatatableController
parent: Controllers
nav_order: 5
---

# customDatatableController

`APIVERSION: 52`

`STATUS: ACTIVE`

Controlador del lwc custom datatable

**Author** Oriol Farras

**Group** Controllers

**Date** 01-19-2022

## Methods

### `static getColumnas(String componente)`

`AURAENABLED`

#### Parameters

| Param        | Description |
| ------------ | ----------- |
| `componente` |             |

#### Return

**Type**

list&lt;wraperColumn&gt;

**Description**

list&lt;wraperColumn&gt;

**Author** Oriol Farras | 01-14-2022

### `static getFiltros(String componente)`

`AURAENABLED`

#### Parameters

| Param        | Description |
| ------------ | ----------- |
| `componente` |             |

#### Return

**Type**

list&lt;wrapperFilter&gt;

**Description**

list&lt;wrapperFilter&gt;

**Author** Oriol Farras | 01-14-2022

### `static getRegistros(String componente, String filtros, Integer queryOffset)`

`AURAENABLED`

#### Parameters

| Param         | Description |
| ------------- | ----------- |
| `componente`  |             |
| `filtros`     |             |
| `queryOffset` |             |

#### Return

**Type**

wrapperData

**Description**

wrapperData

**Author** Oriol Farras | 01-14-2022

---

## Classes

### wraperColumn

#### Properties

##### `fieldName` → `string`

`AURAENABLED`

##### `label` → `string`

`AURAENABLED`

##### `numColumna` → `Integer`

`AURAENABLED`

##### `type` → `string`

`AURAENABLED`

---

#### Methods

##### `compareTo(Object compareTo)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### wrapperData

#### Properties

##### `keyField` → `String`

`AURAENABLED`

##### `maxRowsSelect` → `Integer`

`AURAENABLED`

##### `queryLimit` → `Integer`

`AURAENABLED`

##### `registros` → `List&lt;sObject&gt;`

`AURAENABLED`

##### `total` → `Integer`

`AURAENABLED`

---

### wrapperFilter

#### Properties

##### `PicklistaData` → `string`

`AURAENABLED`

##### `id` → `string`

`AURAENABLED`

##### `label` → `string`

`AURAENABLED`

##### `name` → `string`

`AURAENABLED`

##### `operand` → `string`

`AURAENABLED`

##### `order` → `Integer`

`AURAENABLED`

##### `required` → `Boolean`

`AURAENABLED`

##### `type` → `string`

`AURAENABLED`

##### `value` → `string`

`AURAENABLED`

---

#### Methods

##### `compareTo(Object compareTo)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

---
