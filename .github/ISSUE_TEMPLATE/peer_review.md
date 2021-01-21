---
name: Peer Review
about: 'Evaluación de proyecto por pares'
title: "Revisión por pares"
labels: "evaluation peer review"
assignees: '100%'

---

<!--Responde las preguntas presentadas para realizar la revisión por pares (peer review) y completa el título del issue con las iniciales de tu nombre.-->

## Identificación  
* ¿A qué grupo pertenece?  
  Soy representante del grupo #16  
## Evaluación
* (Opcional) Coloque un comentario relevante de la impresión que tuvo en usted el proyecto de este grupo  
  Me gusta el recorrido teórico del principio, tal como en la documentación del curso. Comentaron los pasos y usaron cada definición de objetos y funciones.
  Las funciones y variables cumplen con su objetivo y son reutilizables para extenderlo a todos los incisos. El código es claro, entendible y limpio.  
  Dicho eso, hay unos detalles __muy pequeños__ que se pueden mejorar, algunos son cuestión de estilo, otros no alteran la funcionalidad en este proyeto, pero pueden afectar en proyectos más grandes.  
  1. **Usar más de un `return` en una estructura de control.** Por ejemplo, la función `iterate()` retorna un valor booleano si la condición se cumple. Ustedes usaron 2 returns para cada valor. Eso no altera en nada la funcionalidad y al ser muy corto no se nota, pero en bloques de código mucho más grandes, seguir la salida de cada return puede complicarse y llevar a errores. ¿La solución? pueden usar una variable que guarde el resultado que luego retornarán al final. De esa manera se ahorrarán código y será más legible. Hay quienes piensan que no es necesario hacerlo, pero solo es una sugerencia **;)**.  
  2. **El críterio de convergencia usado no es el mismo que el propuesto.** En la función `testJM()` la comprobación del criterio dice que `abs(z) <= 2` pero en el marco teórico dice que `|z| < 2` por lo que el **=** no debería estar ahí. Es un detalles minúsculo y fácil de corregir.  
  3. **Las iteraciones pueden optimizarse (en teoría).** Esto recién lo supe y puede que no sea la gran cosa, pero tiene sentido. Cuando se itera de la forma ascendente: `for i in 1:a` Julia debe comprobar en cada iteración si **i** no sobrepasa el **valor máximo**, es decir, el valor de la variable `a`, pero si la iteración se realiza al revés: `for i in a:-1:1` la comprobación se realiza una sola vez, para luego decrecer hasta 1. En este proyecto no habrá diferencia, pero en iteraciones mucho más largas, ese cambio puede optimizar el rendimiento ya que no se hacen llamados a la variable en cada iteración.  
  
Son sugerencia que pueden o no tomar en cuenta. En general es un **excelente proyecto y felicito a todos los involucrados.** Sigan adelante.  
* Responda los siguiente con sí o no:
  - ¿Cumple con todos los requisitos mencionados en el enunciado del proyecto?  
    Sí
  - ¿Cada bloque de código tiene suficiente claridad para entender usted lo que realiza?  
    Sí
  - ¿El proyecto presenta todo lo solicitado?  
    Sí
