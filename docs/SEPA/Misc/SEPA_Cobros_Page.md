---
layout: default
nav_exclude: true
---

# SEPA_Cobros_Page

`APIVERSION: 52`

`STATUS: ACTIVE`

Custom controller para la VF SEPA_Cobros_Page

**Author** Oriol Farras

**Group** Misc

## Constructors

### `SEPA_Cobros_Page()`

---

## Fields

### `TIPOCONFIGURACION` → `String`

---

## Properties

### `CreDtTm` → `String`

### `FechaFactura` → `String`

### `IdCobro` → `String`

### `MsgId` → `String`

### `NumFacturas` → `Integer`

### `OrgBIC` → `String`

### `OrgCP` → `String`

### `OrgCity` → `String`

### `OrgContact` → `String`

### `OrgEmail` → `String`

### `OrgIBAN` → `String`

### `OrgId` → `String`

### `OrgName` → `String`

### `OrgPais` → `String`

### `OrgStreet` → `String`

### `OrgStreetNum` → `String`

### `SumFacturas` → `String`

### `TipoRemesa` → `String`

### `header` → `String`

### `idAcreedor` → `String`

### `listaFacturas` → `List<WrapFactura>`

---

## Methods

### `Init()`

### `getPmtInfId(List<WrapFactura> lista)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `getTotalImporte(List<WrapFactura> listaFacturas)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `setWrapperCobros(CC_SII_FacturaObj factura)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---

## Classes

### WrapFactura

#### Properties

##### `BIC` → `String`

##### `DeudorCP` → `String`

##### `DeudorCity` → `String`

##### `DeudorDir1` → `String`

##### `DeudorDir2` → `String`

##### `DeudorNom` → `String`

##### `DeudorPais` → `String`

##### `IBANCliente` → `String`

##### `Id` → `String`

##### `IdCompleto` → `String`

##### `Importe` → `String`

##### `MandatoFecha` → `String`

##### `MandatoId` → `String`

##### `NumFactura` → `String`

##### `OrgBIC` → `String`

##### `OrgCP` → `String`

##### `OrgCity` → `String`

##### `OrgContact` → `String`

##### `OrgEmail` → `String`

##### `OrgId` → `String`

##### `OrgName` → `String`

##### `OrgPais` → `String`

##### `OrgStreet` → `String`

##### `OrgStreetNum` → `String`

##### `Prioridad` → `String`

##### `Proposito` → `String`

##### `TipoRemesa` → `String`

##### `Ustrd` → `String`

##### `fecha` → `String`

##### `idAcreedor` → `String`

---

---
