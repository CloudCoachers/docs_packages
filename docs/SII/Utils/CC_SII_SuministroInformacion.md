---
layout: default
title: Utils
nav_order: 4
parent: SII
---

# CC_SII_SuministroInformacion

`APIVERSION: 52`

`STATUS: ACTIVE`

Inner classes para la generación de los Nodos XMl de facturas enviadas y recibidas

**Author** Oriol Farras

**Group** Utils

**Date** 2022

## Classes

### CabeceraSii

Innner clase del nodo CabeceraSii

#### Constructors

##### `CabeceraSii()`

##### `CabeceraSii(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `iDVersionSii` → `String`

##### `tipoComunicacion` → `String`

##### `titular` → `CC_SII_SuministroInformacion.PersonaFisicaJuridicaESType`

---

#### Methods

##### `populateXmlNode(Dom.XmlNode outerNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### DatosPresentacionType

Innner clase del nodo DatosPresentacionType

#### Constructors

##### `DatosPresentacionType()`

##### `DatosPresentacionType(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `nifPresentador` → `String`

##### `timestampPresentacion` → `String`

---

### IdEmisorFactura

Innner clase del nodo IdEmisorFactura

#### Constructors

##### `IdEmisorFactura()`

##### `IdEmisorFactura(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `nif` → `String`

---

#### Methods

##### `populateXmlNode(Dom.XmlNode outerNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### IdFacturaExpedidaType

Innner clase del nodo IdFacturaExpedidaType

#### Constructors

##### `IdFacturaExpedidaType()`

##### `IdFacturaExpedidaType(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `fechaExpedicionFacturaEmisor` → `String`

##### `idEmisorFactura` → `CC_SII_SuministroInformacion.IDEmisorFactura`

##### `numSerieFacturaEmisor` → `String`

##### `numSerieFacturaEmisorResumenFin` → `String`

---

#### Methods

##### `populateXmlNode(Dom.XmlNode outerNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### PeriodoLiquidacion

Innner clase del nodo PeriodoLiquidacion

#### Constructors

##### `PeriodoLiquidacion()`

---

#### Fields

##### `ejercicio` → `String`

##### `periodo` → `String`

---

#### Methods

##### `populateXmlNode(Dom.XmlNode outerNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### PersonaFisicaJuridicaESType

Innner clase del nodo PersonaFisicaJuridicaESType

#### Constructors

##### `PersonaFisicaJuridicaESType()`

##### `PersonaFisicaJuridicaESType(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `nif` → `String`

##### `nifRepresentante` → `String`

##### `nombreRazon` → `String`

---

#### Methods

##### `populateXmlNode(Dom.XmlNode outerNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### RegistroDuplicadoType

Innner clase del nodo RegistroDuplicadoType

#### Constructors

##### `RegistroDuplicadoType()`

##### `RegistroDuplicadoType(DOM.XmlNode responseNode)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

#### Fields

##### `codigoErrorRegistro` → `Integer`

##### `descripcionErrorRegistro` → `String`

##### `estadoRegistro` → `String`

---

---
