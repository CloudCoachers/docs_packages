---
layout: default
title: Tests
nav_order: 4
parent: SII
---

# CC_SII_UtilsTest

`ISTEST`

`APIVERSION: 52`

`STATUS: ACTIVE`

Test CC_EnviarSII_AUC

**Author** Oriol Farras

**Group** Tests

**Date** 12/2021

## Fields

### `XMLRESPUESTACORRECTOFE` → `String`

### `XMLRESPUESTACORRECTOFR` → `String`

### `XMLRESPUESTAFAULT` → `String`

---

## Methods

### `static testFormatearFecha()`

`ISTEST`

### `static testPopulateDoc()`

`ISTEST`

### `static testgetSObjectField()`

`ISTEST`

### `static testCreateFileOnRecord()`

## `ISTEST`

## Classes

### CC_RespuestaFacturasMock

#### Constructors

##### `CC_RespuestaFacturasMock(String numFactura, String nodeName)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `nodeName` → `String`

##### `numFactura` → `String`

---

#### Methods

##### `respond(HTTPRequest req)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### CC_RespuestasBajaFacturasMock

#### Constructors

##### `CC_RespuestasBajaFacturasMock(String numFactura, String nodeName)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `nodeName` → `String`

##### `numFactura` → `String`

---

#### Methods

##### `respond(HTTPRequest req)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

---
