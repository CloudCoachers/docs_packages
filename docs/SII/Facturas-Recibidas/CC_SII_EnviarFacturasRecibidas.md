---
layout: default
title: Facturas Recibidas
nav_order: 4
parent: Facturas Recibidas
---

# CC_SII_EnviarFacturasRecibidas

`APIVERSION: 52`

`STATUS: ACTIVE`

Clase con los metodos para enviar de facturas recibidas

**Author** Oriol Farras

**Group** Facturas Recibidas

**Date** 2022

## Fields

### `RECARGOEQMAP` → `Map<String,String>`

### `TIPOSIVALIST` → `List<String>`

### `config` → `CC_ConfigEnvioSII__c`

### `tipoenvio` → `string`

### `tiporectificativa` → `string`

---

## Methods

### `static enviarFacturasRecibidasSII(List<CC_SII_FacturaObj> facturas, String tipoenvio, String tipoConfiguracion)`

metodo que envia al sii las facturas pasasdas por parametro

#### Parameters

| Param               | Description                                   |
| ------------------- | --------------------------------------------- |
| `facturas`          | lista con el tipo abstracto CC_SII_FacturaObj |
| `tipoenvio`         | tipo de envio                                 |
| `tipoConfiguracion` | tipo de configuración                         |

#### Return

**Type**

String

**Description**

Resultado del envio

**Author** Oriol Farras

### `static rellenarXMLFacturasRecibidas(Dom.XmlNode methodNode, List<CC_SII_FacturaObj> facturas)`

Metodo que genera el xml para la factura/s entradas por parametro

#### Parameters

| Param        | Description                                          |
| ------------ | ---------------------------------------------------- |
| `methodNode` | Nodo XML donde anidar las facturas                   |
| `facturas`   | lista de tipo factura\_\_c con las facturas a enviar |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static generarCabecera(Dom.XmlNode cabecera, CC_SII_FacturaObj factura)`

Metodo para generar la cabecera del suministro de facturas emitidas

#### Parameters

| Param      | Description                                    |
| ---------- | ---------------------------------------------- |
| `cabecera` | Nodo XML donde anidar los datos de la cabecera |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static generarRegistroLRFacturasRecibidas(Dom.XmlNode registroLRFacturasEmitidas, CC_SII_FacturaObj factura)`

Metodo que genera el arbol xml RegistroLRFacturasemitidas

#### Parameters

| Param                        | Description                                            |
| ---------------------------- | ------------------------------------------------------ |
| `registroLRFacturasEmitidas` | Nodo en el que anidar el registro de facturas emitidas |
| `factura`                    | Factura de donde vamos a extraer los datos             |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static rellenarPeriodoLiquidacion(Dom.XmlNode periodoLiquidacion, CC_SII_FacturaObj factura)`

Periodo de liquidación de la factura

#### Parameters

| Param                | Description                                               |
| -------------------- | --------------------------------------------------------- |
| `PeriodoLiquidacion` | Nodo XML donde anidar los datos de periodo de liquidación |
| `factura`            | Factura de donde extraer los datos de liquidación         |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static rellenarIdFactura(Dom.XmlNode idFactura, CC_SII_FacturaObj factura)`

Metodo que rellena los datos del nodo IDFactura

#### Parameters

| Param       | Description                                  |
| ----------- | -------------------------------------------- |
| `idFactura` | Nodo XML donde vamos a anidar la informacion |
| `factura`   | Factura de donde vamos a recoger los datos   |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static rellenarFacturaRecibida(Dom.XmlNode facturaRecibida, CC_SII_FacturaObj factura)`

Metodo para rellenar el contenido de la factura

#### Parameters

| Param             | Description                                     |
| ----------------- | ----------------------------------------------- |
| `facturaExpedida` | nodo donde anidar los valores de la factura     |
| `factura`         | factura de donde extraeremos los datos a enviar |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static rellenarDesglose(Dom.XmlNode facturaRecibida, CC_SII_FacturaObj factura)`

Metodo para rellenar el contenido de la factura

#### Parameters

| Param             | Description                                     |
| ----------------- | ----------------------------------------------- |
| `facturaExpedida` | nodo donde anidar los valores de la factura     |
| `factura`         | factura de donde extraeremos los datos a enviar |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

### `static rellenarsujetoPasivo(Dom.XmlNode facturaRecibida, CC_SII_FacturaObj factura)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `static rellenarDesgloseIVA(Dom.XmlNode facturaRecibida, CC_SII_FacturaObj factura)`

metodo para rellenar el bloque desglose iva

#### Parameters

| Param             | Description                           |
| ----------------- | ------------------------------------- |
| `facturaRecibida` | nodo XML facturaRecibida              |
| `factura`         | Objecto de facturas CC_SII_FacturaObj |

**Author** Oriol Farras

### `static rellenarContraparte(Dom.XmlNode facturaRecibida, CC_SII_FacturaObj factura)`

Metodo para rellenar el contenido del nodo de contraparte

#### Parameters

| Param             | Description                                     |
| ----------------- | ----------------------------------------------- |
| `facturaExpedida` | nodo donde anidar los valores de la factura     |
| `factura`         | factura de donde extraeremos los datos a enviar |

#### Return

**Type**

void

**Description**

void

**Author** Oriol Farras | 01/10/2021

---
