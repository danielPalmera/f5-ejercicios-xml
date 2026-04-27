Dado siguiente DTD escribe 
El árbol de estructura
Un document XML que valide contra el siguiente DTD

<!ELEMENT matricula (ciclo,alumnos)>
<!ELEMENT ciclo (#PCDATA)>
<!ELEMENT alumnos (alumno)+>
<!ELEMENT alumno (nombre,year,asignaturas)>
<!ELEMENT nombre (#PCDATA)>
<!ELEMENT year (#PCDATA)>
<!ELEMENT asignaturas (asignatura)+>
<!ELEMENT asignatura (#PCDATA)>


