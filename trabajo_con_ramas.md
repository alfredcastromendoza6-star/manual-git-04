# Investigación: Trabajo en Ramas en Git

## ¿Qué es el trabajo en ramas?

El trabajo en ramas (branching) es una forma de organizar el desarrollo de un proyecto utilizando Git, un sistema de control de versiones.
Una rama permite crear una línea independiente de desarrollo a partir de otra. De esta manera, los desarrolladores pueden realizar cambios sin modificar directamente el código principal del proyecto.

Por ejemplo, un proyecto puede tener una rama llamada main, que contiene la versión estable, y otra llamada login, donde se desarrolla una nueva función de inicio de sesión.

## ¿Cómo funciona?

Un flujo de trabajo básico con ramas es:

1. Crear una rama para una nueva función o corrección.
2. Realizar cambios en esa rama.
3. Guardar los cambios mediante commits.
4. Revisar y probar el código.
5. Fusionar (merge) la rama con la rama principal.
6. Eliminar la rama cuando ya no sea necesaria.

Esto permite que varias personas trabajen al mismo tiempo en diferentes partes de un proyecto.

## Ventajas de trabajar con ramas

* Trabajo independiente: cada desarrollador puede trabajar en una función diferente.
* Seguridad: los cambios no afectan inmediatamente al código principal.
* Trabajo colaborativo: varias personas pueden desarrollar simultáneamente.
* Revisión del código: los cambios pueden revisarse antes de incorporarlos al proyecto.
* Organización: cada rama puede representar una función, corrección o experimento.