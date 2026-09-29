# git-work — flujo colaborativo con Git

Repositorio de práctica del flujo colaborativo (fork, issue, rama, PR,
conflicto, etiqueta y release) del módulo DPL.

## Índice

- [Entorno e instalacion](#entorno-e-instalacion)
- [Configuracion](#configuracion)
- [Comprobación](#comprobacion)
- [Problemas encontrados y solucion](#problemas-encontrados-y-solucion)
- [Repositorio remoto](#repositorio-remoto)

## Entorno e instalacion
Clonar el repositorio y abrir index.html en el navegador.

## Configuracion
En css/cover.css, la línea 10 define el color del botón y la 11 su sombra.

## Comprobacion
Las salidas reales de los comandos de verificación (`git log`, `git remote -v`, `git tag`, etc.) han sido guardadas y se pueden consultar en el archivo [comprobaciones.txt](comprobaciones.txt) de este repositorio.

## Problemas encontrados y solucion
| Problema | Causa | Solución |
| :--- | :--- | :--- |
| Conflicto de fusión en `css/cover.css` | Se modificó la línea 10 (`color`) de forma simultánea en la rama `main` local (color morado) y en la rama `cool-colors` del PR #2 (color verde oscuro). | Se editó el archivo manualmente en local para conservar la propuesta `darkgreen` del colaborador (`user2`). Se borraron las marcas de conflicto de Git (`<<<<<<<`, `=======`, `>>>>>>>`), se preparó el archivo con `git add` y se completó la fusión con `git commit`. |

## Repositorio remoto
https://github.com/zabdive21/git-work
