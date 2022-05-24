---
layout: default
title: Utils
nav_order: 4
nav_exclude: true
---

# CC_SII_EnviarFacturas_BCH

`APIVERSION: 53`

`STATUS: ACTIVE`

Classe que implementa Batchable y Schedulabe para poder programar y enviar por lotes las facturas

**Author** Oriol Farras

**Group** Utils

**Date** 2022

## Constructors

### `CC_SII_EnviarFacturas_BCH(Date fecha, String tipoConfiguracion)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---

## Fields

### `FACTURA_ENVIADAS` → `String`

### `FACTURA_RECIBIDAS` → `String`

### `erroresResultadosEnvio` → `String`

### `fecha` → `Date`

### `fechaOrigen` → `Date`

### `tipoConfiguracion` → `String`

---

## Methods

### `execute(SchedulableContext sc)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `start(Database.BatchableContext BC)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `execute(Database.BatchableContext BC, List<sObject> scope)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `finish(Database.BatchableContext BC)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `static finish(String erroresResultadosEnvio)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---
