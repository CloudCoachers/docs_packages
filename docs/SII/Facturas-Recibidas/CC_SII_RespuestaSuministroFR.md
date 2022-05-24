---
layout: default
title: Facturas Recibidas
nav_order: 4
parent: Facturas Recibidas
---

# CC_SII_RespuestaSuministroFR

`APIVERSION: 52`

`STATUS: ACTIVE`

Gestion de la respuesta del webservice de presentacion de facturas recibidas

**Author** Oriol Farras

**Group** Facturas Recibidas

**Date** 2022

## Fields

### `reqBody` → `string`

### `reqResponse` → `string`

---

## Methods

### `static procesarRespuesta(Dom.XmlNode bodyNode, String bodyChildNodeName, List<CC_SII_FacturaObj> facturas, String tipoConfiguracion)`

metodo que procesa la respuesta recibida por el servicio

#### Parameters

| Param               | Description                                                        |
| ------------------- | ------------------------------------------------------------------ |
| `bodyNode`          | nodo con el body de la respuesta                                   |
| `bodyChildNodeName` | nombre del node con el body de la resputa                          |
| `facturas`          | lista de facturas donde indicar el resultado                       |
| `tipoConfiguracion` | tipo de la configuracion del metadadato SII_Facturas_Object\_\_mdt |

#### Return

**Type**

String

**Description**

resultado de la presentación

**Author** Oriol Farras | 05-24-2022

### `static guardarRespuesta(CC_SII_RespuestaSuministroFR.RespuestaSuministro respuesta, List<CC_SII_FacturaObj> facturaspresentadas, String mensajeError, String tipoConfiguracion)`

metodo que guarda la respuesta recibida por el servicio

#### Parameters

| Param                 | Description                                                              |
| --------------------- | ------------------------------------------------------------------------ |
| `respuesta`           | tipo de la inner class RespuestaSuministro con los datos de la respuesta |
| `facturaspresentadas` | lista con las facturas presentadas                                       |
| `mensajeError`        | mensajde de error recibido                                               |
| `tipoConfiguracion`   | tipo de la configuracion del metadadato SII_Facturas_Object\_\_mdt       |

#### Return

**Type**

List&lt;String&gt;

**Description**

resultado de la presentación

**Author** Oriol Farras | 05-24-2022

---

## Classes

### Cabecera

Inner class para la gestion del nodo Cabecera

#### Constructors

##### `Cabecera(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Properties

##### `IDVersionSii` → `String`

##### `TipoComunicacion` → `String`

##### `Titular` → `Titular`

---

### IDEmisorFactura

Inner class para la gestion del nodo IDEmisorFactura

#### Constructors

##### `IDEmisorFactura(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Properties

##### `NIF` → `String`

---

### IDFactura

Inner class para la gestion del nodo IDFactura

#### Constructors

##### `IDFactura(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Properties

##### `FechaExpedicionFacturaEmisor` → `String`

##### `IDEmisorFactura` → `IDEmisorFactura`

##### `NumSerieFacturaEmisor` → `String`

---

### RespuestaLinea

Inner class para la gestion del nodo RespuestaLinea

#### Constructors

##### `RespuestaLinea(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Properties

##### `CSV` → `String`

##### `CodigoErrorRegistro` → `String`

##### `DescripcionErrorRegistro` → `String`

##### `EstadoRegistro` → `String`

##### `IDFactura` → `IDFactura`

##### `RefExterna` → `String`

---

### RespuestaSuministro

Inner class para la gestion del nodo RespuestaSuministro

#### Constructors

##### `RespuestaSuministro(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Properties

##### `CSV` → `String`

##### `Cabecera` → `Cabecera`

##### `EstadoEnvio` → `String`

##### `RespuestaLinea` → `List&lt;RespuestaLinea&gt;`

---

### Titular

Inner class para la gestion del nodo Titular

#### Constructors

##### `Titular(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Properties

##### `NIF` → `String`

##### `NombreRazon` → `String`

---

---
