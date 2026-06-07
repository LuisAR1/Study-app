# Estructura del Proyecto

## Problema actual

El proyecto contiene una carpeta principal `Study-app` y una copia parcial dentro de `Study-app/Study app`. Antes de borrar o mover archivos, hay que confirmar cual version contiene los cambios mas recientes.

Tambien hay HTML, CSS y JavaScript mezclados en los mismos archivos, lo que hace dificil:

- Leer una funcionalidad completa.
- Reutilizar estilos.
- Corregir errores sin afectar otras partes.
- Aprender buenas practicas de organizacion.

## Estructura objetivo

La estructura recomendada para esta etapa es:

```text
Study-app/
  assets/
    images/
  css/
    base.css
    layout.css
    components.css
    login.css
    menu.css
    grupos.css
    grafo.css
  js/
    firebase.js
    auth.js
    students.js
    groups.js
    connections.js
    notifications.js
    ui.js
    pages/
      login-page.js
      menu-page.js
      grupos-page.js
      grafo-page.js
  login.html
  menu.html
  grupos.html
  grafo.html
```

## Orden de refactor recomendado

1. Confirmar carpeta activa y duplicados.
2. Confirmar Git y hacer un commit del estado original.
3. Mover imagenes a `assets/images`.
4. Extraer estilos comunes a `css/base.css`, `css/layout.css` y `css/components.css`.
5. Extraer estilos especificos por pagina.
6. Crear `js/firebase.js` y reemplazar configuraciones duplicadas.
7. Extraer logica por funcionalidad.
8. Documentar reglas y modelo de datos de Firestore.

## Regla de aprendizaje

Cada refactor debe hacerse en pasos pequenos. Despues de cada paso:

- La app debe seguir abriendo.
- Se debe revisar que las rutas sigan funcionando.
- Se debe hacer un commit con un mensaje claro.

