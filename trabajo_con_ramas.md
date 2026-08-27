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

## Ejemplo de el trabajo con ramas

Un ejemplo de trabajo en ramas en Git sería el desarrollo de una página web por parte de un equipo de programadores. Primero, todos parten de una rama principal llamada main, que contiene el código estable del proyecto. Luego, un programador crea una rama llamada feature-login para desarrollar el sistema de inicio de sesión, mientras otro crea una rama llamada feature-pagos para trabajar en el sistema de pagos. Cada uno realiza sus cambios y los guarda mediante commits sin afectar la rama principal. Cuando terminan sus tareas, revisan y prueban el código y, si todo funciona correctamente, fusionan sus ramas con main mediante un proceso llamado merge. De esta manera, los integrantes del equipo pueden trabajar al mismo tiempo en diferentes funciones del proyecto de forma organizada y segura.

## Conclusion de trabajo en ramas 

El trabajo en ramas permite organizar mejor un proyecto, trabajar en equipo y realizar cambios sin afectar el código principal. Es una herramienta fundamental de Git para desarrollar de manera segura, ordenada y eficiente.

## Concepto clave adicional: Pull Requests / Merge Requests
En entornos colaborativos (como GitHub, GitLab o Bitbucket), el paso 5 de tu flujo (Fusionar la rama) no se suele hacer directamente desde la terminal del desarrollador. En su lugar, se abre una Pull Request (PR). Esto permite que los compañeros de equipo revisen el código, hagan comentarios, sugieran cambios y ejecuten pruebas automáticas antes de autorizar la fusión con la rama principal.

## Un conflicto de fusión (merge conflict)
 ocurre cuando Git no puede integrar automáticamente los cambios de dos ramas porque ambas han modificado la misma línea en el mismo archivo de maneras distintas, o porque una rama eliminó un archivo que la otra intentó modificar.

- A diferencia de las fusiones automáticas donde Git une el código sin problemas, ante un conflicto el sistema detiene el proceso y te pide a ti, como desarrollador, que decidas manualmente qué cambios conservar y cuáles descartar.

## ¿Por qué ocurre un conflicto?
Git es muy eficiente uniendo cambios que ocurren en diferentes archivos o en distintas líneas de un mismo archivo. Sin embargo, se produce un conflicto cuando:

-Modificación concurrente de la misma línea: Dos desarrolladores editan exactamente las mismas líneas en un archivo partiendo de la misma base, pero con código diferente.

- Edición vs. Eliminación: Un desarrollador modifica una sección de código en su rama mientras que otro elimina esa misma sección o el archivo completo en otra rama.