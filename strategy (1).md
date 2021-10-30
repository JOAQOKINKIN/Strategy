# Patrón de Diseño: Strategy  

## ¿Qué es Strategy?  

*Strategy es un patrón de diseño de tipo comportamiento que permite crear grupos de algoritmos, colocarlos en clases separadas y hacer sus objetos intercambiables.*  
***

## ¿Para qué sirve?  

-Utiliza el patrón Strategy cuando quieras utilizar variantes de un algoritmo dentro de un objeto y poder cambiar de un algoritmo a otro durante el tiempo de ejecución.

-Utiliza el patrón cuando tengas muchas clases similares que solo se diferencien en la forma en que se ejecutan cietyos comportamientos.

-Utiliza el patron cuando tu clase tenga un enorme operador condicional que cambie entre distintas variables del mismo algoritmo.

-Utiliza el patrón para aislar la lógica de negocio de una clase, de los detalles de implementación de algoritmos que pueden no ser tan importantes en el contexto de esa lógica.
***

## Estructura

!<https://refactoring.guru/images/patterns/diagrams/strategy/structure.png?id=c6aa910c94960f35d100>
***
## ¿Como Usarlo?

1. En la clase contexto, identifica un algoritmo que tienda a sufrir cambios frecuentes. También puede ser un enorme condicional que seleccione y ejecute una variante del mismo algoritmo durante el tiempo de ejecución.

2. Declara la interfaz estrategia común a todas las variantes del algoritmo.

3. Uno a uno, extrae todos los algoritmos y ponlos en sus propias clases. Todas deben implementar la misma interfaz estrategia.

4. En la clase contexto, añade un campo para almacenar una referencia a un objeto de estrategia.

5. Los clientes de la clase contexto deben asociarla con una estrategia adecuada que coincida con la forma en la que esperan que la clase contexto realice su trabajo principal.
***

## Pros 

-Puedes intercambiar algoritmos usados dentro de un objeto durante el tiempo de ejecución.

-Puedes aislar los detalles de implementación de un algoritmo del código que lo utiliza.

-Puedes sustituir la herencia por composición.

-Principio de abierto/cerrado. Puedes introducir nuevas estrategias sin tener que cambiar el contexto.
***

## Contras

-Los clientes deben conocer las diferencias entre estrategias para poder seleccionar la adecuada.

-Muchos lenguajes de programación modernos tienen un soporte de tipo funcional que te permite implementar distintas versiones de un algoritmo dentro de un grupo de funciones anónimas.
***

## Integrantes

### Poblete, Faustino.

### Petitfour, Facundo.

### Frasca, Joaquin.
***