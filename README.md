# Study App

Study App es una aplicacion web para estudiantes que quieren crear grupos de estudio, encontrar compañeros, gestionar conexiones y visualizar una red de estudiantes.

## Objetivo del proyecto

Convertir la app en un proyecto presentable de portafolio mientras se aprenden fundamentos reales de desarrollo web:

- Estructura de archivos.
- HTML, CSS y JavaScript modular.
- Firebase Authentication y Firestore.
- Git y flujo de commits.
- Debugging.
- Diseno de funcionalidades.
- Buenas practicas de mantenimiento.

## Estado actual

La app actualmente esta construida con archivos HTML que contienen estructura, estilos y logica JavaScript en el mismo lugar. Usa Firebase desde el frontend y contiene estas pantallas principales:

- `login.html`: registro, inicio de sesion y recuperacion de contrasena.
- `menu.html`: feed principal, grupos, busqueda de estudiantes, conexiones y notificaciones.
- `grupos.html`: grupos a los que pertenece el usuario.
- `grafo.html`: visualizacion de conexiones entre estudiantes.

## Prioridad tecnica

Antes de agregar nuevas funcionalidades, el primer objetivo es ordenar el proyecto:

1. Separar CSS y JavaScript de los HTML.
2. Centralizar la configuracion de Firebase.
3. Documentar el modelo de datos de Firestore.
4. Mejorar manejo de errores y seguridad.

