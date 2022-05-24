---
layout: default
---

# CC_EnviarSII_AUC

`APIVERSION: 52`

`STATUS: ACTIVE`

Baja de facturas emitidas

**Author** Oriol Farras

**Group** Controllers

**Date** 2022

## Fields

### `FACTURA_ENVIADAS` → `String`

### `FACTURA_ENVIADAS_RECT` → `String`

### `FACTURA_RECIBIDAS` → `String`

### `FACTURA_RECIBIDAS_RECT` → `String`

---

## Methods

### `static getDatosEnvioSII(ID idFactura)`

`AURAENABLED`

Metodo que devuelve el estado del ultimo sumistro realizado de la factura pasada por parametro

#### Parameters

| Param       | Description |
| ----------- | ----------- |
| `idFactura` |             |

#### Return

**Type**

String

**Description**

estado del ultimo suministro

### `static enviarSII(List<String> idsFacturas, String tipoenvio, String tipofactura, Boolean esRectificada)`

`AURAENABLED`

metodo que envia al sii las facturas indicadas por parametro

#### Parameters

| Param           | Description                         |
| --------------- | ----------------------------------- |
| `idsFacturas`   | ids de las facturas                 |
| `tipoenvio`     | tipo de envio                       |
| `tipofactura`   | tipo de factura                     |
| `esRectificada` | indica si la factura es rectificada |

#### Return

**Type**

string

**Description**

string resultado del envio que se visualizara en el LWC

**Author** Oriol Farras

### `static EnviarFacturasRecibidas(List<String> idsFacturas, String tipoenvio, Boolean esRectificada)`

`AURAENABLED`

metodo privado para enviar las facturas recibidas

#### Parameters

| Param           | Description                             |
| --------------- | --------------------------------------- |
| `idsFacturas`   | ids de las facturas                     |
| `tipoenvio`     | tipo de envio                           |
| `esRectificada` | indica si se trata de un recitificación |

#### Return

**Type**

String

**Description**

resultado del suministro

### `static EnviarFacturasEnviadas(List<String> idsFacturas, String tipoenvio, Boolean esRectificada)`

`AURAENABLED`

metodo privado para enviar las facturas emitidas

#### Parameters

| Param           | Description                             |
| --------------- | --------------------------------------- |
| `idsFacturas`   | ids de las facturas                     |
| `tipoenvio`     | tipo de envio                           |
| `esRectificada` | indica si se trata de un recitificación |

#### Return

**Type**

String

**Description**

resultado del suministro

### `static marcarFacturasEnviadas(List<String> idsFacturas, String sobjectName)`

`AURAENABLED`

Metodo para marcar las facturas como enviadas al SII

#### Parameters

| Param         | Description                                      |
| ------------- | ------------------------------------------------ |
| `idsFacturas` | ids de las facturas a marcar                     |
| `sobjectName` | nombre del metadatado SII_Facturas_Object\_\_mdt |

### `static getFacturasQuery(SII_Facturas_Object__mdt configuracionObjeto, List<String> idsFacturas)`

Metodo privado para generar la query de las facturas dados lo metadatos

#### Parameters

| Param                 | Description                  |
| --------------------- | ---------------------------- |
| `configuracionObjeto` | objeto del metadato          |
| `idsFacturas`         | ids de las facturas a buscar |

#### Return

**Type**

String

**Description**

query que vamos a realizar

---
