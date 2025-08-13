# Análisis y Diseño

## Análisis de Requisitos

En este apartado, se describirán los requisitos que el sistema pueda contener y sus posibles exigencias. Se intentará recabar todos los datos posibles sobre la situación y problemática actual que acontece con este proyecto.

Es posible actualizar con el tiempo agregar mayor información.

### Visión general de DREAMINK

DREAMINK es una aplicación web de código abierto pensada para acompañar al guionista **únicamente en la fase de estructuración previa al guion literario**. Su razón de ser es ofrecer un espacio claro, flexible y centralizado donde plasmar la idea embrionaria de una película y convertirla, paso a paso, en un armazón dramático coherente que luego pueda volcarse a texto en *formato Fountain*. En ningún momento pretende sustituir al software de escritura *escena-a-escena* ni cubrir el terreno del guion técnico: su fortaleza está en el terreno de la **planificación creativa**, donde todavía se trabaja con:

- conceptos,
- fichas
- y tarjetas movibles.

#### Tratamiento general: la brújula creativa

El recorrido del usuario comienza con la sección de **tratamiento**, un panel de campos de texto donde podrá definir, con libertad pero sin perder de vista los *pilares básicos*, qué historia quiere contar. Aquí introduce el:

- título de la obra,
- el género principal y complementarios,
- el *logline* que condensa la premisa,
- las sinopsis breve y extendida,
- la descripción del mundo en el que todo sucede,
- los temas que desea explorar
- y el tono narrativo que busca.

Esta primera parada funciona como *brújula creativa*: cada decisión que el guionista tome más adelante podrá contrastarla con esta declaración de intenciones iniciales.

#### Estructura dramática dinámica: actos, secuencias y escenas

Una vez fijadas las líneas maestras, DREAMINK despliega su **tablero narrativo**. El sistema **no impone un número prefijado de actos ni de secuencias**; el usuario decide *cuántos bloques necesita*: puede trabajar con tres actos clásicos, con cinco o con cualquier otra división que le resulte útil. Cada acto se crea con un **título y una descripción**, y de la misma forma cada secuencia (o sub-bloque interno) recibe **su propio título** y **su propio resumen**. Esta libertad se traduce en un lienzo adaptable donde el escritor experimenta y reorganiza su estructura hasta encontrar el ritmo que desea.

Dentro de los actos y las secuencias, el guionista puede añadir **escenas**. Las escenas son el nivel más granular de la herramienta y cuentan también con ABMC completo: se dan de alta, se dan de baja, se modifican o se consultan con la misma facilidad *que se reordena una tarjeta en un corcho*. Como ayuda visual, **cada escena admite un color libremente asignable**: rojo, azul, verde, el que el autor prefiera. El color no tiene un significado rígido; sirve como etiqueta rápida para lo que cada guionista necesite—ya sea marcar estados de avance, distinguir líneas temporales o simplemente separar momentos intensos de momentos ligeros. En el tablero, esa explosión de color permite identificar de un vistazo patrones y posibles *desequilibrios dramáticos*.

#### Fichas de personajes: pulsos internos y rostros externos

En paralelo al esqueleto argumental, DREAMINK ofrece un **módulo de personajes** que invita a profundizar en quienes mueven la historia. Cada ficha arranca con los datos generales—nombre, rol, edad aproximada—y se bifurca en dos grandes apartados: **atributos internos** (motivaciones, creencias, conflictos íntimos, arco de transformación) y **atributos externos** (apariencia, ocupación, nivel socioeconómico, posesiones, etc.). El guionista va rellenando estos campos a su ritmo, de modo que la personalidad, las contradicciones y los objetivos de cada figura queden anclados antes de lanzarla a la acción. Las fichas permanecen siempre accesibles para consulta rápida mientras se decide dónde y cómo intervenirá cada personaje en las escenas.

#### Fichas de locaciones: atmósfera y función dramática del espacio

El tercer pilar lo conforman las **locaciones**. Cada escenario dispone de un nombre identificador y de una descripción donde el autor plasma tanto la atmósfera física (aspecto, luz, sonido, época) como la **función dramática** que ese lugar cumple en la trama. Esta información ayuda a asegurar coherencia espacial y a evitar contradicciones cuando una misma locación reaparece a lo largo del relato. Como en los otros módulos, se pueden crear, modificar, consultar o eliminar fichas sin restricciones.

#### Ideas sueltas: un espacio para el brainstorming

A petición expresa del usuario, se incorpora una nueva sección autónoma denominada **“ideas sueltas”**. Funciona como un bloc de notas enriquecido: cada idea consta de un título o etiqueta rápida y de una descripción libre. Puede tratarse de una línea de diálogo, de una imagen poderosa o de un giro argumental futuro. El módulo opera con la misma lógica ABMC (alta, baja, modificación y consulta) que el resto; así, el guionista conserva sus chispazos creativos bien ordenados y listos para arrastrarlos a la estructura cuando cobren forma.

#### Exportación a Fountain: del tablero al guion literario

Cuando el guionista siente que su andamiaje narrativo está listo, **DREAMINK compacta todo en un archivo Fountain**. El tratamiento, los actos, las secuencias, las escenas (con su título descriptivo como comentario), los personajes y las locaciones viajan al documento de texto plano conservando la jerarquía y el orden establecidos en el tablero. El resultado es un esqueleto de guion literario que puede abrirse en cualquier editor compatible o seguirse puliendo en un simple editor de texto; no hay bloqueo a formatos propietarios ni pérdida de información durante la transición.

#### Alcance y filosofía de simplicidad

Fiel a su espíritu de herramienta previa al guion literario, DREAMINK **no introduce autenticación ni perfiles de usuario**; asume un entorno monousuario y local. Tampoco aborda la construcción de series (temporadas y episodios) ni la fase de guion técnico. El objetivo es mantenerse liviano y enfocado, dejando la puerta abierta a futuras extensiones pero sin sobrecargar la experiencia inicial.

En síntesis, la nueva versión de DREAMINK se presenta como un **corkboard digital altamente configurable**: desde el tratamiento global hasta la colorida malla de escenas, pasando por personajes, lugares e ideas sueltas, todo converge en un espacio único donde la historia respira antes de tomar la forma de guion literario.
