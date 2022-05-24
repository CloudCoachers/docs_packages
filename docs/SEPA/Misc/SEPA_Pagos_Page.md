---
layout: default
nav_exclude: true
---

# SEPA_Pagos_Page

`APIVERSION: 53`

`STATUS: ACTIVE`

Custom controller para la VF SEPA_Pagos

**Author** Oriol Farras

**Group** Misc

## Constructors

### `SEPA_Pagos_Page()`

---

## Fields

### `IBAN` → `String`

### `TIPOCONFIGURACION` → `String`

### `limiteConcepto` → `integer`

---

## Properties

### `CreDtTm` → `String`

### `CtgyPurp` → `String`

### `FechaFactura` → `String`

### `IdPago` → `String`

### `IdUltimoDeudor` → `String`

### `MsgId` → `String`

### `NomUltimodeudor` → `String`

### `NumFacturas` → `Integer`

### `OrgBIC` → `String`

### `OrgCP` → `String`

### `OrgCity` → `String`

### `OrgDir1` → `String`

### `OrgDir2` → `String`

### `OrgIBAN` → `String`

### `OrgId` → `String`

### `OrgIdOther` → `String`

### `OrgName` → `String`

### `OrgPais` → `String`

### `Prioridad` → `String`

### `SumFacturas` → `String`

### `TipoRemesa` → `String`

### `chrgBr` → `String`

### `header` → `String`

### `instrPrty` → `String`

### `listaFacturas` → `List<WrapFactura>`

### `svcLvl` → `String`

---

## Methods

### `Init()`

### `setWrapperPagos(CC_SII_FacturaObj factura)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `getPmtInfId(List<WrapFactura> lista)`

#### Parameters

| Param | Description |
| ----- | ----------- |

### `getTotalImporte(List<WrapFactura> listaFacturas)`

#### Parameters

| Param | Description |
| ----- | ----------- |

---

## Classes

### WrapFactura

#### Properties

##### `AcreCP` → `String`

##### `AcreCity` → `String`

##### `AcreDir1` → `String`

##### `AcreDir2` → `String`

##### `AcreIBAN` → `String`

##### `AcreID` → `String`

##### `AcreNom` → `String`

##### `AcrePais` → `String`

##### `AcrePurp` → `String`

##### `BIC` → `String`

##### `Fecha` → `String`

##### `IdCompleto` → `String`

##### `IdUltimoDeudor` → `String`

##### `Importe` → `String`

##### `NomUltimodeudor` → `String`

##### `NumFactura` → `String`

##### `OrgBIC` → `String`

##### `OrgCP` → `String`

##### `OrgCity` → `String`

##### `OrgDir1` → `String`

##### `OrgDir2` → `String`

##### `OrgIBAN` → `String`

##### `OrgIdOther` → `String`

##### `OrgName` → `String`

##### `OrgPais` → `String`

##### `Prioridad` → `String`

##### `UltmtCdtr` → `String`

##### `UltmtCdtrId` → `String`

##### `Ustrd` → `String`

---

---
