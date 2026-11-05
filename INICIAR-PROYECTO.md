# 🚀 Iniciar un proyecto con SDD AI Toolkit

Esta guía explica cómo comenzar, continuar y retomar un proyecto de software utilizando los prompts de **SDD AI Toolkit**.

No necesitas ejecutar herramientas especiales ni instalar dependencias. Solo necesitas un asistente de IA, los archivos Markdown de esta biblioteca y un lugar donde guardar la documentación de tu proyecto.

> **Regla principal:** no empieces pidiendo código. Primero comprende, especifica y planifica lo necesario.

---

## 1. Antes de empezar

Necesitas:

- Una idea de proyecto, aunque todavía no esté completamente definida.
    
- Un asistente de IA, como ChatGPT, Claude, Gemini o un asistente de programación.
    
- Acceso a los prompts de este repositorio.
    
- Una carpeta independiente para guardar el proyecto.
    

Puedes descargar la biblioteca con:

```
git clone https://github.com/AsierDev24/sdd-ai-toolkit.git
```

O consultar los archivos directamente en GitHub.

**Importante:** esta biblioteca contiene instrucciones reutilizables. El código y la documentación generados deben guardarse en la carpeta del proyecto, no dentro de `sdd-ai-toolkit`.

---

## 2. Crear la carpeta del proyecto

Por ejemplo, si vas a desarrollar una aplicación de gastos:

```
MisProyectos/
└── ControlGastos/
    └── docs/
        └── sdd/
```

No necesitas crear todavía carpetas de código ni todos los documentos SDD.

La estructura crecerá según las necesidades del proyecto.

---

## 3. Proporcionar las reglas generales

Abre este archivo:

[**00 - Reglas generales.md**](https://chatgpt.com/c/00%20-%20Sistema/00%20-%20Reglas%20generales.md)

Copia su contenido en una conversación nueva con la IA o adjunta el archivo.

Estas reglas deben mantenerse como referencia durante todas las fases.

Si cambias de conversación o asistente, tendrás que volver a proporcionar las instrucciones necesarias, salvo que la herramienta ya tenga acceso efectivo a ellas.

---

## 4. Copiar el prompt de inicio

Después de proporcionar las reglas generales, copia este mensaje:

```
Quiero comenzar un proyecto de software utilizando
SDD AI Toolkit, una biblioteca de instrucciones
basada en Spec-Driven Development (SDD).

Aplica las reglas generales que te he proporcionado.

Vamos a trabajar de forma incremental y adaptando
la profundidad del proceso a la complejidad y
los riesgos reales del proyecto.

Estas son las condiciones de trabajo:

1. No escribas código antes de que exista una
   definición suficiente y una tarea autorizada.

2. No inventes requisitos, decisiones, resultados
   de pruebas ni información del proyecto.

3. Distingue claramente entre información
   confirmada, propuestas, suposiciones y
   cuestiones pendientes.

4. Hazme las preguntas necesarias para avanzar,
   preferiblemente en grupos pequeños.

5. Utiliza los documentos aprobados como
   referencia del proyecto.

6. Antes de avanzar entre fases importantes,
   presenta el resultado y solicita mi aprobación.

7. No realices commits, push, despliegues,
   operaciones destructivas ni acciones externas
   sensibles sin mi autorización.

8. Indica qué documentación debería guardar
   y qué fase corresponde ejecutar después.

Mi idea inicial es:

[ESCRIBE AQUÍ TU IDEA]

Primero vamos a clasificar el proyecto.

No implementes nada todavía.
```

Este mensaje establece el contexto inicial, pero **no sustituye el contenido de los prompts de la biblioteca**.

---

## 5. Clasificar el proyecto

Proporciona ahora:

[**01 - Clasificar proyecto.md**](https://chatgpt.com/c/00%20-%20Sistema/01%20-%20Clasificar%20proyecto.md)

Y envía:

```
Aplica la instrucción "01 - Clasificar proyecto.md"
a la idea que te he explicado.

Utiliza las reglas generales.

Ayúdame a identificar el tipo de proyecto,
su complejidad, riesgos, usuarios y necesidades.

Recomienda el nivel de proceso SDD adecuado.

Prepara el contenido de project-profile.md.

No avances a la siguiente fase hasta que
revise y apruebe el resultado.
```

La IA debería ayudarte a decidir si el proyecto necesita un proceso ligero, estándar, avanzado o crítico, según corresponda.

Cuando estés conforme, responde:

```
Apruebo project-profile.md.

Utilizaremos este documento como referencia
para las siguientes fases.
```

Guarda el documento aprobado en:

```
MiProyecto/docs/sdd/project-profile.md
```

---

## 6. Continuar con las fases

Después de clasificar el proyecto, utiliza los prompts que correspondan.

|Fase|Objetivo|Carpeta|
|---|---|---|
|Descubrimiento|Entender la idea y definir el alcance|`01 - Descubrimiento/`|
|Especificaciones|Definir requisitos y criterios de aceptación|`02 - Especificaciones/`|
|Diseño|Definir arquitectura, datos y seguridad|`03 - Diseño/`|
|Planificación|Definir MVP, roadmap y tareas|`04 - Planificacion/`|
|Desarrollo|Implementar y revisar código|`05 - Desarrollo/`|
|Validación|Preparar pruebas y evaluar seguridad|`06 - Validacion/`|
|Publicación|Preparar GitHub y despliegue|`07 - Publicacion/`|

**No tienes que ejecutar todos los prompts obligatoriamente.**

La clasificación inicial ayuda a determinar cuáles necesitas y con qué profundidad.

### Mensaje reutilizable para cualquier fase

```
Vamos a continuar con el proyecto [NOMBRE].

Aplica las reglas generales de SDD AI Toolkit
y la instrucción [NOMBRE DEL PROMPT]
que te he proporcionado.

Ten en cuenta los documentos aprobados
relevantes para esta fase.

Estado actual:
[RESUMEN DEL ESTADO]

Objetivo de esta fase:
[QUÉ QUEREMOS CONSEGUIR]

No inventes información que falte.

Si necesitas aclaraciones, pregúntame antes
de tomar decisiones importantes.

Al terminar:
- Presenta el resultado.
- Identifica dudas y riesgos.
- Indica qué documento debo guardar.
- Propón el siguiente paso.
- Espera mi aprobación.
```

**Recuerda:** debes proporcionar el contenido real del prompt y de los documentos necesarios. No basta con indicar sus nombres si la IA no puede leerlos.

---

## 7. Guardar la documentación

Mantén los documentos aprobados dentro de tu proyecto.

Por ejemplo:

```
ControlGastos/
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
├── src/
├── tests/
└── README.md
```

Es una estructura de ejemplo, no una lista obligatoria de archivos.

Los documentos pueden simplificarse o combinarse cuando el proyecto lo justifique.

### Cómo aprobar un documento

Cuando el resultado sea correcto:

```
Apruebo la versión actual de [DOCUMENTO].

Guárdala como referencia aprobada.

Indícame qué fase corresponde después
y qué archivos necesitas para continuar.
```

Si necesitas modificaciones:

```
Todavía no apruebo [DOCUMENTO].

Quiero modificar lo siguiente:

[DESCRIBE LOS CAMBIOS]

Actualiza el documento sin alterar
las decisiones previamente aprobadas
que no estén afectadas.

Preséntamelo de nuevo para revisión.
```

---

## 8. Empezar a desarrollar

Cuando exista una tarea suficientemente definida y aprobada, utiliza:

[**12 - Implementar tarea.md**](https://chatgpt.com/c/05%20-%20Desarrollo/12%20-%20Implementar%20tarea.md)

Ejemplo:

```
Quiero implementar TASK-001.

Aplica las reglas generales y la instrucción
"12 - Implementar tarea.md".

Consulta la tarea aprobada, los requisitos
relacionados y las decisiones de diseño.

Antes de modificar código:
- Revisa el estado real del proyecto.
- Confirma el alcance de la tarea.
- Identifica posibles riesgos.

Implementa únicamente lo autorizado.

Después indica:
- Archivos modificados.
- Cambios realizados.
- Pruebas realmente ejecutadas.
- Resultados observados.
- Limitaciones y pendientes.

No hagas commit, push ni despliegues
sin mi autorización.
```

Después puedes revisar los cambios mediante:

[**13 - Revisar codigo.md**](https://chatgpt.com/c/05%20-%20Desarrollo/13%20-%20Revisar%20codigo.md)

Y utilizar las instrucciones de validación que correspondan.

---

## 9. Retomar un proyecto en otra conversación

Cuando cambies de conversación, de asistente o retomes un proyecto días después, no necesitas empezar desde cero.

Proporciona:

- Las reglas generales.
    
- Los documentos aprobados relevantes.
    
- El estado actual del proyecto.
    
- Las tareas completadas y pendientes.
    
- Los cambios importantes realizados desde la última sesión.
    

Copia este mensaje:

```
Quiero retomar un proyecto existente
que utiliza SDD AI Toolkit.

Aplica las reglas generales que te
he proporcionado.

Te facilitaré los documentos aprobados
y el estado actual del proyecto.

Antes de hacer cambios, analiza el contexto
y responde:

1. ¿Cuál es el objetivo del proyecto?
2. ¿En qué fase nos encontramos?
3. ¿Qué decisiones están aprobadas?
4. ¿Qué tareas están completadas?
5. ¿Qué tareas siguen pendientes?
6. ¿Existen contradicciones o información faltante?
7. ¿Cuál es el siguiente paso recomendado?

No escribas código ni modifiques documentos
hasta que confirme cómo continuaremos.
```

**Los documentos aprobados son la fuente de referencia.** No dependas únicamente de que una IA recuerde conversaciones anteriores.

---

## 10. Cambiar requisitos durante el desarrollo

Si cambian las necesidades del proyecto, revisa el impacto antes de programar.

Mensaje recomendado:

```
Quiero proponer un cambio en el proyecto.

Cambio solicitado:
[DESCRIBE EL CAMBIO]

Analiza qué elementos se verían afectados:

- Alcance.
- Requisitos.
- Criterios de aceptación.
- Arquitectura.
- Modelo de datos.
- Seguridad.
- MVP y roadmap.
- Tareas.
- Implementación existente.
- Pruebas.

Indica qué documentos necesitan actualizarse.

No implementes el cambio todavía.

Preséntame el análisis de impacto
para que pueda decidir qué aprobar.
```

---

## 11. Errores que debes evitar

- **Empezar directamente por el código:** primero define lo necesario.
    
- **Enviar todos los prompts a la vez:** trabaja por fases.
    
- **Confiar en nombres de archivos sin adjuntarlos:** proporciona su contenido.
    
- **No guardar documentos aprobados:** perderás trazabilidad.
    
- **Aceptar decisiones inventadas:** revisa las propuestas.
    
- **Confundir pruebas diseñadas con ejecutadas:** exige evidencias reales.
    
- **Crear documentación excesiva:** adapta el proceso al proyecto.
    
- **Publicar sin revisar:** comprueba seguridad, secretos y configuración.
    

---

## 12. Lista de comprobación

Antes de comenzar a implementar una tarea:

- He proporcionado las reglas generales.
    
- El proyecto está clasificado.
    
- He definido y aprobado el alcance necesario.
    
- Existen requisitos y criterios verificables.
    
- Tengo un diseño suficiente para la tarea.
    
- La tarea está definida y autorizada.
    
- La IA dispone del contexto relevante.
    

Antes de dar una entrega por finalizada:

- Los cambios se han revisado.
    
- Las pruebas necesarias se han ejecutado realmente.
    
- Los resultados y limitaciones están documentados.
    
- Se han evaluado los riesgos de seguridad relevantes.
    
- La documentación refleja el estado real.
    
- Las operaciones de publicación o despliegue están autorizadas.
    

---

## Enlaces útiles

- [Repositorio SDD AI Toolkit](https://github.com/AsierDev24/sdd-ai-toolkit)
    
- [README principal](https://chatgpt.com/c/README.md)
    
- [Reglas generales](https://chatgpt.com/c/00%20-%20Sistema/00%20-%20Reglas%20generales.md)
    
- [Clasificar proyecto](https://chatgpt.com/c/00%20-%20Sistema/01%20-%20Clasificar%20proyecto.md)
    
- [Explorar idea](https://chatgpt.com/c/01%20-%20Descubrimiento/01%20-%20Explorar%20idea.md)
    

---

**SDD AI Toolkit — Empieza con una idea. Avanza con especificaciones. Construye con control.**