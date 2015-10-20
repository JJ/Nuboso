# Licencia

Esta obra está sujeta a la licencia Reconocimiento-CompartirIgual 4.0 Internacional de Creative Commons. Para ver una copia de esta licencia, visite http://creativecommons.org/licenses/by-sa/4.0/.

![cc-by-sa](img/by-sa.png)

# Prólogo y agradecimientos

Este libro se escribió originalmente para el
[curso de computación nube](http://curso-nube.github.io/) impartido en el Centro de profesores de Jaén en diciembre de 2014. Posteriormente se ha ido enriqueciendo con el material que se ha ido usando en los cursos de [Infraestructura Virtual](https://jj.github.io/IV) y [Cloud Computing](https://jj.github.io/IV)) de grado y máster en Informática, respectivamente.

Es un libro que está continuamente renovándose, por lo que seguramente habrá algún
(ciento de) fallo. Pero dado que es un libro libre, puedes corregir
esos fallos y hacerte tu propia versión en GitHub o
[hacernos sugerencias y comentarios](https://github.com/JJ/nuboso/issues)
que atenderemos rápida y debidamente. Si te atreves una vez escrito el
libro a hacer los cambios tú mismo y a solicitarnos la incorporación a
versiones posteriores del libro, te lo agradeceremos aún más y
aparecerás en este prólogo. 

Para aprovechar este libro tendrás que tener ciertos conocimientos de
programación. El principal lenguaje de programación usado es
[JavaScript, que puedes aprender en este otro libro (también mío)](https://www.amazon.es/dp/B00HXL8QA0?tag=atalaya-21&camp=3634&creative=24822&linkCode=as4&creativeASIN=B00HXL8QA0&adid=15Q8XP8D82TTXHRS5Y5F&)
o, por supuesto, en cualquier otro tutorial que encuentres. Es
imprescindible también conocer
[git, que puedes aprender en este otro libró que publiqué con Pablo Hinojosa](https://www.amazon.es/dp/B00K515GL2?tag=atalaya-21&camp=3634&creative=24822&linkCode=as4&creativeASIN=B00K515GL2&adid=1BVSCTRKGH632QR323YS&). Con
los primeros capítulos será suficiente, se trata de saber usar
repositorios para gestionar tu código, algo esencial en el espíritu de
*DevOps* que trato de transmitir en este libro. También hará falta
cierto manejo de la línea de órdenes de Linux (que es la misma del Mac)

>Lo siento, pero hasta hace tanto, nube y Windows no se llevan bien. Si no quieres abandonar
>tu Windows, que es un sistema operativo de escritorio y consumo, no
>de desarrolladores, instálate Linux en una máquina virtual y trabaja
>con él, aunque en ese Linux, a su vez, puede que necesites instalarte
>también un hipervisor para trabajar con máquinas virtuales, con lo
>que será más fácil que lo montes en una partición.

## Agradecimientos adicionales

A Jacinto Carrillo, del centro de profesores, por habernos dado la
oportunidad de dar este curso y a José Antonio Vacas, que fue quien
nos presentó. 

## Un libro libre

Este libro es libre. Puedes haberlo recibido de un amigo, generado por
tu cuenta [a partir del repositorio](https://github.com/JJ/Nuboso) o
comprado. En cualquiera de los casos, está a la venta en Amazon a
precios populares. El autor te agradece que
lo recomiendes, hables de él, digas que te ha parecido y, por
supuesto, que lo compres. 

## Instrucciones de uso

Te beneficiarás de este libro si lo usas con el ordenador abierto y
vas copiando y pegando los ejemplos al terminal o al editor e
intentando hacer los ejercicios. Necesitarás un ordenador Linux con
Ubuntu (o un Mac con una serie de herramientas instaladas) y con una
conexión a Internet decente (básicamente, que no sea con el móvil).

Si quieres, créate un repositorio en GitHub y ve subiendo los
ejercicios. No es que vaya a corregirlos, pero puedes compartirlos con
compañeros y corregirlos entre vosotros. Si dispongo de tiempo para
echaros una mano, haré lo que pueda por ayudar también.

# Introducción a la computación en nube

La computación en nube ha supuesto una revolución en el arte de la
programación, en medios y en métodos. En medios porque ya no hay que
depender de un simple sistema, o varios, una aplicación monolítica y
estática durante toda la vida de la aplicación: los soportes *físicos*
se convierten en algo *elástico*, mutable y sobre todo definible
usando programas escritos en lenguajes específicos, adaptados al
dominio respectivo.

Esto, a su vez, ha hecho que cambie la metodología: los ciclos de
desarrollo son mucho más rápidos, pero los equipos se engloban en el
concepto de *DevOps* que mezcla los departamentos de sistemas
desarrollo y calidad en un solo grupo que trabaja conjuntamente y se
responsabiliza de todo el ciclo de vida, desde la definición del
entorno de desarrollo, prueba y despliegue hasta la puesta en
producciónd e la aplicación.

Por eso, si tu formación en programación es tradicional y piensas en
una sola máquina (o un solo sistema con varias máquinas), una sola
aplicación, quizás con varios *tiers* o partes (cliente, servidor,
*middleware*), debes cambiar la mentalidad y pensar en muchas piezas
débilmente acopladas, donde la información puede residir en múltiples
sitios a la vez en diferentes grados de elaboración y dónde los puntos
de entrada de los clientes pueden ser, a la vez múltiples. Los
recursos pueden estar en diferentes máquinas, ser de diferentes
vendedores y, en general, estar en la nube.

Precisamente para que tú no estés en las nubes y desciendas al suelo
de, ejem, la nube, está este libro. Espero que te sea de ayuda.
