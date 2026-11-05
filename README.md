# SDD AI Toolkit

**Biblioteca de prompts en español para desarrollar software con inteligencia artificial siguiendo Spec-Driven Development (SDD).**

Desde la idea inicial hasta la implementación, las pruebas y la preparación del despliegue, con un proceso estructurado, adaptable y basado en especificaciones.

> **La IA ayuda a construir. Las especificaciones guían el desarrollo. Tú mantienes el control.**

---

## ¿Qué es SDD AI Toolkit?

**SDD AI Toolkit**, originalmente denominado **MisInstruccionesSW**, es una biblioteca de **19 instrucciones reutilizables en Markdown** para trabajar con asistentes de inteligencia artificial durante el ciclo de desarrollo de software.

Su objetivo es ayudarte a desarrollar proyectos de forma organizada, evitando empezar directamente por el código sin haber definido antes qué necesitas construir.

La metodología se basa en **Spec-Driven Development (SDD)**: utilizar especificaciones claras y verificables para orientar las decisiones técnicas, la implementación y la validación.

### ¿Qué puedes hacer con esta biblioteca?

- Transformar una idea en requisitos claros.
    
- Definir el alcance de un proyecto.
    
- Diseñar su arquitectura, datos y seguridad.
    
- Planificar un MVP y dividir el trabajo en tareas.
    
- Implementar cambios de forma incremental.
    
- Revisar código y preparar pruebas.
    
- Evaluar riesgos de seguridad.
    
- Preparar un repositorio GitHub y un despliegue.
    
- Mantener documentación y trazabilidad entre fases.
    

**No es un generador automático de aplicaciones ni un programa ejecutable.** Es un conjunto de instrucciones que utilizas con una IA.

---

## Cómo funciona

El flujo general sigue estas etapas:

```
flowchart TD
    A["Idea"] --> B["Clasificación"]
    B --> C["Descubrimiento"]
    C --> D["Especificaciones"]
    D --> E["Diseño"]
    E --> F["Planificación"]
    F --> G["Desarrollo"]
    G --> H["Validación"]
    H --> I["Publicación"]
    H -->|Correcciones| G
```

**El proceso es adaptativo.**

Un script pequeño no necesita el mismo nivel de documentación que una aplicación multiusuario o un sistema crítico.

La primera instrucción clasifica el proyecto para determinar qué profundidad de trabajo resulta apropiada.

---

## Inicio rápido

### 1. Obtén la biblioteca

Puedes descargarla desde GitHub o clonar el repositorio:

```
git clone https://github.com/AsierDev24/sdd-ai-toolkit.git
```

También puedes abrir los archivos directamente desde GitHub.

No necesitas instalar dependencias para utilizar los prompts.

### 2. Abre tu asistente de IA

Puedes utilizar ChatGPT, Claude, Gemini u otro asistente capaz de procesar instrucciones Markdown.

El asistente debe poder acceder al contenido de los archivos que le proporciones.

**Importante:** mencionar un nombre de archivo no garantiza que la IA pueda leerlo.

### 3. Proporciona las reglas generales

Abre:

[**00 — Reglas generales**](https://chatgpt.com/c/00%20-%20Sistema/00%20-%20Reglas%20generales.md)

Copia su contenido en la conversación o adjunta el archivo.

Estas reglas establecen cómo debe trabajar la IA durante el proyecto.

### 4. Clasifica tu proyecto

Abre:

[**01 — Clasificar proyecto**](https://chatgpt.com/c/00%20-%20Sistema/01%20-%20Clasificar%20proyecto.md)

Proporciona esta segunda instrucción junto con una descripción breve de tu idea.

Puedes utilizar este mensaje:

```
Quiero comenzar un proyecto de software nuevo
utilizando SDD AI Toolkit.

Aplica las reglas generales y la instrucción
"01 - Clasificar proyecto.md" que te he proporcionado.

Mi idea es:
[DESCRIBE AQUÍ TU PROYECTO]

No escribas código todavía.

Ayúdame a clasificar el proyecto según su
complejidad, riesgos, usuarios y necesidades.

Hazme las preguntas necesarias sin inventar
información ni tomar decisiones importantes
por tu cuenta.

Al terminar, prepara project-profile.md
y espera mi aprobación antes de continuar.
```

La IA debería ayudarte a definir el perfil del proyecto y el nivel de proceso recomendado.

### 5. Guarda el resultado y continúa

Guarda el documento aprobado `project-profile.md` dentro de tu proyecto.

Después continúa con:

[**01 — Explorar idea**](https://chatgpt.com/c/01%20-%20Descubrimiento/01%20-%20Explorar%20idea.md)

Y sigue las instrucciones que correspondan según la clasificación.

**No necesitas utilizar todos los prompts en todos los proyectos.**

---

## Estructura del repositorio

```
sdd-ai-toolkit/
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

La biblioteca está organizada en **8 fases** y contiene **19 archivos Markdown de instrucciones**.

---

## Índice de instrucciones

### 00 — Sistema

Establece las reglas de trabajo y adapta la metodología al proyecto.

|Instrucción|Propósito|
|---|---|
|[00 — Reglas generales](https://chatgpt.com/c/00%20-%20Sistema/00%20-%20Reglas%20generales.md)|Define principios, restricciones, aprobaciones y trazabilidad.|
|[01 — Clasificar proyecto](https://chatgpt.com/c/00%20-%20Sistema/01%20-%20Clasificar%20proyecto.md)|Determina complejidad, riesgo y nivel de proceso.|

### 01 — Descubrimiento

Permite comprender la idea antes de convertirla en requisitos.

|Instrucción|Propósito|
|---|---|
|[01 — Explorar idea](https://chatgpt.com/c/01%20-%20Descubrimiento/01%20-%20Explorar%20idea.md)|Analiza el problema, los usuarios y los objetivos.|
|[02 — Definir alcance](https://chatgpt.com/c/01%20-%20Descubrimiento/02%20-%20Definir%20alcance.md)|Delimita lo incluido, lo excluido y las restricciones.|

### 02 — Especificaciones

Define qué debe hacer el software y cómo comprobarlo.

|Instrucción|Propósito|
|---|---|
|[03 — Requisitos funcionales](https://chatgpt.com/c/02%20-%20Especificaciones/03%20-%20Requisitos%20funcionales.md)|Describe comportamientos y funcionalidades.|
|[04 — Requisitos no funcionales](https://chatgpt.com/c/02%20-%20Especificaciones/04%20-%20Requisitos%20no%20funcionales.md)|Define restricciones y atributos de calidad.|
|[05 — Criterios de aceptación](https://chatgpt.com/c/02%20-%20Especificaciones/05%20-%20Criterios%20de%20aceptacion.md)|Establece condiciones verificables de aceptación.|

### 03 — Diseño

Define cómo se organizará la solución.

|Instrucción|Propósito|
|---|---|
|[06 — Arquitectura](https://chatgpt.com/c/03%20-%20Dise%C3%B1o/06%20-%20Arquitectura.md)|Diseña componentes, responsabilidades y decisiones técnicas.|
|[07 — Modelo de datos](https://chatgpt.com/c/03%20-%20Dise%C3%B1o/07%20-%20Modelo%20de%20datos.md)|Define estructuras, relaciones y reglas de datos.|
|[08 — Seguridad](https://chatgpt.com/c/03%20-%20Dise%C3%B1o/08%20-%20Seguridad.md)|Identifica riesgos y diseña controles de seguridad.|

### 04 — Planificación

Organiza el trabajo en entregas y tareas verificables.

|Instrucción|Propósito|
|---|---|
|[09 — Definir MVP](https://chatgpt.com/c/04%20-%20Planificacion/09%20-%20Definir%20MVP.md)|Selecciona la primera entrega mínima viable.|
|[10 — Crear roadmap](https://chatgpt.com/c/04%20-%20Planificacion/10%20-%20Crear%20roadmap.md)|Organiza entregas, dependencias e hitos.|
|[11 — Desglosar tareas](https://chatgpt.com/c/04%20-%20Planificacion/11%20-%20Desglosar%20tareas.md)|Convierte el trabajo aprobado en tareas concretas.|

### 05 — Desarrollo

Guía la implementación incremental y la revisión.

|Instrucción|Propósito|
|---|---|
|[12 — Implementar tarea](https://chatgpt.com/c/05%20-%20Desarrollo/12%20-%20Implementar%20tarea.md)|Implementa una tarea autorizada con cambios controlados.|
|[13 — Revisar código](https://chatgpt.com/c/05%20-%20Desarrollo/13%20-%20Revisar%20codigo.md)|Evalúa calidad, alcance, riesgos y posibles defectos.|

### 06 — Validación

Ayuda a obtener evidencias sobre la calidad y la seguridad.

|Instrucción|Propósito|
|---|---|
|[14 — Generar pruebas](https://chatgpt.com/c/06%20-%20Validacion/14%20-%20Generar%20pruebas.md)|Diseña y prepara pruebas vinculadas a los requisitos.|
|[15 — Auditar seguridad](https://chatgpt.com/c/06%20-%20Validacion/15%20-%20Auditar%20seguridad.md)|Evalúa controles, riesgos y evidencias de seguridad.|

### 07 — Publicación

Prepara la entrega del software sin asumir operaciones automáticas.

|Instrucción|Propósito|
|---|---|
|[16 — Preparar GitHub](https://chatgpt.com/c/07%20-%20Publicacion/16%20-%20Preparar%20GitHub.md)|Revisa la preparación del repositorio para su publicación.|
|[17 — Preparar despliegue](https://chatgpt.com/c/07%20-%20Publicacion/17%20-%20Preparar%20despliegue.md)|Planifica entornos, configuración, verificaciones y recuperación.|

---

## ¿Dónde se guardan los documentos de cada proyecto?

**Los prompts de SDD AI Toolkit son reutilizables. Los documentos generados pertenecen a cada proyecto.**

Por ejemplo:

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

Esta estructura es orientativa.

Los archivos se crean conforme resulten necesarios. No es obligatorio generarlos todos desde el primer día.

Puedes utilizar un repositorio independiente para cada proyecto.

---

## Ejemplo de uso: desarrollar una aplicación

Supongamos que quieres crear una aplicación para organizar tus gastos personales.

**Primera etapa: comprender el proyecto.**

Utilizas las reglas generales, clasificas el proyecto y exploras la idea.

**Segunda etapa: especificar.**

Defines qué operaciones realizará la aplicación, qué datos necesita y qué condiciones deben cumplirse.

**Tercera etapa: diseñar.**

Decides una arquitectura proporcionada y preparas el modelo de datos y los controles de seguridad relevantes.

**Cuarta etapa: planificar.**

Defines un MVP, organizas las entregas y creas tareas pequeñas.

**Quinta etapa: desarrollar.**

Implementas una tarea autorizada, revisas los cambios y realizas las verificaciones pertinentes.

**Sexta etapa: validar y entregar.**

Revisas pruebas y seguridad y preparas la distribución o el despliegue que corresponda.

El proceso puede repetirse cuando aparezcan nuevas necesidades.

---

## Principios de la metodología

### Especificaciones antes que código

El desarrollo parte de requisitos y decisiones suficientemente claros.

### Proceso proporcional

La profundidad de las fases depende de la complejidad y del riesgo.

### Trazabilidad

Se busca mantener relaciones entre:

**Objetivos → Requisitos → Criterios de aceptación → Tareas → Implementación → Pruebas → Evidencias**

### Desarrollo incremental

Se priorizan cambios pequeños, revisables y verificables.

### Seguridad desde el diseño

Los controles de seguridad se consideran según los riesgos reales del proyecto.

### Aprobación de decisiones importantes

La IA puede proponer soluciones, pero no debe asumir que sus propuestas están aprobadas.

### Evidencias reales

Una prueba planificada no equivale a una prueba ejecutada.

Un despliegue preparado no equivale a un despliegue realizado.

### Control de operaciones

No se deben realizar operaciones sensibles, destructivas o con efectos externos sin la autorización correspondiente.

---

## Preguntas frecuentes

### ¿Tengo que ejecutar los 19 prompts?

No. Debes utilizar los que correspondan al proyecto, con el nivel de profundidad apropiado.

Las reglas generales se aplican durante todo el proceso.

### ¿Puedo utilizarlo con cualquier IA?

Puedes utilizarlo con asistentes capaces de interpretar las instrucciones y recibir el contexto necesario.

Los resultados dependerán de las capacidades y limitaciones de cada herramienta.

### ¿Necesito Obsidian?

No. Los archivos son Markdown y pueden utilizarse con Obsidian, Visual Studio Code u otros editores.

### ¿Puedo empezar a programar antes de terminar toda la documentación?

Sí, cuando exista suficiente definición y una tarea autorizada.

El proceso es incremental: no exige diseñar cada detalle futuro antes de escribir la primera línea de código.

### ¿Cómo retomo un proyecto en una conversación nueva?

Proporciona las reglas generales, los documentos aprobados relevantes y el estado actual del proyecto.

Pide a la IA que identifique la fase, las decisiones tomadas y el siguiente paso antes de modificar nada.

### ¿Qué hago si cambian los requisitos?

Revisa el impacto sobre especificaciones, diseño, planificación, código y pruebas.

Actualiza los documentos afectados antes de implementar cambios significativos.

### ¿La biblioteca garantiza que el software generado sea correcto o seguro?

No.

Las instrucciones ayudan a estructurar el trabajo, pero no sustituyen la revisión humana, las pruebas reales ni las evaluaciones técnicas necesarias.

---

## Estado del proyecto

**Biblioteca inicial completada: 19 instrucciones distribuidas en 8 fases.**

El repositorio contiene los prompts reutilizables y esta guía de uso.

La biblioteca está disponible para su utilización manual con asistentes de IA. Su eficacia práctica deberá evaluarse y mejorarse a partir de proyectos reales.

---

## 📄 Licencia

**SDD AI Toolkit** se distribuye bajo la licencia **Creative Commons Atribución 4.0 Internacional (CC BY 4.0)**.

Puedes utilizar, copiar, modificar y compartir los prompts y la documentación, incluso para fines comerciales, siempre que cumplas las condiciones de atribución.

Al redistribuir el material, debes reconocer su autoría, incluir una referencia a la licencia e indicar si has realizado modificaciones.

**Autor:** [AsierDev24](https://github.com/AsierDev24)

**Repositorio original:** [sdd-ai-toolkit](https://github.com/AsierDev24/sdd-ai-toolkit)

Consulta el archivo [LICENSE](https://chatgpt.com/c/LICENSE) para conocer los términos completos.

Esta licencia se aplica a los materiales originales de la biblioteca sobre los que el autor tenga derechos. No sustituye las licencias de terceros ni determina automáticamente la licencia del software desarrollado utilizando estos prompts.

---

## Contribuciones y mejoras

SDD AI Toolkit puede evolucionar incorporando:

- Ejemplos completos de proyectos.
    
- Guías de inicio más breves.
    
- Plantillas de documentos.
    
- Mejoras de trazabilidad.
    
- Adaptaciones para distintos asistentes de IA.
    
- Revisiones de consistencia entre instrucciones.
    
- Correcciones basadas en experiencias reales.
    

Antes de proponer cambios, conviene revisar las reglas generales y mantener la coherencia de la biblioteca.

---

## Aviso de responsabilidad

Este proyecto proporciona instrucciones y orientaciones para el desarrollo de software asistido por IA.

Su uso no garantiza resultados correctos, seguros, completos ni adecuados para un entorno de producción.

Cada usuario es responsable de revisar las decisiones, el código, las dependencias, los resultados de pruebas y las operaciones que autorice.

---

**SDD AI Toolkit**

_De la idea al software, con especificaciones, trazabilidad y control._