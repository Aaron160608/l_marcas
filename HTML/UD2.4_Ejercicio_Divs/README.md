# Respuestas UD 2.4 - Maquetacion con Divs

# 1. Eleccion de maquetacion (Flexbox vs Inline-block)
*Opcion elegida:* He usado display: flex en la caja .contenido.
*Motivo:* Flexbox es mucho mas comodo. Coloca y alinea las tarjetas de los servidores solas y te evita pelear con los saltos de linea o los espacios en blanco que siempre salen al usar inline-block.

# 2. ¿Diferencia entre margin y padding?
*Padding:* Es el margen interno, el espacio de relleno que hay entre el texto, contenido y el borde de su propia caja.
*Margin:* Es la distancia por fuera de la caja, la que sirve para empujar y separarse de las otras cajas de alrededor.

# 3. ¿Por que saltaba la tercera tarjeta de linea al usar inline-block?
*Explicacion:* Porque el ancho real de la caja no eran solo los 220px. Habia que sumarle el padding de los lados (30px), los bordes (2px) y los margenes (20px), asi que cada tarjeta medía en realidad 272px.
*El calculo:* Las tres tarjetas juntas sumaban $3 \times 272\text{px} = 816\text{px}$ . Como el contenedor .pagina solo medía 800px, la tercera tarjeta no cabia de ancho y se iba para abajo.

# 4. ¿Que propiedades ignoraba el <span> y por que?
*Propiedades ignoradas:* El ancho, el alto y los margenes de arriba y abajo.
*Por que:* La etiqueta <span> viene de serie como elemento en linea display: inline, por lo que su tamano depende unicamente del texto que lleve dentro. Para que te haga caso con el ancho y el alto hay que cambiarlo por display: inline-block.

# 5. ¿Que hace display: none con el espacio que ocupaba la caja?
*Respuesta:* Oculta la caja por completo y libera su hueco. Las demas tarjetas se mueven y ocupan su sitio al instante, sin dejar ningun espacio en blanco.