# DAX I

**DAX**: Data Analysys Expression

## Crear "New Measure" / "nueva medida"

1. Clic derecho en "inspector" de datos (lado derecho de vista reporte)

2. Clic en "Nueva medida"

3. Dar nombre y escribir DAX

## Contexto de filtro / Filter context

### CALCULATE

Evalúa una expresión en un filter context modificado por filtros.

- Se pueden agregar **filtros directos** en los argumentos 2,3,... de CALCULATE
- Se pueden agregar **filtros directos** de **otras tablas** en los argumentos de filtros en CALCULATE, siempre y cuando las tablas estén conectadas en el modelo de datos
- En casos cuando un filtro contenga una DAX, se necesita usar la función [FILTER](#filter)

### ALL, ALLEXCEPT

Funciones que se usan en conjunto con CALCULATE.

- **ALL:** Quita la columna o tabla del filter context para esa expresión.

- **ALLEXCEPT:** Quita todas las columnas de una tabla del filter context excpetuando las especificadas.

### FILTER

Dada una tabla y una condición (DAX booleana), devuelve un subconjunto de la tabla basado en la condición dada.

## VAR

Función DAX que proporciona flexibilidad al escribir funciones complejas. Es como asignar una medida o una subtabla a una variable

### RETURN

Valor que se regresará después de usar VAR para algún cálculo.

## Columnas calculadas

En la vista de tabla (barra lateral, segunda opción) se pueden crear nuevas columnas, las cuales son definidas por expresiones DAX. Estas se llaman columnas calculadas.

## RELATEDTABLE

