Autoevaluación – Hands-On Assignment 4
En esta cuarta entrega hemos usado nuestro dataset previamente refinado en la tercera entrega y nos hemos centrado en crear un archivo RML Mapping para transformar nuestro dataset a RDF. Para la transformación hemos usado la herramienta morph-kgc, la cual nos permitió generar el archivo RDF final.
Basándonos en la plantilla y en el archivo RML Mapping que recibimos como ejemplo, fuimos asignando nombres de referencia, datatypes y otros elementos necesarios. Debido a que el dataset es tan grande, había columnas cuyo datatype parecía obvio, pero tuvimos que cambiarlo porque algunas filas no cumplían ese tipo. Por ejemplo, la categoría "numero" tuvo accidentes que ocurrieron en la autovía y se reportaron con valores como "11NL91", lo cual no nos permitió usar xsd:integer para esa columna y tuvimos que emplear xsd:string.
Otro ejemplo similar son las columnas positiva_alcohol y positiva_droga. Aunque lo lógico hubiese sido usar xsd:boolean, no a todos los individuos se les realizaron ambas pruebas, por lo tanto tuvimos que volver a usar xsd:string.
Después utilizamos la herramienta morph-kgc, a la cual le proporcionamos nuestro dataset (archivo CSV), nuestro archivo RML Mapping y el archivo config.ini, y nos devolvió el archivo RDF deseado en sintaxis N-Triples.
Archivos entregados
1.	2025_Accidentalidad.csv
⦁	Nuestro dataset obtenido en la entrega número 3.
2.	mapping.rml.ttl
⦁	El archivo que utilizamos para convertir nuestro dataset a RDF.
3.	config.ini
⦁	archivo auxiliar para la transformación a RDF.
4.	accidentes.nt
⦁	archivo RDF generado en formato NTriples.

Conclusión
El grupo ha cumplido los objetivos del Hands-On 4 de forma completa.
Además, hemos aprendido a definir RML mappings y a transformar datos a RDF mediante la herramienta morph-kgc. No redefine términos ontológicos, cumpliendo las normas de separación entre esquema y datos.
    


## Conclusión

El grupo ha cumplido los objetivos del Hands-On 2 de forma completa.

Además, hemos aprendido a estructurar datos abiertos en RDF, aplicar una naming strategy coherente y desarrollar una ontología válida en OWL.
