# Respuestas Ejercicio 5 - Parte A: Detective de Colisiones

# 1. h1
*Color:* brown
*Color Real:* brown
*Explicacion:* Gana la regla titulo porque los selectores de ID tienen mas prioridad que las clases o las etiquetas.

# 2. p class="aviso"
*Color:* purple
*Color Real:* purple
*Razonamiento:* Habia tres reglas. Gana p.aviso porque junta etiqueta y clase en el mismo selector, porque es mas especifica que las reglas sueltas.

# p id="importante"
*Color:* black
*Color Real:* black
*Razonamiento:* Gana #importante porque un selector de ID aplasta a cualquier otra regla de clase o etiqueta.

# <div><p>
*Color:* orange
*Color Real:* orange
*Razonamiento:* Gana div p porque le dice al navegador exactamente donde esta el parrafo.