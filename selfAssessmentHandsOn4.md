En esta cuarta entrega hemos usado nuestro dataset previamente refinado en la tercera entrega y nos hemos centrado en crear un archivo RML Mapping para transformar nuestro dataset a RDF. Para la transformación hemos usado la herramienta morph-kgc, la cual nos permitió generar el archivo RDF final.

Basándonos en la plantilla y en el archivo RML Mapping que recibimos como ejemplo, fuimos asignando nombres de referencia, datatypes y otros elementos necesarios. Debido a que el dataset es tan grande, había columnas cuyo datatype parecía obvio, pero tuvimos que cambiarlo porque algunas filas no cumplían ese tipo. Por ejemplo, la categoría "numero" tuvo accidentes que ocurrieron en la autovía y se reportaron con valores como "11NL91", lo cual no nos permitió usar xsd:integer para esa columna y tuvimos que emplear xsd:string.

Otro ejemplo similar son las columnas positiva_alcohol y positiva_droga. Aunque lo lógico hubiese sido usar xsd:boolean, no a todos los individuos se les realizaron ambas pruebas, por lo tanto tuvimos que volver a usar xsd:string.

Después utilizamos la herramienta morph-kgc, a la cual le proporcionamos nuestro dataset (archivo CSV), nuestro archivo RML Mapping y el archivo config.ini, y nos devolvió el archivo RDF deseado en sintaxis N-Triples.

## Archivos entregados

1. 2025_Accidentalidad.csv
    - Nuestro dataset obtenido en la entrega número 3.

1. mapping.rml.ttl
    - El archivo que utilizamos para convertir nuestro dataset a RDF.

2. config.ini
    - archivo auxiliar para la transformación a RDF.

3. accidentes.nt
    - archivo RDF generado en formato NTriples.


## Conclusión
