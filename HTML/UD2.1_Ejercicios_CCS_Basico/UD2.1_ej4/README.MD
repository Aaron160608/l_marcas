# Respuestas Ejercicio 4

# Error obtenido al duplicar un ID en la validacion de W3C
Al colocar el atributo id="corp" en mas de un elemento en el archivo HTML, el validador oficial del W3C devuelve el siguiente mensaje de error: Error: Duplicate ID `corp`.

# ¿Por que se desaconseja usar selectores de id para aplicar estilos CSS?
Se desaconseja utilizar selectores de ID para poner estilos CSS porque:
*Reutilizacion imposible*: Los identificadores tienen que ser unicos en toda la pagina HTML
*Especificidad desmedida*: Los selectores de ID tiene un peso de especificidad muy alto, la dificulta de sobrescribir sus reglas sin recurrir a malas practicas.
*Buenas practicas*: La recomendacion general en maquetacion moderna es emplear *clases* para definir estilos CSS y reservar los ID solo para anclas de navegacion con JavaScript.