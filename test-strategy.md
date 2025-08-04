# Estrategia de Testeo y Corrección

## Problemas Encontrados y Soluciones Aplicadas

1. **Error en el uso de `addEventListener`**
   - **Problema:** Se utilizó `"addeventListener"` (con error de sintaxis).
   - **Solución:** Se corrigió a `"addEventListener"` para asegurar la funcionalidad de los botones.

2. **Generación incorrecta del número aleatorio**
   - **Problema:** Se generaban números decimales fuera del rango esperado.
   - **Solución:** Se ajustó la lógica para generar un número entero entre 1 y 100:  
     `Math.floor(Math.random() * 100) + 1`.

3. **Validación débil del input del usuario**
   - **Problema:** Se permitían letras, números negativos, decimales y valores fuera de rango.
   - **Solución:** Se implementó validación para aceptar únicamente enteros positivos entre 1 y 100.

4. **Manejo de errores poco amigable**
   - **Problema:** Se utilizaban alertas (`alert`) para mostrar errores.
   - **Solución:** Los errores ahora se muestran directamente en la interfaz con estilo (fondo naranja).

5. **Comparación de tipos incorrecta**
   - **Problema:** Se comparaba texto (`string`) con número (`number`).
   - **Solución:** El valor ingresado por el usuario se convierte explícitamente a número antes de la comparación.

6. **Mensajes y colores incorrectos**
   - **Problema:** Los mensajes y colores no coincidían con los requerimientos del juego.
   - **Solución:** Se ajustaron los textos y estilos para reflejar correctamente los estados de victoria, error o derrota.

7. **Selector de elemento mal escrito**
   - **Problema:** Se usaba `document.querySelector('lowOrHi')` (sin el punto).
   - **Solución:** Se cambió a `document.querySelector('.lowOrHi')` para seleccionar correctamente el elemento con clase CSS.

8. **Número de intentos incorrecto**
   - **Problema:** El juego finalizaba a los 5 intentos.
   - **Solución:** Se modificó la lógica para permitir 10 intentos, como indica el proyecto.

9. **Lógica de victoria/derrota invertida**
   - **Problema:** Los mensajes de éxito y fracaso no se mostraban correctamente.
   - **Solución:** Se corrigió la condición para mostrar el mensaje correcto según el resultado del jugador.

Todas las modificaciones fueron probadas para verificar que el juego responde correctamente en cada escenario. Se validó también que la interfaz y comportamiento general coincidan con lo solicitado en el proyecto original.
