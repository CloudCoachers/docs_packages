---
layout: default
nav_exclude: true
---

# CC_CreateSEPA

`APIVERSION: 52`

`STATUS: ACTIVE`

Custom controller para la creación de ficheros SEPA

**Author** Oriol Farras

**Group** Misc

## Fields

### `FACTURAS_GENERADAS` → `string`

### `FACTURAS_RECIBIDAS` → `string`

### `MAX_RESULTS` → `Integer`

---

## Methods

### `static CreateSEPA(String jsonDatos, List<String> idsFacturas, String recordId)`

`AURAENABLED`

Metodo para crear un fichero dados los datos de la facturas recibidas

#### Parameters

| Param         | Description |
| ------------- | ----------- |
| `tipoFactura` |             |
| `idsFacturas` |             |

#### Return

**Type**

string

**Description**

string

**Author** Oriol Farras | 11-23-2021

### `static updateSEPA(String jsonDatos, String recordId)`

`AURAENABLED`

metodo para actualizar una remesa en el caso de haber eliminado alguna factura de la misma

#### Parameters

| Param       | Description |
| ----------- | ----------- |
| `jsonDatos` |             |
| `recordId`  |             |

#### Return

**Type**

string

**Description**

string

**Author** Oriol Farras | 05-24-2022

### `static esRecibida(String tipo)`

validar si es recibida o emitida

#### Parameters

| Param  | Description |
| ------ | ----------- |
| `tipo` |             |

#### Return

**Type**

Boolean

**Description**

Boolean

**Author** Oriol Farras | 12-20-2021

### `static crearSEPAFile(String nombre, FicheroSEPA__c registro, Blob xmlBlob)`

Metodo para crear un fichero con los datos de la remesa y lo almacena en el registro de fichero sepa

#### Parameters

| Param      | Description |
| ---------- | ----------- |
| `nombre`   |             |
| `registro` |             |
| `xmlBlob`  |             |

#### Return

**Type**

Boolean

**Description**

Boolean

**Author** Oriol Farras | 12-20-2021

### `static getOrgBanks(String tipoConfiguracion)`

`AURAENABLED`

Metodo que devuelve todos los bancos

#### Parameters

| Param               | Description |
| ------------------- | ----------- |
| `tipoConfiguracion` |             |

#### Return

**Type**

string

**Description**

string

**Author** Oriol Farras | 12-20-2021

### `static updateRegistrosEnviados(List<String> idsFacturas, String tipoConfiguracion, FicheroSEPA__c registroSEPA)`

Metodo que marca las facturas como enviadas al SEPA

#### Parameters

| Param               | Description           |
| ------------------- | --------------------- |
| `idsFacturas`       | ids de las facturas   |
| `tipoConfiguracion` | tipo de configuración |
| `registroSEPA`      | id del registro sepa  |

**Author** Oriol Farras

### `static lookupSearch(String searchTerm, String tipoFactura)`

`AURAENABLED`

Metodo que devuelve el numero de remesa para el filtro de numero remesa

#### Parameters

| Param         | Description |
| ------------- | ----------- |
| `searchTerm`  |             |
| `tipoFactura` |             |

#### Return

**Type**

List&lt;LookupSearchResult&gt;

**Description**

List&lt;LookupSearchResult&gt;

**Author** Oriol Farras

### `static addRemesas(List<String> ids, String idFicheroSEPA, String fieldClass, String tipoConfiguracion)`

`AURAENABLED`

Metodo para añadir a un remesa existente nuevas facturas

#### Parameters

| Param               | Description |
| ------------------- | ----------- |
| `ids`               |             |
| `idFicheroSEPA`     |             |
| `fieldClass`        |             |
| `tipoConfiguracion` |             |

#### Return

**Type**

String

**Description**

String

**Author** Oriol Farras

---

## Classes

### wrapperBank

Innner class para guardar los datos bancarios

#### Properties

##### `label` → `string`

##### `value` → `string`

---

#### Methods

##### `setValues(CC_SII_FacturaObj banco)`

###### Parameters

| Param | Description |
| ----- | ----------- |

---

### wrapperDatos

Innner class para guardar los datos del registro sepa

#### Properties

##### `IBAN` → `string`

##### `fecharemesa` → `date`

##### `nombre` → `string`

##### `tipoFactura` → `string`

##### `tiporemesa` → `string`

---

---
