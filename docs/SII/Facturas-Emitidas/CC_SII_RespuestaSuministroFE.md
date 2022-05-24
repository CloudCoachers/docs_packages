---
layout: default
title: Facturas Emitidas
nav_order: 4
parent: Facturas Emitidas
---

# CC_SII_RespuestaSuministroFE

`APIVERSION: 52`

`STATUS: ACTIVE`

Gestion de la respuesta del webservice de presentacion de facturas emitidas

**Author** Oriol Farras

**Group** Facturas Emitidas

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

### `static guardarRespuesta(CC_SII_RespuestaSuministroFE.RespuestaLRFEmitidasType respuesta, List<CC_SII_FacturaObj> facturaspresentadas, String mensajeError, String tipoConfiguracion)`

metodo que guarda la respuesta recibida por el servicio

#### Parameters

| Param                 | Description                                                                   |
| --------------------- | ----------------------------------------------------------------------------- |
| `respuesta`           | tipo de la inner class RespuestaLRFEmitidasType con los datos de la respuesta |
| `facturaspresentadas` | lista con las facturas presentadas                                            |
| `mensajeError`        | mensajde de error recibido                                                    |
| `tipoConfiguracion`   | tipo de la configuracion del metadadato SII_Facturas_Object\_\_mdt            |

#### Return

**Type**

list&lt;string&gt;

**Description**

resultado de la presentación

**Author** Oriol Farras | 05-24-2022

---

## Classes

### RespuestaExpedidaType

Innner class del nodo RespuestaExpedidaType

#### Constructors

##### `RespuestaExpedidaType()`

##### `RespuestaExpedidaType(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `codigoErrorRegistro` → `Integer`

##### `csv` → `String`

##### `descripcionErrorRegistro` → `String`

##### `estadoRegistro` → `String`

##### `iDFactura` → `CC_SII_SuministroInformacion.IDFacturaExpedidaType`

##### `refExterna` → `String`

##### `registroDuplicado` → `CC_SII_SuministroInformacion.RegistroDuplicadoType`

---

### RespuestaLRFEmitidasType

Innner class del nodo RespuestaLRFEmitidasType

#### Constructors

##### `RespuestaLRFEmitidasType()`

##### `RespuestaLRFEmitidasType(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `cabecera` → `CC_SII_SuministroInformacion.CabeceraSii`

##### `csv` → `String`

##### `datosPresentacion` → `CC_SII_SuministroInformacion.DatosPresentacionType`

##### `estadoEnvio` → `String`

##### `respuestaLinea` → `List&lt;CC_SII_RespuestaSuministroFE.RespuestaExpedidaType&gt;`

---

---
