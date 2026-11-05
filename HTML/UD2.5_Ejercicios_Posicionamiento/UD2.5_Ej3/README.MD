# Ejercicio 3: Tarjeta y Scroll

# Parte A: Posicionamiento de la etiqueta y overflow
*Elemento con position: relative:* La tarjeta contenedora necesita tener position: relative para que la etiqueta etiquetada con position: absolute tome las referencias de coordenadas respecto a la propia tarjeta y no respecto a toda la pantalla.
*Efecto de overflow: hidden:* Si se le pone overflow: hidden a la tarjeta, la parte de la etiqueta -20% que sobresale de las esquinas se recorta y desaparece. Para solucionarlo, hay que quitar esa propiedad de la tarjeta contenedora para permitir que los elementos posicionados afuera se vean.

# Parte B: Pruebas de overflow y visibility vs display

# 1. Valores de overflow:
*visible:* El contenido se sale de la caja y se sobrepone al resto de cosas.
*hidden:* Lo que no cabe se corta y desaparece sin opcion a verlo.
*scroll:* Pone barras de desplazamiento siempre, quepan o no los textos.
*auto:* Muestra la barra de scroll solo si el contenido sobrepasa las dimensiones de la caja (es la solucion mas limpia).

# 2. Diferencia entre visibility: hidden y display: none:
*visibility: hidden:* Oculta el elemento visualmente, pero sigue manteniendo el hueco físico que ocupaba en la pantalla.
*display: none:* Elimina el elemento del flujo por completo. No se ve y tampoco deja ningún tipo de espacio, haciendo que las demás cajas se muevan y ocupen su lugar.