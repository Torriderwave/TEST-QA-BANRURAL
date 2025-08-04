# Estrategia de Testeo y Corrección

A continuación se detallan los problemas encontrados en el archivo index.html y las soluciones aplicadas para cumplir con los requisitos del proyecto:

1. **Uso incorrecto de addEventListener**
   - *Problema:* Se usó "addeventListener" en vez de "addEventListener", lo que impedía que los botones funcionaran.
   - *Solución:* Se corrigió el nombre del método a "addEventListener".

2. **Generación de número aleatorio incorrecta**
   - *Problema:* El número aleatorio se generaba como decimal y en un rango incorrecto (0-10 o 0-100).
   - *Solución:* Se ajustó la generación para obtener un entero entre 1 y 100 usando `Math.floor(Math.random() * 100) + 1`.

3. **Validación de input insuficiente**
   - *Problema:* Permitía letras, decimales, negativos y números mayores a 100.
   - *Solución:* Se agregó validación para aceptar solo números enteros positivos entre 1 y 100.

4. **Mensaje de error poco amigable**
   - *Problema:* Se usaba `alert` del navegador para mostrar errores de input.
   - *Solución:* Ahora el mensaje de error se muestra en la interfaz, usando el área de resultados y CSS (fondo naranja).

5. **Comparación de tipos incorrecta**
   - *Problema:* Se comparaba string con número, lo que podía causar fallos.
   - *Solución:* Se convierte el input a número antes de comparar.

6. **Mensajes y colores no seguían los requisitos**
   - *Problema:* Los mensajes y colores de éxito/error no coincidían con lo solicitado en el README.
   - *Solución:* Se ajustaron los textos y colores para cada caso según los requisitos.

7. **Selector de lowOrHi incorrecto**
   - *Problema:* Se usaba `document.querySelector('lowOrHi')` en vez de `document.querySelector('.lowOrHi')`.
   - *Solución:* Se corrigió el selector para que apunte al elemento correcto.

8. **Número de intentos incorrecto**
   - *Problema:* El juego permitía solo 5 intentos en vez de los 10 requeridos.
   - *Solución:* Se ajustó la variable a 10 intentos.

9. **Lógica de victoria/derrota invertida**
   - *Problema:* Los mensajes de victoria y derrota estaban invertidos y no se mostraban correctamente.
   - *Solución:* Se corrigió la lógica para mostrar el mensaje adecuado según el resultado del juego.

---

Cada uno de estos puntos fue verificado y corregido para asegurar el funcionamiento correcto del juego y el cumplimiento de los requisitos del cliente.