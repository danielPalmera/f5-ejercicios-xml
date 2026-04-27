Escribir un DTD que valide una biblioteca de libros que contengan un ISBN único, usuarios que contengan un DNI único y préstamos de libros  a usuarios . Utiliza Un DTD empleando los atributos ID i IDREF . Además clasifica los libros según si son: clásico, novela o teatro,  siendo por defecto un clásico.
<?xml version="1.0" encoding="UTF-8"?>
<biblioteca>
  	<libro ISBN="A978849759251" titulo="La Celestina" tipo=”clasico”/>
  	<libro ISBN="A8481301264 " titulo="El nombre de la Rosa"/>
	 <libro ISBN="A9788497592581" titulo="Don Juan" tipo=”teatro”/>
  	
  	<usuario DNI="Z47673211" nombre="Antonio"/>
  	<usuario DNI="Z47673212" nombre="Maria"/>
  	
   	<prestamo DNI="Z47673211" ISBN="A8481301264 A9788497592581"/>
</biblioteca>