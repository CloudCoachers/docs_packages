---
layout: default
title: Log
parent: Misc
nav_order: 1
---

# Log

`APIVERSION: 54`

`STATUS: ACTIVE`

Class with loogin options

**Author** Oriol Farras

**Date** 04/2022

**Group** Misc

## Fields

### `CLASSNAME` → `String`

### `IS_ENABLED` → `Boolean`

### `ORG_NAMESPACE` → `String`

### `STACK_LINE` → `Pattern`

### `log` → `Log__e`

---

## Methods

### `static debug()`

debug without parameters

**Author** Oriol Farras | 05-24-2022

### `static debug(String message)`

debug with message

#### Parameters

| Param     | Description    |
| --------- | -------------- |
| `message` | message to log |

**Author** Oriol Farras | 05-24-2022

### `static debug(List<Object> values)`

debug with list of objects

#### Parameters

| Param    | Description   |
| -------- | ------------- |
| `values` | values to log |

**Author** Oriol Farras | 05-24-2022

### `static debug(String message, List<Object> values)`

debug with message an list of objects

#### Parameters

| Param     | Description    |
| --------- | -------------- |
| `message` | message to log |
| `values`  | values to log  |

**Author** Oriol Farras | 05-24-2022

### `static debug(String message, List<Object> values, LogLocation loglocationdata)`

debug with message list of objects and location for packages

#### Parameters

| Param             | Description         |
| ----------------- | ------------------- |
| `message`         | message to log      |
| `values`          | values to log       |
| `loglocationdata` | {@link LogLocation} |

**Author** Oriol Farras | 05-24-2022

### `static error()`

error without parameters

**Author** Oriol Farras | 05-24-2022

### `static error(List<Object> values)`

error log with list of objects

#### Parameters

| Param    | Description         |
| -------- | ------------------- |
| `values` | values to log error |

**Author** Oriol Farras | 05-24-2022

### `static error(String message)`

error log with message

#### Parameters

| Param     | Description   |
| --------- | ------------- |
| `message` | error message |

**Author** Oriol Farras | 05-24-2022

### `static error(String message, List<Object> values)`

error log with message and list of objects

#### Parameters

| Param     | Description   |
| --------- | ------------- |
| `message` | error meesage |
| `values`  | values list   |

**Author** Oriol Farras | 05-24-2022

### `static error(String message, List<Object> values, LogLocation loglocationdata)`

log error with message, list of objects and location for packages

#### Parameters

| Param             | Description                           |
| ----------------- | ------------------------------------- |
| `message`         | error message                         |
| `values`          | list of values                        |
| `loglocationdata` | location of error {@link LogLocation} |

**Author** Oriol Farras | 05-24-2022

### `static emit(String message, List<Object> values, LoggingLevel level, LogLocation loglocationdata)`

`SUPPRESSWARNINGS`

method to emit platform event

#### Parameters

| Param             | Description                           |
| ----------------- | ------------------------------------- |
| `message`         | message to emit                       |
| `values`          | list of values to format              |
| `level`           | level of logging                      |
| `loglocationdata` | location of error {@link LogLocation} |

**Author** Oriol Farras | 05-24-2022

### `static cast(List<Object> values)`

method to cast to string object values

#### Parameters

| Param    | Description    |
| -------- | -------------- |
| `values` | values to cast |

#### Return

**Type**

List&lt;String&gt;

**Description**

List&lt;String&gt;

**Author** Oriol Farras | 05-24-2022

### `static storeLocation(Map<String,Object> data)`

method to get location of error

#### Parameters

| Param  | Description            |
| ------ | ---------------------- |
| `data` | data to store location |

**Author** Oriol Farras | 05-24-2022

### `static className(Matcher matcher)`

method to get classname

#### Parameters

| Param     | Description     |
| --------- | --------------- |
| `matcher` | matcher pattern |

#### Return

**Type**

String

**Description**

String

**Author** Oriol Farras | 05-24-2022

### `static methodName(Matcher matcher)`

method to get methodname

#### Parameters

| Param     | Description     |
| --------- | --------------- |
| `matcher` | matcher pattern |

#### Return

**Type**

String

**Description**

String

**Author** Oriol Farras | 05-24-2022

### `static hasNamespace(Matcher matcher)`

method to determine if has namespace

#### Parameters

| Param     | Description     |
| --------- | --------------- |
| `matcher` | matcher pattern |

#### Return

**Type**

Boolean

**Description**

Boolean

**Author** Oriol Farras | 05-24-2022

### `static prettyMethod(String method)`

method to prettify method name

#### Parameters

| Param    | Description        |
| -------- | ------------------ |
| `method` | method to pretiffy |

#### Return

**Type**

String

**Description**

String

**Author** Oriol Farras | 05-24-2022

### `static isEnabled()`

method to determine if looging is enabled

#### Return

**Type**

Boolean

**Description**

Boolean

**Author** Oriol Farras | 05-24-2022

### `static currentEvent()`

`TESTVISIBLE`

method to get current event for testing poupouses

#### Return

**Type**

Log\_\_e

**Description**

Boolean

**Author** Oriol Farras | 05-24-2022

---
