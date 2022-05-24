---
layout: default
title: CC_Utils
parent: Utils
nav_order: 5
---

# CC_Utils

`NAMESPACEACCESSIBLE`

`APIVERSION: 52`

`STATUS: ACTIVE`

Clase con utiles para

**Group** Misc

**Author** Oriol Farras

**Date** 01/12/2021

## Methods

### `static getsObjectField(sObject facturaObject, String fieldName)`

`NAMESPACEACCESSIBLE`

return the object value for the sObject record

#### Parameters

| Param           | Description |
| --------------- | ----------- |
| `facturaObject` |             |
| `fieldName`     |             |

#### Return

**Type**

Object

**Description**

Object

**Author** Oriol Farras | 10-11-2021

### `static createFileOnRecord(String fileContents, String filename, Id attachedTo)`

`NAMESPACEACCESSIBLE`

store file on provided id

#### Parameters

| Param         | Description            |
| ------------- | ---------------------- |
| `xmlResponse` | - xml to store         |
| `title`       | - title of the file    |
| `filename`    | - name of the file     |
| `recordId`    | - record to be related |

**Author** Oriol Farras | 10-20-2021

### `static getFacturasQuery(SII_Facturas_Object__mdt configuracionObjeto, List<String> idsFacturas)`

`NAMESPACEACCESSIBLE`

Esta funcion pasado un configuración de objeto

#### Parameters

| Param                 | Description |
| --------------------- | ----------- |
| `configuracionObjeto` |             |
| `idsFacturas`         |             |

#### Return

**Type**

String

**Description**

String

**Author** Oriol Farras | 11-18-2021

---
