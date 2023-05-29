---
description: Prólogo
---

# Como convertirse en un desarrollador Go

Este proyecto tiene la intención de convertirse en un libro de referencia sobre el lenguaje Go para la comunidad hispanohablante.

El mayor motivo por el que elegí Go como mi herramienta de trabajo fue mi pasado con otros lenguajes, por supuesto que no hay lenguaje perfecto para todas las necesidades, pero en mi caso Go soluciona varios problemas que para mi fueron importantes o al menos creo que lo son. Solo para nombrar algunos:

* En mis comienzos comencé a trabajar desarrollando aplicaciones Android en su momento usábamos Java 1.6, realmente tener un buen entorno de desarrollo suele ser bastante pesado y no es fácil para todos tener un equipo que lo pueda correr. Pero no fue eso lo que menos gusto sino fue la sintaxis, tenes que escribir demasiado y aprender una enorme cantidad de palabras reservadas. Eso para mi hace que sea menos legible, cuando uno debe comenzar a ver un proyecto nuevo eso es muy importante. En cuanto a esto Go es más sencillo, muchas menos palabras por reservadas, y además el formateador de texto built-in es el estándar en la industria, lo que hace que el código de todos se vea similar. Esto ayuda mucho a su lectura y compresión.
* En cuanto a Python (un lenguaje que me encanta y cuando leí el Zen de Python no pude estar más de acuerdo) me marco mucho la transición de la versión 2 a la 3, un verdadero dolor de cabeza, muchas librerías que usábamos dejaban de tener soporte la para la versión 2 mientras que otras todavía no tenían soporte para la 3. Esto es muy importante, que un lenguaje con el cual tenemos productos creados en producción necesitan mantener compatibilidad para las cosas nuevas así uno puede actualizar un proyecto sin que todo explote por los aires. En ese sentido Go mantiene una promesa de compatibilidad que cumple muy estrictamente (ver esto [https://www.youtube.com/watch?v=moS35OlJBmY\&t=7s](https://www.youtube.com/watch?v=moS35OlJBmY\&t=7s)) básicamente que "Go sea aburrido" es excelente para nuestros entornos de producción.
* Con ambos un tema importante era el deploy de las aplicaciones, lo que es complicado en ocasiones ya que en a veces el entorno de desarrollo termina siendo distinto a producción. Y por ejemplo desarrollamos con una JVM  o interprete de Python de una versión distintas o tenemos una versión de la librería que estamos usando diferente. Lo que nos puede desconcertar a veces, ya que no son tan obvios esos problemas y traernos grandes dolores de cabeza.  En cambio con Go al generar un único binario termina siendo todo mucho más sencillo, te olvidas de las dependencias, corres el binario y listo hasta agregarlo a un contenedor como Docker o Podman resulta más fácil.
* Que sea pensado para que trabajes con composición y no herencia, para mi es otro punto a favor, te libras de esos problemas de no saber de que clase que heredamos viene esa función, en resumen hace el código más sencillo.
* Otra cosa que me resulto interesante sobre Go es la forma en la que  hace que sea más sencillo pensar en "Concurrencia y Paralelismo", cuando desarrollamos algo esto nos acerca más a como funcionan las cosas en la vida real al abstraer un problema para crear una solución. Sin tener que acudir a lenguajes funcionales como Haskell o Erlang (los cuales son muy buenos, pero resulta mucho más difícil conseguir desarrolladores y ni hablar de que alguien que nunca toco ese tipo de lenguaje se acostumbre a ellos.) &#x20;

Esos son algunos de los motivos, otra cosa más que me atrajo mucho al principio, fueron los primeros desarrolladores del lenguaje, personas de las que se puede aprender mucho y de las cuales recomiendo mucho ver sus conferencias y blogs. (ejemplo Rob Pike, Dave Cheney, Roger Peppe, Robert Griesemer, etc).

Proverbios más importantes del lenguaje: [https://go-proverbs.github.io/](https://go-proverbs.github.io/)

Espero que este libro les sea de utilidad. Basta de palabras, vamos a comenzar a aprender, en primer lugar vamos a ver que necesitamos para armar nuestro entorno de desarrollo.

Cuando este en un proceso más avanzado, se va a empezar a compartir con la plataforma GitBook.
