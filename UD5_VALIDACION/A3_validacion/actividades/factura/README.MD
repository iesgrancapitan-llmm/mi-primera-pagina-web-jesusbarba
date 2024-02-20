# Ejercicio 1 XSD - Factura

## 1. Crea un XSD que valide este [fichero XML](ej1factura.xml)

### Debes tener en cuenta las siguientes consideraciones.
- El método de diseño del fichero XSD debe ser mediante definición de tipos.
- La factura debe tener una cabecera y al menos un apunte.
### La cabecera contendrá la fecha y la información de cliente.

### El cliente tiene 3 atributos:
- cliente_id es un identificador obligatorio
- nombre: no es obligatorio
- teléfono: no es obligatorio
### La dirección del cliente tiene los elementos nombre_via, numero, localidad, provincia, cp y país.

### Pais es un elemento que no es obligatorio.

### El nombre_via tiene un atributo tipo_via con los siguientes posibles valores

### Calle, Avda, Plaza o Carretera. Por defecto el valor el calle.

### Cada apunte debe tener un concepto.

### El apunte tiene los siguientes atributos
- Precio: Atributo obligatorio.
- Descuento puede tener los valores “promoción” o “regular” por defecto el valor
será regular.
- Moneda será un atributo fijo cuyo valor es “euro”.

### El concepto tiene el atributo cantidad que no es obligatorio.
### En la fecha los elementos pueden aparecer en el orden dia, mes, año o mes, dia, año

**[XSD](ej1factura.xsd)**