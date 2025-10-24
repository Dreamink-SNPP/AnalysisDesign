# Análisis

## Requerimientos Detallados

### ¿Cuáles son las operaciones CRUD completas?

Las operaciones CRUD completas son aquellas básicas de CREATE, READ, UPDATE y DELETE. Sirve para casi cualquier módulo, como la gestión de personajes, la gestión de escenas, la gestión de secuencias, la gestión de actos, la gestión de locaciones y también la gestión de ideas. También para la gestión de proyectos, básicamente.

### ¿Qué validaciones deben realizarse?

Las validaciones que deben realizarse son básicas para la mayoría. Por ejemplo, cuando creas a un personaje la parte obligatoria es su nombre y listo. O también la parte de locaciones, que es obligatoria y debe tener un nombre, siendo opcional la descripción y en qué escena estará partícipe.

### ¿Hay restricciones de negocio?

Las restricciones de negocio pueden ser las siguientes:

- No se pueden crear proyectos con el mismo nombre.
- Cada usuario tiene sus propios proyectos.
- Cada proyecto tiene sus propios personajes.
- Cada proyecto tiene su propia estructura (actos, secuencias, escenas).
- Cada proyecto tiene sus propias locaciones.
- Cada proyecto tiene sus propias ideas.
- Los usuarios no pueden ver los proyectos de otros usuarios.
- Los usuarios no pueden editar los proyectos de otros usuarios.
- Los usuarios no pueden eliminar proyectos de otros usuarios.

### Flujos de Negocio Críticos

#### ¿Cómo es el flujo típico de un usuario creando un proyecto completo?

El flujo típico de un usuario creando un proyecto completo es el siguiente:

1. El usuario inicia sesión en el sistema.
2. El usuario selecciona la opción "Crear proyecto" en el menú principal.
3. El usuario ingresa el título del proyecto y los diferentes datos como:
    - Género
    - Tono
    - Idea
    - Logline
    - Storyline
    - Motor de la Historia
    - Sinopsis Corta
    - Sinopsis Larga
    - Mundo o Universo Narrativo
    - Temas
    - Resumen de personajes
4. El usuario puede agregar personajes, actos, secuencias, escenas y locaciones al proyecto.
5. También puede agregar ideas sueltas para sus propósitos.
6. El proyecto se guarda automáticamente cada vez que se realiza una acción.

#### ¿Hay dependencias entre módulos? (ej: ¿podés crear escenas sin tener actos?)

**Existen dependencias entre módulos:**

- Por ejemplo, no se puede crear una estructura si no hay un proyecto creado.
- No puedes crear una secuencia si no hay un acto creado.
- No se puede crear una escena si no hay una secuencia creada.
- No puedes crear una locación si no hay un proyecto creado.

#### ¿Qué pasa si un usuario intenta eliminar un personaje usado en escenas?

Si un usuario intenta eliminar un personaje usado en escenas, no ocurre nada. El personaje aún sigue estando disponible en su respectivo lugar. Incluso si una escena se borra siendo que una locación está asociada a ella, igualmente dicha locación no se elimina.

### Roles de Usuario

#### ¿Hay diferentes tipos de usuarios? (Admin, Escritor, Colaborador, etc.)

No hay diferentes tipos de usuarios. Solamente un usuario accede con sus credenciales al sistema.

#### ¿Todos los usuarios pueden hacer todo?

Sí, todos los usuarios tienen libertad de crear proyectos, actos, secuencias, escenas, locaciones y personajes. Lo que no pueden hacer, es ver, editar, borrar proyectos de otros usuarios.

#### ¿Hay permisos diferenciados?

No hay permisos diferenciados. Todos los usuarios tienen el mismo nivel de acceso.

### Reglas de Negocio Específicas

Del modelo de dominio veo que:
- Character tiene una relación "U" (¿unique?) en name
- Scenes tienen position y color
- ¿Qué reglas aplican para positions?
- ¿Cómo se manejan las relaciones N:M (como SceneLocation)?

Respondiendo a estas preguntas e incognitas, voy a responder poco a poco. El Character o personaje como nombre (name) es único. Las escenas tienen color y position se usa para el tablero tipo Kanban dentro de la funcionalidad del sistema. Las reglas que aplican para positions es que tienen que ser únicos por así decirlo, que dos escenas no ocupen un mismo lugar en el tablero. Las relaciones que manejan N:M es simple, honestamente. No hay mucho que decir.

### Casos de Uso Faltantes
Revisando el modelo de dominio, veo que **faltan** estos casos de uso:

- Gestión de Sesiones (hay entidad Session pero no casos de uso explícitos)
- Gestión de Actos (Act) - solo aparece como "Asignar a Acto" pero no hay CRUD
- Gestión de Secuencias (Sequence) - similar al punto anterior
- Búsqueda global de proyectos
- Versionado/historial de cambios (si aplica)
- Colaboración entre usuarios (si aplica)

Respondiendo a estas cuestiones, en cuando a la gestión de sesión es simplemente el *default authentication* que viene con **Rails 8**. La gestión de actos y secuencias ya tienen un CRUD completo en el sistema, falta agregar eso en los casos de uso. No hay versionado o historial de cambios ni tampoco colaboración entre usuarios. Eso escapa de la posibilidad del proyecto.
