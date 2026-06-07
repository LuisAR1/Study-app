# Contexto del Proyecto

Este archivo define el lenguaje del proyecto para que las decisiones tecnicas usen los mismos nombres.

## Producto

**Study App** es una red social academica para estudiantes.

## Conceptos del dominio

**Estudiante**

Usuario registrado de la aplicacion. Tiene perfil academico, materias de interes, horarios disponibles y conexiones con otros estudiantes.

Campos actuales observados:

- `uid`
- `username`
- `nombre`
- `email`
- `universidad`
- `carrera`
- `materias`
- `horarios`
- `conexiones`
- `grupos`
- `createdAt`

**Grupo de estudio**

Publicacion creada por un estudiante para reunir personas alrededor de una materia, modalidad o meta de estudio.

Campos actuales observados:

- `titulo`
- `descripcion`
- `materia`
- `modalidad`
- `cupos`
- `autorUid`
- `autorUsername`
- `autorNombre`
- `autorUniversidad`
- `miembros`
- `likes`
- `createdAt`

**Conexion**

Relacion aceptada entre dos estudiantes. Actualmente se guarda como una lista de `uid` dentro del documento de cada estudiante.

**Solicitud de conexion**

Peticion enviada por un estudiante a otro para conectarse.

Campos actuales observados:

- `de`
- `deUsername`
- `deNombre`
- `para`
- `estado`
- `createdAt`

**Username**

Nombre publico unico usado para iniciar sesion. Actualmente se guarda un documento en la coleccion `usernames` que relaciona `username` con `email` y `uid`.

## Colecciones Firestore observadas

- `estudiantes`
- `usernames`
- `grupos`
- `solicitudes`

## Decisiones iniciales

- La app seguira siendo HTML, CSS y JavaScript vanilla mientras se aprenden fundamentos.
- Firebase seguira siendo el backend inicial.
- Se priorizara claridad y aprendizaje antes de migrar a frameworks.
- Las funcionalidades nuevas se agregaran despues de ordenar estructura, datos y flujo de trabajo.

