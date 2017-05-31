# Hablando de Testing…

Como buenos devtesters que somos, en nuestro día a día surgen infinidad de conversaciones, referencias o lecturas acerca de los test. Oímos hablar continuamente de test funcionales, test unitarios, test de aceptación, test de componentes, test de regresión… pero ¿nos estamos expresando bien?

---
*¿Un test de aceptación es distinto de un test funcional?¿Y un test funcional de un test unitario? ¿Es correcto decir test unitarios de aceptación? ¿Los test unitarios son todos los que ejecutan directamente el código? ¿Los test de aceptación son los de GUI? ¿Todos los test son funcionales? ¿Un test de componente es unitario?*

---

Intentando aclarar posibles dudas como las anteriores, debemos tener claro que todos los test son calificados por dos propiedades, el **NIVEL** y el **TIPO**. El nivel de test está relacionado con el alcance del objeto de prueba. El tipo de test está relacionado con la validación objetivo. Simplificando, podríamos decir que todo test debe tener un alcance y un objetivo.

Niveles de test (de menor a mayor alcance):
1. **Unitarias o de componente**: Se prueba de forma individual y aislada según las especificaciones de más bajo nivel (función, clase, interfaces, procedimientos).
2. **Integración**: Comprueba la interacción entre dos o más componentes desacoplados del sistema global.
3. **Sistema**: Prueba el diseño y comportamiento de todos los componentes del sistema integrados.
4. **Aceptación**: Comprueba que el sistema cumple todos los requisitos del cliente.

Tipos de test:
- **Funcionales**: Evaluar que se cumplen las capacidades requeridas.
- **No funcionales**: Evaluar la fiabilidad, usabilidad, eficiencia, mantenibilidad y portabilidad.
- **Estructurales**: Evaluar corrección estructural implementada (Se basan en la cobertura)
- **De cambios**: Evaluar el impacto del cambio.

**NOTA**: Dentro de los tipos de test, existen subtipos como pueden ser los de robustez, estrés, seguridad, regresión, retesting, etc. pero que no son el objetivo de este post ;)

Aunque la terminología respecto a los test esté evolucionando diariamente o haya distintas metodologías con sus propios términos, todos podemos partir de unas bases comunes. Existen infinidad de post y publicaciones, pero hemos querido reseñar las contempladas en los estándares ISO (http://www.softwaretestingstandard.org/) e ISTQB (http://istqbexamcertification.com/) de testing y calidad software.
