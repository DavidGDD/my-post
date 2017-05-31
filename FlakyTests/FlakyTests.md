Ese dichoso rojo en los tests...

Todo el mundo que ha pasado por integración continua, ha sufrido o sufre esos dichos tests que a veces fallan y a veces van bien, piensas que nuestro desarrollo es incorrecto, luego piensas que el desarrollo es correcto y luego ya no sabes que pensar (dependiendo de cuántas veces los ejecutes).

Estos tests tienen un nombre... “Flaky Tests” (tests escamosos) y se refieren a todos aquellos tests no deterministas.

La automatización de tests y su valor, reside en en el determinismo de los resultados, es decir, que si la ejecución de un test es correcta, no necesito validar paso a paso mi código bajo test, ya que se que en las mismas condiciones, su ejecución va a ser siempre la misma. Cuando se rompe el determinismo de un test o de un código, me veo obligado a tener que hacer este trabajo tanto para resultados correctos como incorrectos, por lo que tener un test automático no me aporta ningún valor.

El principal ámbito de testing afectado por este tipo de tests son los tests de regresión, base de la integración continua, donde pretendemos validar de forma automática que cambios en el código no “rompen” la funcionalidad ya existente.

Un “flaky test” puede implicar un problema en el código probado o un problema en la implementación del propio test. Han de ser estudiados con detenimiento para determinar el origen de la indeterminación.

Principales causas para que un test sea “Flaky”:
Asincronía: El test desencadena una acción asíncrona que no es gestionada correctamente. El resultado depende de la velocidad con la que se resuelve esa acción.
Concurrencia: Cuando nuestro test desencadena cierta concurrencia en alguna pieza o componente que puede entrar en condiciones de carrera o bloqueos que producen resultados variables.
Dependencias entre tests: En ocasiones los test no están correctamente aislados, por lo que una variación en el conjunto de pruebas puede implicar un estado inconsistente ante la ejecución de los mismos.

Existen otras causas menos comunes como la falta de recursos en la infraestructura (hilos, conexiones disponibles, etc.), operaciones de I/O, conectividad entre distintas piezas, inputs con datos ordenados aleatoriamente y muchos otros menos frecuentes.

Existen diferentes estrategias para gestionar los flaky tests, pero lo más importante es saber que no siempre es culpa del test ni tampoco siempre culpa del código, hay que estudiarlo con detenimiento.

Referencias:
http://mir.cs.illinois.edu/~qluo2/fse14LuoHEM.pdf
https://testing.googleblog.com/2016/05/flaky-tests-at-google-and-how-we.html﻿