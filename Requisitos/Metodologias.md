# Análisis y Diseño

## Metodologías no Convencionales para el Levantamiento de Requerimientos

Este documento presenta un conjunto de metodologías poco comunes para el levantamiento de requerimientos de software, adaptadas al contexto del proyecto **DREAMINK**. Su objetivo es ampliar las formas tradicionales de recolección de requisitos, priorizando técnicas que minimicen la interacción constante con el usuario final y permitan validar y refinar los requisitos de manera ágil.

### 1. Prototipado Desechable (*Throwaway Prototyping*)

**Descripción:**  
Se desarrollan prototipos rápidos, de baja fidelidad, que no se integrarán al producto final. El objetivo es validar ideas, flujos y requisitos antes de invertir en un diseño definitivo.

**Aplicación en *DREAMINK*:**  
- Crear un prototipo interactivo simple del *tablero narrativo* usando herramientas como Figma o Miro.
- Simular la creación de actos, secuencias y escenas con colores asignados.  
- Presentar el prototipo a guionistas para recibir retroalimentación temprana.  
- Ajustar la lógica de interacción y el orden de las funciones antes de escribir código.

**Ejemplo:**  
Se crea un prototipo con tres pantallas:
1. **Vista general del tablero:** columnas para actos y tarjetas para secuencias y escenas.
2. **Formulario de escena:** campos para título, descripción y selección de color.
3. **Exportación simulada:** vista previa de cómo quedaría el archivo Fountain.

El guionista interactúa con el prototipo y comenta si el flujo le resulta natural o si prefiere otros pasos.

### 2. Storyboarding Funcional

**Descripción:**  
Similar al storyboard cinematográfico, pero aplicado al software. Se representan visualmente las interacciones paso a paso del usuario con el sistema.

**Aplicación en DREAMINK:**  
- Documentar gráficamente cómo un usuario pasa de una idea suelta a integrarla en un acto y secuencia.
- Identificar en el storyboard cuántos clics o acciones se requieren y si existen redundancias.

**Ejemplo:**  
Storyboard para el caso: *"Transformar una idea suelta en una escena"*  
1. Usuario abre la sección **Ideas Sueltas**.
2. Selecciona una idea y la arrastra al acto correspondiente.
3. El sistema abre un formulario de escena para completar detalles.
4. Escena aparece en el tablero con el color seleccionado.

### 3. Análisis de Documentos

**Descripción:**  
Consiste en estudiar documentos, guiones y plantillas reales para extraer patrones y requisitos que se usan en la práctica.

**Aplicación en DREAMINK:**  
- Analizar guiones en formato Fountain de distintos géneros.
- Identificar campos y convenciones que se repiten (p.ej., encabezados de escena, manejo de diálogos).
- Incorporar esos campos en el diseño de exportación.

**Ejemplo:**  
Del análisis de varios guiones se detecta que muchos incluyen un campo “NOTAS DEL DIRECTOR” al final de la escena. Aunque no se usa en todos, se podría ofrecer como campo opcional en el módulo de escenas.

### 4. Ingeniería Inversa de Software Heredado

**Descripción:**  
Analizar herramientas similares, especialmente open source, para comprender cómo estructuran la información y qué funcionalidades ofrecen.

**Aplicación en DREAMINK:**  
- Revisar herramientas como **Trelby**, **KIT Scenarist** o **WriterDuet** (versión gratuita).
- Mapear qué funciones tienen en común y qué problemas mencionan sus usuarios.
- Tomar inspiración en funciones útiles y evitar errores comunes.

**Ejemplo:**  
Al analizar Trelby se observa que la exportación a PDF es rígida y no personalizable. DREAMINK podría diferenciarse ofreciendo más control en la exportación Fountain.

### 5. Análisis de Escenarios con Mínima Interacción

**Descripción:**  
Definir escenarios narrativos basados en observaciones, sin depender de entrevistas prolongadas con usuarios.

**Aplicación en DREAMINK:**  
- Describir cómo un guionista con poco tiempo usaría la aplicación en un descanso de 10 minutos.
- Identificar requisitos de usabilidad como guardado automático o acceso rápido desde móvil.

**Ejemplo:**  
Escenario: *"Capturar una idea en el móvil y retomarla en el PC"*
1. Usuario abre DREAMINK en su teléfono.
2. Añade una idea suelta con título y breve descripción.
3. Al llegar a su casa, abre DREAMINK en su computadora y la idea aparece lista para integrar en la estructura.

### 6. Combinación de Técnicas

Para obtener mejores resultados, se recomienda **combinar las metodologías** anteriores. Por ejemplo:
- **Prototipado + Storyboarding:** crear un prototipo y acompañarlo de un storyboard para que los guionistas comprendan el flujo antes de probarlo.
- **Análisis de Documentos + Ingeniería Inversa:** revisar guiones reales y herramientas existentes para asegurarse de cubrir campos importantes y flujos eficientes.

## Conclusión

El uso de metodologías no convencionales en el levantamiento de requerimientos para DREAMINK permitirá:
- Reducir malentendidos.
- Ahorrar tiempo y recursos.
- Asegurar que el sistema se ajuste a las prácticas reales de los guionistas.
- Diferenciar el producto de soluciones existentes, aportando valor en aspectos donde otras herramientas son rígidas.

Estas metodologías complementan el análisis de requisitos ya realizado y servirán como base sólida para pasar a la siguiente fase: **análisis de sistemas y diseño**.
