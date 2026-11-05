# MisInstruccionesSW

**Biblioteca reutilizable de instrucciones para desarrollar software con inteligencia artificial mediante Spec-Driven Development (SDD).**

De una idea a un proyecto funcional, documentado, probado y preparado para su publicación, manteniendo el control sobre las decisiones técnicas y los cambios realizados.

---

## ¿Qué es MisInstruccionesSW?

**MisInstruccionesSW** es una colección de prompts en formato Markdown diseñada para trabajar con asistentes de inteligencia artificial durante todo el ciclo de desarrollo de software.

Su propósito es evitar que el desarrollo comience directamente escribiendo código sin haber entendido primero el problema.

En lugar de pedir simplemente:

> Hazme una aplicación para gestionar mis gastos.

La biblioteca propone un proceso:

**Idea → Descubrimiento → Requisitos → Diseño → Planificación → Desarrollo → Validación → Publicación**

Cada etapa dispone de instrucciones que ayudan a la IA a trabajar de manera ordenada, con documentación, trazabilidad y aprobaciones.

### ¿Para qué proyectos sirve?

Está pensada para adaptarse a distintos tipos de software:

- Scripts y automatizaciones.
    
- Herramientas de línea de comandos.
    
- Bibliotecas y paquetes.
    
- Proyectos personales.
    
- Aplicaciones web y de escritorio.
    
- APIs y servicios backend.
    
- Proyectos de código abierto.
    
- Sistemas multiusuario.
    
- Aplicaciones profesionales.
    
- Sistemas que incorporan inteligencia artificial.
    

**No todos los proyectos necesitan el mismo proceso.** La biblioteca clasifica inicialmente cada proyecto y ajusta el nivel de detalle según su complejidad y riesgo.

---

## ¿Qué necesito para utilizarla?

Necesitas:

1. Un asistente de IA capaz de trabajar con instrucciones y documentos Markdown.
    
2. Acceso a los archivos de esta biblioteca.
    
3. Una carpeta independiente para guardar los documentos de cada proyecto.
    
4. Un editor, como Obsidian o Visual Studio Code.
    

**Opcionalmente:**

- Git para controlar versiones.
    
- GitHub para alojar repositorios.
    
- Un asistente de programación con acceso al código.
    
- Herramientas de pruebas y desarrollo propias del proyecto.
    

No es necesario instalar ningún paquete específico de MisInstruccionesSW.

La biblioteca contiene instrucciones, no un ejecutable.

---

## Estructura de la biblioteca

```
MisInstruccionesSW/
│
├── README.md
│
├── 00 - Sistema/
│   ├── 00 - Reglas generales.md
│   └── 01 - Clasificar proyecto.md
│
├── 01 - Descubrimiento/
│   ├── 01 - Explorar idea.md
│   └── 02 - Definir alcance.md
│
├── 02 - Especificaciones/
│   ├── 03 - Requisitos funcionales.md
│   ├── 04 - Requisitos no funcionales.md
│   └── 05 - Criterios de aceptacion.md
│
├── 03 - Diseño/
│   ├── 06 - Arquitectura.md
│   ├── 07 - Modelo de datos.md
│   └── 08 - Seguridad.md
│
├── 04 - Planificacion/
│   ├── 09 - Definir MVP.md
│   ├── 10 - Crear roadmap.md
│   └── 11 - Desglosar tareas.md
│
├── 05 - Desarrollo/
│   ├── 12 - Implementar tarea.md
│   └── 13 - Revisar codigo.md
│
├── 06 - Validacion/
│   ├── 14 - Generar pruebas.md
│   └── 15 - Auditar seguridad.md
│
└── 07 - Publicacion/
    ├── 16 - Preparar GitHub.md
    └── 17 - Preparar despliegue.md
```

La biblioteca contiene **19 archivos de instrucciones**: las reglas generales y 18 prompts operativos.

Los números se utilizan para identificar las instrucciones y su orden lógico dentro del proceso.

---

# Guía de inicio rápido

## Paso 1. Crear un proyecto nuevo

Imagina que quieres desarrollar una aplicación para gestionar gastos personales.

Primero crea una carpeta independiente.

```
MisProyectos/
└── ControlGastos/
```

La carpeta `MisInstruccionesSW` contiene las instrucciones reutilizables.

La carpeta `ControlGastos` contendrá los documentos, el código y las pruebas de ese proyecto concreto.

**No mezcles ambos contenidos.**

## Paso 2. Iniciar una conversación con la IA

Abre una conversación nueva con tu asistente de IA.

Proporciónale el contenido de:

`00 - Sistema/00 - Reglas generales.md`

Después, envía este mensaje:

```
Vamos a comenzar un proyecto de software nuevo.

Quiero que trabajemos utilizando mi metodología
MisInstruccionesSW, basada en Spec-Driven Development.

Aplica las reglas generales que te he proporcionado.

No empieces a escribir código.

Primero vamos a clasificar el proyecto y después
seguiremos las fases que correspondan.

Quiero que me hagas las preguntas necesarias,
sin inventar requisitos ni tomar decisiones
importantes por tu cuenta.

Cuando una fase esté lista, presenta sus resultados
y espera mi aprobación antes de continuar.
```

**Importante:** no presupongas que una IA conoce automáticamente esta biblioteca. Debes proporcionarle las instrucciones y el contexto necesarios, ya sea pegando el contenido, adjuntando archivos o trabajando en un entorno donde pueda leerlos.

## Paso 3. Clasificar el proyecto

Proporciona a la IA:

`00 - Sistema/01 - Clasificar proyecto.md`

Explica tu idea:

```
Quiero crear una aplicación para gestionar mis
gastos personales.

Inicialmente la utilizaré yo, pero podría
ampliarla en el futuro.

Ayúdame a clasificar el proyecto siguiendo
la instrucción proporcionada.
```

La IA debería ayudarte a identificar:

- Tipo de proyecto.
    
- Usuarios previstos.
    
- Complejidad técnica.
    
- Riesgos.
    
- Sensibilidad de los datos.
    
- Necesidades de seguridad.
    
- Nivel de proceso recomendado.
    

El resultado será un documento del proyecto:

`project-profile.md`

Guárdalo en la carpeta de tu proyecto.

No es necesario aceptar todas las recomendaciones de la IA. Puedes corregirlas antes de aprobar el documento.

## Paso 4. Explorar la idea

Cuando hayas aprobado la clasificación, proporciona:

`01 - Descubrimiento/01 - Explorar idea.md`

Mensaje de ejemplo:

```
Continuemos con el proyecto ControlGastos.

Aplica la instrucción "01 - Explorar idea.md".

Utiliza las reglas generales y el
project-profile.md aprobado.

Ayúdame a definir el problema, los usuarios,
los objetivos y las funcionalidades generales.

No diseñes todavía la arquitectura ni escribas código.

Al finalizar, prepara el contenido de vision.md
para que pueda revisarlo y aprobarlo.
```

El resultado será:

`vision.md`

Después continúa con:

`02 - Definir alcance.md`

El resultado será:

`scope.md`

Estos documentos sirven como base para las especificaciones.

## Paso 5. Continuar por las fases necesarias

A partir de aquí, utiliza los prompts correspondientes.

|Fase|Qué se hace|Documentos habituales|
|---|---|---|
|Sistema|Clasificar el proyecto|`project-profile.md`|
|Descubrimiento|Entender la idea y el alcance|`vision.md`, `scope.md`|
|Especificaciones|Definir comportamientos y criterios|`functional-requirements.md`, `non-functional-requirements.md`, `acceptance-criteria.md`|
|Diseño|Definir arquitectura, datos y seguridad|`architecture.md`, `data-model.md`, `security-design.md`|
|Planificación|Elegir MVP, entregas y tareas|`mvp-definition.md`, `roadmap.md`, `tasks.md`|
|Desarrollo|Implementar y revisar cambios|Código, registro de implementación e informe de revisión|
|Validación|Preparar y ejecutar pruebas; evaluar seguridad|`test-plan.md`, `test-results.md`, `security-audit.md`|
|Publicación|Preparar repositorio y despliegue|`github-readiness.md`, `deployment-readiness.md`|

Los nombres de documentos son convenciones de trabajo. Algunos entregables pueden simplificarse, combinarse u omitirse justificadamente según el proyecto.

---

# Cómo utilizar cada prompt

El patrón es siempre parecido.

### 1. Selecciona la instrucción

Por ejemplo:

`04 - Planificacion/11 - Desglosar tareas.md`

### 2. Proporciona el contexto necesario

La IA debe disponer de las reglas generales y de los documentos aprobados relevantes para esa instrucción.

No basta con mencionar un archivo si la IA no puede acceder a su contenido.

### 3. Indica qué quieres hacer

Por ejemplo:

```
Vamos a desglosar las tareas de la primera
entrega aprobada.

Aplica la instrucción "11 - Desglosar tareas.md".

Utiliza el MVP, el roadmap y las especificaciones
aprobadas.

No implementes código todavía.

Prepara tasks.md con tareas pequeñas,
dependencias, criterios de finalización
y trazabilidad.

Espera mi aprobación.
```

### 4. Revisa el resultado

Comprueba que:

- Responde a tu objetivo.
    
- No incluye requisitos inventados.
    
- No contradice decisiones anteriores.
    
- Distingue propuestas de decisiones aprobadas.
    
- Mantiene el alcance.
    
- Identifica dudas y riesgos.
    

### 5. Aprueba o solicita cambios

Puedes responder:

```
Apruebo esta versión de tasks.md.

Guárdala como referencia aprobada para
la siguiente fase.
```

O bien:

```
Todavía no lo apruebo.

Quiero modificar estas partes:
[...]

Actualiza el documento y vuelve a
presentarlo para revisión.
```

### 6. Guarda el documento

Conserva el resultado aprobado en el proyecto.

Si la IA tiene acceso a archivos, puedes autorizarle a crearlos o actualizarlos.

Si trabajas en un chat sin acceso al sistema de archivos, guarda el Markdown manualmente.

---

# Organización recomendada de un proyecto

Un proyecto puede comenzar con una estructura sencilla:

```
MisProyectos/
└── ControlGastos/
    ├── docs/
    │   └── sdd/
    │       ├── project-profile.md
    │       ├── vision.md
    │       ├── scope.md
    │       ├── functional-requirements.md
    │       ├── non-functional-requirements.md
    │       ├── acceptance-criteria.md
    │       ├── architecture.md
    │       ├── data-model.md
    │       ├── security-design.md
    │       ├── mvp-definition.md
    │       ├── roadmap.md
    │       └── tasks.md
    │
    ├── src/
    ├── tests/
    └── README.md
```

**Esta estructura es ilustrativa, no obligatoria.**

Al principio no necesitas crear todos los archivos ni las carpetas de código. Puedes ir añadiéndolos conforme avances.

Para un script pequeño, varios documentos podrían ser mucho más breves.

Para una aplicación compleja, puede ser conveniente conservar una documentación más detallada.

---

# ¿Tengo que utilizar todos los prompts?

**No.**

La biblioteca está diseñada para adaptar el proceso al proyecto.

### Ejemplo A: script pequeño

Quieres crear un script que organice automáticamente archivos de una carpeta.

Podría ser suficiente:

1. Clasificar el proyecto.
    
2. Explorar y delimitar brevemente la idea.
    
3. Definir requisitos y criterios esenciales.
    
4. Elegir una solución sencilla.
    
5. Planificar una tarea pequeña.
    
6. Implementar.
    
7. Revisar y probar.
    
8. Documentar el uso.
    

No tendría sentido inventar una base de datos, un sistema multiusuario o una infraestructura cloud.

### Ejemplo B: aplicación personal

Quieres una aplicación para gestionar tus gastos.

Probablemente necesitarás mayor atención a:

- Requisitos.
    
- Modelo de datos.
    
- Seguridad.
    
- MVP.
    
- Pruebas.
    
- Persistencia.
    
- Configuración.
    
- Publicación.
    

### Ejemplo C: aplicación multiusuario

Quieres desarrollar una plataforma para múltiples usuarios.

El proceso probablemente requerirá mayor profundidad en:

- Autenticación.
    
- Autorización.
    
- Aislamiento de datos.
    
- Privacidad.
    
- Arquitectura.
    
- Integraciones.
    
- Pruebas.
    
- Auditoría.
    
- Despliegue.
    
- Recuperación.
    

**La clasificación inicial orienta el nivel de rigor. No es una excusa para omitir controles indispensables.**

---

# ¿Cuándo empiezo a escribir código?

Cuando exista suficiente definición y una tarea autorizada para implementar.

El flujo habitual es:

```
Idea
  ↓
Requisitos aprobados
  ↓
Diseño suficiente
  ↓
MVP definido
  ↓
Roadmap
  ↓
Tareas aprobadas
  ↓
Implementar una tarea
  ↓
Revisar el código
  ↓
Probar
  ↓
Corregir si es necesario
  ↓
Continuar con la siguiente tarea
```

No necesitas terminar toda la aplicación antes de probarla.

La biblioteca favorece el desarrollo incremental: construir partes pequeñas, comprobarlas y continuar.

---

# Cómo trabajar con un asistente de programación

Cuando llegues a la fase de desarrollo, puedes utilizar un asistente con acceso al repositorio.

Por ejemplo, para implementar una tarea:

```
Aplica las reglas generales de MisInstruccionesSW
y la instrucción "12 - Implementar tarea.md".

Quiero implementar TASK-001.

Consulta las especificaciones aprobadas,
la arquitectura y tasks.md.

Inspecciona primero el repositorio real.

No modifiques archivos fuera del alcance
sin consultarme.

Implementa el cambio mínimo necesario.

Ejecuta únicamente las verificaciones seguras
y autorizadas que estén disponibles.

Al terminar, indícame:

- Qué archivos modificaste.
- Qué cambios realizaste.
- Qué pruebas ejecutaste realmente.
- Qué resultados obtuviste.
- Qué quedó pendiente.
- Qué riesgos o bloqueos detectaste.

No hagas commit, push ni despliegues.
```

Después puedes utilizar:

`13 - Revisar codigo.md`

Y continuar con las instrucciones de validación.

**Importante:** una IA puede equivocarse. Revisa especialmente los cambios que afecten a datos, permisos, seguridad, costes o servicios externos.

---

# Cómo retomar un proyecto otro día

No necesitas repetir todo el proceso.

Conserva los documentos aprobados y proporciona a la IA el contexto relevante.

Ejemplo:

```
Vamos a retomar el proyecto ControlGastos.

Estamos utilizando MisInstruccionesSW.

Aplica las reglas generales.

Te proporcionaré los documentos aprobados
y el estado actual del proyecto.

Primero revisa el contexto y dime:

1. En qué fase estamos.
2. Qué está aprobado.
3. Qué tareas están pendientes.
4. Qué información falta.
5. Cuál es el siguiente paso recomendado.

No modifiques código ni documentos todavía.
```

Esto es especialmente importante cuando:

- Abres una conversación nueva.
    
- Cambias de asistente.
    
- Retomas el proyecto después de varias semanas.
    
- Incorporas colaboradores.
    
- Cambias requisitos.
    

**La documentación aprobada es la referencia del proyecto, no la memoria informal de una conversación.**

---

# Cómo gestionar cambios de requisitos

Es normal que una idea evolucione.

Supongamos que inicialmente la aplicación era personal, pero ahora quieres que tenga múltiples usuarios.

No conviene pedir directamente:

> Añade usuarios y contraseñas.

Es mejor comenzar con:

```
Quiero proponer un cambio de alcance.

La aplicación pasará de uso personal
a permitir múltiples usuarios.

Revisa qué documentos SDD se verían afectados.

Identifica cambios necesarios en requisitos,
arquitectura, datos, seguridad, MVP,
roadmap, tareas y pruebas.

No implementes todavía.

Preséntame el análisis de impacto
para decidir qué cambios aprobar.
```

Después se actualizan las especificaciones afectadas y se planifican las tareas correspondientes.

Así se evita que el código evolucione sin que la documentación refleje lo que realmente debe hacer.

---

# Principios de trabajo

## 1. Especificar antes de implementar

Primero entender qué se necesita.

Después decidir cómo construirlo.

## 2. No inventar decisiones

Si falta información, la IA debe preguntar o marcarla como pendiente.

## 3. Mantener la trazabilidad

Cada cambio importante debería poder relacionarse con su necesidad original.

Por ejemplo:

```
Objetivo
   ↓
Requisito
   ↓
Criterio de aceptación
   ↓
Tarea
   ↓
Código
   ↓
Prueba
   ↓
Evidencia
```

## 4. Trabajar incrementalmente

Preferir tareas pequeñas y verificables.

## 5. Aplicar seguridad proporcional

No todos los proyectos tienen el mismo riesgo, pero ninguno debe ignorar riesgos relevantes.

## 6. Diferenciar propuesta y aprobación

La IA puede recomendar.

Las decisiones importantes deben confirmarse.

## 7. No inventar resultados

Una prueba diseñada no es una prueba ejecutada.

Un informe de revisión no equivale a una auditoría.

Un repositorio preparado no significa que esté publicado.

Un despliegue preparado no significa que esté ejecutado.

## 8. Mantener el control humano

No realizar automáticamente operaciones sensibles, destructivas o externas sin autorización.

---

# Errores frecuentes que conviene evitar

### Empezar directamente por el código

Puede provocar cambios de alcance y retrabajo.

**Mejor:** clasificar el proyecto y definir primero lo esencial.

### Pasar todos los prompts a la IA de golpe

Puede generar respuestas enormes, confusas o inconsistentes.

**Mejor:** trabajar fase por fase y aprobar resultados.

### Crear documentación innecesaria

Un script pequeño no necesita la misma documentación que una plataforma profesional.

**Mejor:** adaptar la profundidad al riesgo y complejidad.

### No guardar los documentos

La conversación puede perder contexto o no estar disponible en otra herramienta.

**Mejor:** mantener los documentos del proyecto en archivos Markdown.

### Confiar en pruebas no ejecutadas

Que la IA escriba un test no demuestra que funcione.

**Mejor:** conservar resultados y evidencias reales.

### Publicar sin revisar

Un repositorio puede contener secretos, datos privados o código que no debe distribuirse.

**Mejor:** utilizar las instrucciones de validación y publicación antes de exponerlo.

---

# ¿Cómo usar MisInstruccionesSW con Obsidian?

Obsidian es una forma cómoda de organizar la biblioteca.

1. Abre tu bóveda de Obsidian.
    
2. Guarda la carpeta `MisInstruccionesSW` dentro de ella.
    
3. Abre el prompt que necesites.
    
4. Copia su contenido al asistente de IA o facilítale acceso al archivo.
    
5. Guarda los resultados en la carpeta del proyecto.
    
6. Revisa y aprueba antes de avanzar.
    

También puedes utilizar cualquier editor compatible con Markdown.

**Obsidian no es obligatorio.**

---

# ¿Cómo usarla con GitHub?

GitHub puede servir para:

- Guardar la biblioteca.
    
- Mantener su historial.
    
- Acceder a ella desde diferentes equipos.
    
- Proponer mejoras.
    
- Compartirla con otras personas.
    

### Recomendación de organización

Mantén repositorios separados:

```
GitHub/
├── MisInstruccionesSW/
├── ControlGastos/
├── OrganizadorArchivos/
└── OtroProyecto/
```

`MisInstruccionesSW` contiene las instrucciones reutilizables.

Cada proyecto mantiene su propio código y documentación.

No necesitas copiar toda la biblioteca dentro de cada proyecto.

### Antes de hacer público el repositorio

Revisa:

- Que no contenga secretos.
    
- Que no incluya información privada.
    
- Que los archivos sean los que deseas compartir.
    
- Que tengas derechos para publicar su contenido.
    
- Qué licencia quieres utilizar.
    

**Licencia:** pendiente de decisión del responsable del repositorio.

No se presupone ninguna licencia de código abierto.

---

# Referencia rápida: ¿qué prompt utilizo?

|Si quiero...|Utilizo...|
|---|---|
|Empezar un proyecto|`01 - Clasificar proyecto.md`|
|Aclarar una idea|`01 - Explorar idea.md`|
|Decidir qué incluye|`02 - Definir alcance.md`|
|Definir funcionalidades|`03 - Requisitos funcionales.md`|
|Definir calidad y restricciones|`04 - Requisitos no funcionales.md`|
|Saber cuándo algo está bien hecho|`05 - Criterios de aceptacion.md`|
|Diseñar la solución|`06 - Arquitectura.md`|
|Diseñar los datos|`07 - Modelo de datos.md`|
|Diseñar controles de seguridad|`08 - Seguridad.md`|
|Decidir qué construir primero|`09 - Definir MVP.md`|
|Organizar entregas|`10 - Crear roadmap.md`|
|Crear tareas concretas|`11 - Desglosar tareas.md`|
|Programar una tarea|`12 - Implementar tarea.md`|
|Revisar cambios de código|`13 - Revisar codigo.md`|
|Diseñar y generar pruebas|`14 - Generar pruebas.md`|
|Evaluar seguridad|`15 - Auditar seguridad.md`|
|Preparar un repositorio|`16 - Preparar GitHub.md`|
|Preparar una puesta en funcionamiento|`17 - Preparar despliegue.md`|

**En todas las fases se aplican las reglas generales y se consulta el contexto aprobado relevante.**

---

# Flujo recomendado para mi primer proyecto

Si es la primera vez que utilizas MisInstruccionesSW:

1. Elige un proyecto pequeño y concreto.
    
2. Crea su carpeta.
    
3. Proporciona las reglas generales a la IA.
    
4. Clasifica el proyecto.
    
5. Explora la idea.
    
6. Define el alcance.
    
7. Especifica lo necesario.
    
8. Diseña una solución sencilla.
    
9. Define una primera entrega pequeña.
    
10. Desglosa las tareas.
    
11. Implementa una tarea.
    
12. Revisa y prueba.
    
13. Repite hasta completar la entrega.
    
14. Prepara GitHub o la distribución que corresponda.
    
15. Documenta el resultado y las decisiones pendientes.
    

No es necesario completar todas las fases con el mismo nivel de detalle.

---

# Evolución de la biblioteca

MisInstruccionesSW puede evolucionar con el uso.

Posibles mejoras futuras:

- Ejemplos completos de proyectos.
    
- Plantillas de documentos generados.
    
- Guías para diferentes asistentes de IA.
    
- Automatización de creación de proyectos.
    
- Comprobaciones de consistencia.
    
- Mejoras de trazabilidad.
    
- Adaptaciones a distintos ecosistemas.
    
- Nuevos prompts especializados.
    

Cualquier cambio debe mantener la coherencia entre instrucciones y evitar contradicciones.

---

# Estado del proyecto

**MisInstruccionesSW — Versión inicial de la biblioteca de prompts completada.**

La biblioteca está preparada para comenzar a utilizarse manualmente con asistentes de IA.

Esto no implica que todos sus prompts hayan sido probados en proyectos reales ni que se haya realizado una validación transversal completa.

La metodología podrá refinarse a partir de la experiencia práctica.

---

# Resumen

MisInstruccionesSW busca que desarrollar software con inteligencia artificial no sea simplemente pedir código, sino seguir un proceso controlado:

**Entender → Especificar → Diseñar → Planificar → Construir → Verificar → Entregar**

La IA ayuda a realizar el trabajo.

Las especificaciones conservan las decisiones.

Las pruebas aportan evidencias.

Y la persona responsable mantiene el control del proyecto.