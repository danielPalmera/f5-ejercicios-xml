Cambia el DTD siguiente (ejemplo pg9) 
de tal manera que dia, mes, anyo sean atributos dia y mes requeridos y anyo con valor “2000” fijado. Y haz un xml que valide y esté bien formado.
<!DOCTYPE persona [
	<!ELEMENT persona (nombre, mujer, fecha_de_nacimiento, ciudad)>
	<!ELEMENT nombre (#PCDATA)>
<!ELEMENT mujer EMPTY>
	<!ELEMENT fecha_de_nacimiento (dia, mes, anyo)>
<!ELEMENT dia (#PCDATA)>
<!ELEMENT mes (#PCDATA)>
<!ELEMENT anyo (#PCDATA)>
<!ELEMENT ciudad (#PCDATA)>
]>