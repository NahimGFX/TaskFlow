# taskflow

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Alcance de TaskFlow

Problema: necesito organizar plan de estudio y saber cuáles faltan.
Usuario objetivo: estudiante que planifica entregas semanales.

### Historias de usuario y criterios de aceptación

1. Como estudiante de programación, quiero listar mis actividades de estudio para organizar los temas que debo aprender.
   Criterio: la lista muestra el título, la prioridad y el estado de cada actividad de aprendizaje.

2. Como estudiante de programación, quiero consultar el detalle de una actividad para conocer los temas que debo estudiar.
   Criterio: al tocar una tarjeta aparece la descripción completa de la actividad seleccionada.

3. Como estudiante de programación, quiero crear nuevas actividades de estudio para registrar temas que deseo aprender.
   Criterio: el formulario permite registrar una actividad con título, descripción y prioridad, y la lista muestra la nueva tarea.

4. Como estudiante de programación, quiero editar mis actividades de estudio para actualizar los temas o contenidos que debo aprender.
   Criterio: los cambios guardados se reflejan en la lista y en el detalle de la actividad.

5. Como estudiante de programación, quiero eliminar actividades de estudio que ya no necesito para mantener organizada mi planificación.
   Criterio: después de confirmar la eliminación, la actividad desaparece de la lista.

### Modelo de datos

Task: id (entero único), title (texto), description (texto),
priority (Alta, Media o Baja), isCompleted (verdadero/falso),
userId (entero que identifica al usuario de prueba).

### Pantallas previstas

Lista: tarjetas de tareas y acción para crear.
Detalle: información completa y futuras acciones de editar o eliminar.
Formulario: campos de título, descripción y prioridad.

### Requisitos no funcionales

La navegación debe tener textos comprensibles.
Un id inexistente debe mostrar un mensaje en vez de cerrar la app.

### Contrato de API que necesitaremos

GET /tasks listar tareas
GET /tasks/:id consultar detalle
POST /tasks crear tarea
PATCH /tasks/:id actualizar tarea
DELETE /tasks/:id eliminar tarea

La API concreta se elegirá después. Estas rutas son requisitos, no
direcciones de un servidor ya conectado.
