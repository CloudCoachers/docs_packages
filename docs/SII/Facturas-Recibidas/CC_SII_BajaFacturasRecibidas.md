---
layout: default
---
# CC_SII_BajaFacturasRecibidas

`APIVERSION: 52`

`STATUS: ACTIVE`

Baja de facturas recibidas


**Author** Oriol Farras


**Group** Facturas Recibidas


**Date** 2022

## Fields

### `SIILR_NS` → `String`


### `SIILR_PRE` → `string`


### `SII_NS` → `String`


### `SII_PRE` → `string`


### `config` → `CC_ConfigEnvioSII__c`


---
## Methods
### `static bajaFacturas(List<CC_SII_FacturaObj> facturas, String tipoConfiguracion)`

Metodo para enviar bajas al SII bajas de facturas emitidas

#### Parameters
|Param|Description|
|---|---|
|`facturas`|lista de facturas a dar de baja|
|`tipoConfiguracion`|Nombre de la configuración de SII_Facturas_Object__mdt|

#### Return

**Type**

String

**Description**

Resultado


**Author** Oriol Farras | 05-24-2022

### `static generarCabecera(Dom.XmlNode cabecera, CC_SII_FacturaObj factura)`

Metodo para generar la cabecera del suministro de facturas emitidas

#### Parameters
|Param|Description|
|---|---|
|`Cabecera`|Nodo XML donde anidar los datos de la cabecera|

#### Return

**Type**

void

**Description**

void


**Author** Oriol Farras  | 01/10/2021

### `static rellenarPeriodoLiquidacion(Dom.XmlNode periodoLiquidacion, CC_SII_FacturaObj factura)`

Periodo de liquidación de la factura

#### Parameters
|Param|Description|
|---|---|
|`PeriodoLiquidacion`|Nodo XML donde anidar los datos de periodo de liquidación|
|`factura`|Factura de donde extraer los datos de liquidación|

#### Return

**Type**

void

**Description**

void


**Author** Oriol Farras  | 01/10/2021

### `static rellenarIdFactura(Dom.XmlNode idFactura, CC_SII_FacturaObj factura)`

Metodo que rellena los datos del nodo IDFactura

#### Parameters
|Param|Description|
|---|---|
|`idFactura`|Nodo XML donde vamos a anidar la informacion|
|`factura`|Factura de donde vamos a recoger los datos|

#### Return

**Type**

void

**Description**

void


**Author** Oriol Farras  | 01/10/2021

### `static generarRegistroLRBajaRecibidas(Dom.XmlNode registroLRBajaRecibidas, CC_SII_FacturaObj factura)`

Metodo que genera el arbol xml RegistroLRFacturasemitidas

#### Parameters
|Param|Description|
|---|---|
|`RegistroLRFacturasEmitidas`|Nodo en el que anidar el registro de facturas emitidas|
|`factura`|Factura de donde vamos a extraer los datos|

#### Return

**Type**

void

**Description**

void


**Author** Oriol Farras  | 01/10/2021

### `static rellenarXMLBajaFacturasRecibidas(Dom.XmlNode methodNode, List<CC_SII_FacturaObj> facturas)`

Metodo que genera el xml para la factura/s entradas por parametro

#### Parameters
|Param|Description|
|---|---|
|`methodNode`|Nodo XML donde anidar las facturas|
|`facturas`|lista de tipo factura__c con las facturas a enviar|

#### Return

**Type**

void

**Description**

void


**Author** Oriol Farras  | 01/10/2021

---
## Classes
### IdEmisorFactura

Inner class para almacenar y generar el nodo de id del emisor factura

#### Constructors
##### `IdEmisorFactura()`
---
#### Fields

##### `IdOtro` → `IdOtro`


##### `NIF` → `String`


##### `NombreRazon` → `String`


---
#### Methods
##### `populateXmlNode(Dom.XmlNode outerNode)`
###### Parameters
|Param|Description|
|---|---|

---

### IdFactura

Inner class para almacenar y generar el nodo de id de la factura

#### Constructors
##### `IdFactura()`
---
#### Fields

##### `FechaExpedicionFacturaEmisor` → `String`


##### `IdEmisorFactura` → `IdEmisorFactura`


##### `NumSerieFacturaEmisor` → `string`


---
#### Methods
##### `populateXmlNode(Dom.XmlNode outerNode)`
###### Parameters
|Param|Description|
|---|---|

---

### IdOtro

Inner class para almacenar y generar el nodo de id si es de otro pais

#### Constructors
##### `IdOtro()`
---
#### Fields

##### `CodigoPais` → `String`


##### `ID` → `String`


##### `IDType` → `String`


---
#### Methods
##### `populateXmlNode(Dom.XmlNode outerNode)`
###### Parameters
|Param|Description|
|---|---|

---

---
