# Respuestas UD 3.1 - Ejercicio 1: Laboratorio de Position

# 1. Pruebas con static
*Observacion:* Al poner left: 50px a .c1, el cuadro no se desplaza en absoluto.
*Por que:* Por defecto los elementos son position: static. Con este tipo de posicionamiento las propiedades de desplazamiento (top, bottom, left, right) se ignoran por completo.

# 2. Pruebas con relative
*Observacion:* Al poner .c2 en position: relative con top: 20px y left: 50px, el cuadro se desplaza desde su posicion original.
*Por que:* relative mueve visualmente la caja pero conserva intacto el espacio que ocupaba originalmente en el flujo de la pagina.

# 3. Pruebas con absolute
*Observacion sin relative en el contenedor:* .c3 se desplaza a la esquina superior derecha de la pantalla.
*Observacion con relative en .contenedor:* .c3 pasa a colocarse en la esquina superior derecha de la caja .contenedor.
*Comportamiento del hueco:* A diferencia de relative, los demas cuadros no guardan el hueco de .c3, actuan como si .c3 hubiera desaparecido del flujo normal del documento.

# 4. Pruebas con z-index
*Observacion:* Al subir .c2, pasa a tapar a .c1. Para conseguir que .c1 quede por encima de .c2, hemos aplicado z-index: 2 a .c1.
*Nota:* z-index solo funciona si los elementos tienen una posicion definida diferente a static (en este caso hemos puesto los dos en position: relative).