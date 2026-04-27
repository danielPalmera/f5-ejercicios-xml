Basándose en el XML base de ejercicio1.xml, se generaron nuevas versiones de XML y DTD con estos cambios:

2.1 Dos apellidos
- Cambio en DTD: en Empleado se exige Apellido dos veces seguidas.
- Modelo usado: (Apellido, Apellido, Nombre, NumEmpleado, Email, Telefono, Direccion)
- Cambio en XML: el empleado incluye dos etiquetas Apellido.
- Archivos: ejercicio2.1.dtd y ejercicio2.1.xml.

2.2 Email o Telefono (solo uno)
- Cambio en DTD: se usa una eleccion para permitir Email o Telefono, pero no ambos.
- Modelo usado: (Apellido, Nombre, NumEmpleado, (Email | Telefono), Direccion)
- Cambio en XML: un empleado tiene Email y otro tiene Telefono para demostrar ambos casos validos.
- Archivos: ejercicio2.2.dtd y ejercicio2.2.xml.

2.3 Varios empleados
- Cambio en DTD: Empresa exige al menos dos empleados.
- Modelo usado: (Empleado, Empleado+)
- Cambio en XML: se incluyeron tres empleados.
- Archivos: ejercicio2.3.dtd y ejercicio2.3.xml.

Archivos base de referencia:
- ejercicio1.xml
- ejercicio1.dtd