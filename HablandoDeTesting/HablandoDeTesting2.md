# Hablando de Testing (2)…

Siguiendo la línea del post anterior de **'Hablando de testing...'**, ya aclaradas las diferencias entre niveles de test y tipos de test, intentemos aclarar otra duda habitual… cuando se habla de test caja-negra , test caja blanca, test de usuario, test exploratorios... ¿a que se refieren todas estas denominaciones?

Todos los ejemplos dados (y muchos más que existen) se refieren a **'Técnicas de testing'**. Este concepto hace referencia a qué estrategia utilizas a la hora de afrontar las pruebas de algo y los procedimientos para definir los casos de prueba.

Al igual que cuando programamos funcionalidad podemos resolver el mismo problema con distintas aproximaciones (funcional, orientado a objetos, iterativo, recursivo, etc.) en testing podemos afrontar las pruebas con distintas aproximaciones también.

Para aclarar este concepto de **Técnicas de testing** vamos utilizar las dos más conocidas, test de cada negra y test de caja blanca. La primera es una técnica de testing guiada por especificación, esto quiere decir que algo tiene que hacer lo que está especificado que haga, independientemente de como internamente lo haga (sin conocer sus tripas, de ahí el concepto caja negra). La segunda técnica, caja blanca es una técnica basada en la estructura de la solución, es decir, conocer cómo hace las cosas para buscar los casos de prueba (lo contrario que caja negra).

Ninguna es mejor o peor que otra, son dos aproximaciones igualmente válidas y ambas pueden servir para resolver la implementación de un mismo TIPO y NIVEL de test. Es decir, podemos resolver, por ejemplo, un test unitario funcional con una aproximación de caja negra al igual que lo podemos probar con una aproximación de caja blanca. Es el propio desarrollador el que debe decidir cual de todas las técnicas de testing es la que mejor se adapta a sus necesidades, incluso contemplar alternativas no automáticas como un test exploratorio (que un usuario sin conocimiento del sistema lo pruebe como se le ocurra, sin indicación ninguna).

Repasando rápidamente, habíamos hablado de niveles de test (unitario, integración, sistema y aceptación), tipos de test (funcionales, no funcionales, estructurales y de cambios) y ahora también diferenciamos técnicas de testing.

Nuevamente, remarcar que existen infinidad de términos  y denominaciones para referenciar estas técnicas de testing, pero la intención es aclarar el concepto más allá de los términos que se puedan emplear en cada foro.

http://istqbexamcertification.com/what-is-test-design-technique/
http://softwaretestingfundamentals.com/black-box-testing/
https://es.wikipedia.org/wiki/Exploratory_testing