---
layout: default
title: Utils
nav_order: 4
parent: Utils
---

# CC_SII_Utils

`APIVERSION: 52`

`STATUS: ACTIVE`

Baja de facturas emitidas

**Author** Oriol Farras

**Group** Utils

**Date** 2022

## Fields

### `RESP_NS` → `String`

### `SIILR_NS` → `String`

### `SIILR_PRE` → `string`

### `SII_NS` → `String`

### `SII_PRE` → `string`

---

## Methods

### `static formatearFechaSII(Date d)`

Metodo para formatear una fecha en el formato esperado por el WS de SII

#### Parameters

| Param | Description      |
| ----- | ---------------- |
| `d`   | Fecha de entrada |

#### Return

**Type**

String

**Description**

String Fecha formateada con el formato dd-mm-yyyy

**Author** Oriol Farras | 12/11/2019

### `static populateDoc(DOM.Document doc)`

Metodo que genera los datos basicos del xml, como cabecera y namespaces

#### Parameters

| Param | Description                                  |
| ----- | -------------------------------------------- |
| `doc` | Documento XML donde anidaremos los nodos XML |

#### Return

**Type**

DOM.XmlNode

**Description**

DOM.XmlNode Devuelve el nodo donde anidar los datos

**Author** Oriol Farras | 12/9/2019

### `static addChildElement(Dom.XmlNode xmlnode, String namespace, String prefijo, String clave, String valor)`

metodo que anida una clave a un nodo de XML

#### Parameters

| Param       | Description              |
| ----------- | ------------------------ |
| `xmlnode`   | Nodo de entrada a anidar |
| `namespace` | Nombre del namespace     |
| `prefijo`   | Prefijo a utilizar       |
| `clave`     | nobmre del nodo          |
| `valor`     | valor del nodo           |

**Author** Oriol Farras | 10-01-2021

### `static addChildElement(Dom.XmlNode xmlnode, String namespace, String prefijo, String clave, String valor, Boolean required)`

metodo que anida una clave a un nodo de XML

#### Parameters

| Param       | Description                    |
| ----------- | ------------------------------ |
| `xmlnode`   | Nodo de entrada a anidar       |
| `namespace` | Nombre del namespace           |
| `prefijo`   | Prefijo a utilizar             |
| `clave`     | nobmre del nodo                |
| `valor`     | valor del nodo                 |
| `required`  | indica si el nodo es requerido |

**Author** Oriol Farras | 10-01-2021

### `static getsObjectField(sObject facturaObject, String fieldName)`

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

## Classes

### UtilsException

---
