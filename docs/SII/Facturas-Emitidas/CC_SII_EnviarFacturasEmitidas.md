---
layout: default
title: Facturas Emitidas
nav_order: 4
parent: Facturas Emitidas
---

# CC_SII_EnviarFacturasEmitidas

`APIVERSION: 52`

`STATUS: ACTIVE`

Envio de facturas emitidas

**Author** Oriol Farras

**Group** Facturas Emitidas

**Date** 2022

## Fields

### `SIILR_NS` → `String`

### `SIILR_PRE` → `string`

### `SII_NS` → `String`

### `SII_PRE` → `string`

### `config` → `CC_ConfigEnvioSII__c`

### `tipoenvio` → `String`

### `tiporectificativa` → `String`

---

## Methods

### `static enviarFacturas(List<CC_SII_FacturaObj> facturas, String tipoenvio, String tipoConfiguracion)`

#### Parameters

| Param | Description |
| ----- | ----------- |

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

**Author** Oriol Farras | 12/9/2019

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

**Author** Oriol Farras | 12/9/2019

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

**Author** Oriol Farras | 12/9/2019

### `static rellenarFacturaExpedida(Dom.XmlNode facturaExpedida, CC_SII_FacturaObj factura)`

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

**Author** Oriol Farras | 12/9/2019

### `static generarRegistroLRFacturasEmitidas(Dom.XmlNode registroLRFacturasEmitidas, CC_SII_FacturaObj factura)`

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

**Author** Oriol Farras | 12/9/2019

### `static rellenarXMLFacturasEmitidas(Dom.XmlNode methodNode, List<CC_SII_FacturaObj> facturas)`

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

**Author** Oriol Farras | 12/9/2019

---
