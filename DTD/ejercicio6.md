Escribir un DTD que valide una librería de libros que contenga un ISBN único, ten en cuenta que el parámetro ID tiene que empezar por un caràcter no numérico
<?xml version="1.0" encoding="UTF-8"?>
<libreria>
	<libro ISBN="A9788497592581" titulo="El origen de las especies"/>
  	<libro ISBN="A978849759251" titulo="La Celestina"/>
  	<libro ISBN="A8481301264" titulo="El nombre de la Rosa"/>
</libreria>

Ahora añade una compra / un ticket en el cual se esté haciendo referencia a uno de los libros de la librería (IDREF).

Solucion propuesta:

DTD (ejercicio6.dtd)
<!ELEMENT libreria (libro+, ticket+)>

<!ELEMENT libro EMPTY>
<!ATTLIST libro
	ISBN ID #REQUIRED
	titulo CDATA #REQUIRED>

<!ELEMENT ticket EMPTY>
<!ATTLIST ticket
	idTicket ID #REQUIRED
	refLibro IDREF #REQUIRED
	cantidad CDATA #REQUIRED>

XML valido (ejercicio6.xml)
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE libreria SYSTEM "ejercicio6.dtd">
<libreria>
	<libro ISBN="A9788497592581" titulo="El origen de las especies"/>
	<libro ISBN="A9788497592511" titulo="La Celestina"/>
	<libro ISBN="A8481301264" titulo="El nombre de la Rosa"/>

	<ticket idTicket="T001" refLibro="A9788497592581" cantidad="1"/>
</libreria>