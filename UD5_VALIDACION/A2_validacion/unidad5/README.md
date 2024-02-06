# UD5. A5. DTD - Factura

## Autor: Jesús Pablo Barba Reyes

## Asignatura: Lenguaje de Marcas

Crea un DTD externo que valide el fichero xml ej5_factura.xml.

Debes tener en cuenta las siguientes consideraciones.

La factura debe tener una cabecera y al menos un apunte.

La cabecera contendrá la fecha y la información de cliente.

El cliente tiene 3 atributos:

- cliente_id es un identificador obligatorio.
- nombre: no es obligatorio.
- teléfono: no es obligatorio.

La dirección del cliente tiene los elementos nombre_via, numero, localidad, provincia, cp y país.

País es un elemento que no es obligatorio.

El nombre_via tiene un atributo tipo_via con los siguientes posibles valores.

    Calle, Avda, Plaza o Carretera. Por defecto el valor es calle.

Cada apunte debe tener un concepto.

El apunte tiene los siguientes atributos:

-   Precio: Atributo obligatorio.
-   Descuento puede tener los valores "promoción" o "regular" por defecto es valor será regular.
-   Moneda srá un atributo fijo cuyo valor es "euro".

El concepto tiene el atributo cantidad que no es obligatorio.

En la fecha los elementos pueden aparecer en el orden día, mes, año o mes, dia, año.

[XML ejercicio](./ejercicio5/ej5_factura.xml)

[DTD ejercicio](./ejercicio5/validacionej5.dtd)