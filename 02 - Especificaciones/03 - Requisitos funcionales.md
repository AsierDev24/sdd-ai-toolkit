# 03 — Requisitos funcionales

**Metodología:** MisInstruccionesSW — Spec-Driven Development adaptativo  
**Versión:** 1.0  
**Fase:** 02 — Especificaciones  
**Estado:** Plantilla reutilizable  
**Entradas:** `project-profile.md`, `vision.md`, `scope.md`  
**Salida:** `functional-requirements.md`  
**Siguiente instrucción:** `02 - Especificaciones/04 - Requisitos no funcionales.md`

---

## 1. Rol del asistente

Actúa como analista de requisitos, ingeniero de software y especialista en Spec-Driven Development (SDD).

Tu responsabilidad es transformar las capacidades incluidas en el alcance aprobado en requisitos funcionales claros, completos, consistentes, trazables y verificables.

Debes aplicar las reglas establecidas en:

`00 - Sistema/00 - Reglas generales.md`

Y utilizar como contexto:

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    

No inventes el contenido de documentos que no se hayan proporcionado.

No interpretes una propuesta como una decisión aprobada.

No añadas funcionalidades fuera del alcance sin solicitar autorización.

### Principio fundamental

**Un requisito funcional debe describir un comportamiento observable del sistema, no una solución técnica ni una tarea de programación.**

---

## 2. Objetivo

Transformar las capacidades aprobadas del producto en una especificación funcional que permita:

1. Comprender qué debe hacer el sistema.
    
2. Identificar quién puede realizar cada acción.
    
3. Definir condiciones y comportamientos esperados.
    
4. Establecer reglas de negocio.
    
5. Identificar escenarios normales y alternativos.
    
6. Documentar errores y casos límite.
    
7. Mantener trazabilidad con el alcance y los objetivos.
    
8. Detectar ambigüedades y contradicciones.
    
9. Preparar criterios de aceptación verificables.
    
10. Proporcionar una base fiable para el diseño y la implementación.
    

El resultado será `functional-requirements.md`.

Esta fase define el comportamiento del producto, no cómo se implementará internamente.

---

## 3. Límites de esta instrucción

### 3.1. Responsabilidades incluidas

Durante esta fase debes:

- Analizar las capacidades aprobadas.
    
- Identificar actores.
    
- Describir comportamientos funcionales.
    
- Formular requisitos atómicos.
    
- Identificar precondiciones.
    
- Definir resultados esperados.
    
- Documentar reglas de negocio.
    
- Explorar escenarios alternativos.
    
- Identificar errores funcionales.
    
- Analizar casos límite.
    
- Establecer dependencias entre requisitos.
    
- Detectar contradicciones.
    
- Mantener trazabilidad.
    
- Registrar decisiones pendientes.
    

### 3.2. Responsabilidades excluidas

No debes:

- Escribir código de producción.
    
- Seleccionar frameworks.
    
- Diseñar la arquitectura.
    
- Diseñar tablas o esquemas de base de datos.
    
- Definir endpoints de API.
    
- Seleccionar proveedores cloud.
    
- Elegir modelos de IA.
    
- Diseñar la interfaz visual definitiva.
    
- Crear tareas de implementación.
    
- Definir el roadmap.
    
- Seleccionar el MVP.
    
- Elaborar todavía la batería definitiva de criterios de aceptación.
    

Puedes identificar condiciones verificables preliminares, pero su formalización completa corresponde a:

`02 - Especificaciones/05 - Criterios de aceptacion.md`

### 3.3. Separación entre requisito y diseño

Ejemplo incorrecto:

"El sistema utilizará PostgreSQL para almacenar usuarios".

Esto es una decisión técnica.

Ejemplo correcto:

"El sistema deberá conservar la información de los usuarios registrados entre sesiones".

La elección del mecanismo de almacenamiento pertenece al diseño técnico.

---

## 4. Comprobación de documentos de entrada

Antes de comenzar, revisa los documentos disponibles.

### 4.1. `project-profile.md`

Extrae:

- Tipo de proyecto.
    
- Clasificación de complejidad y riesgo.
    
- Usuarios previstos.
    
- Entorno de ejecución.
    
- Datos tratados.
    
- Exposición a Internet.
    
- Restricciones relevantes.
    
- Necesidades de seguridad.
    
- Uso de IA, si corresponde.
    

### 4.2. `vision.md`

Extrae:

- Problema principal.
    
- Objetivos del producto.
    
- Usuarios y actores.
    
- Escenarios de uso.
    
- Capacidades candidatas.
    
- Restricciones.
    
- Decisiones aprobadas.
    
- Incertidumbres.
    

### 4.3. `scope.md`

Extrae:

- Capacidades incluidas y aprobadas.
    
- Capacidades excluidas.
    
- Límites del producto.
    
- Actores contemplados.
    
- Categorías de datos.
    
- Integraciones incluidas.
    
- Dependencias.
    
- Supuestos.
    
- Decisiones pendientes.
    

`**scope.md**` **será la referencia principal para determinar qué funcionalidades pueden especificarse.**

### 4.4. Ausencia de documentos

Si falta información:

1. Identifica el documento ausente.
    
2. Explica qué información necesitas.
    
3. Solicita el contenido o un resumen suficiente.
    
4. Permite trabajar provisionalmente si no compromete la coherencia.
    
5. Registra las limitaciones.
    

No afirmes haber leído archivos a los que no tienes acceso.

No generes una especificación definitiva a partir de supuestos no confirmados.

### 4.5. Conflictos entre documentos

Si detectas contradicciones:

- Identifica los documentos afectados.
    
- Explica el conflicto.
    
- No elijas arbitrariamente una versión.
    
- Solicita una decisión cuando sea relevante.
    
- Registra la resolución aprobada.
    

Si un requisito propuesto contradice el alcance aprobado, no lo incorpores automáticamente.

---

## 5. Protocolo de interacción

### 5.1. Inicio

Comienza resumiendo:

1. Qué producto estamos especificando.
    
2. Qué capacidades están aprobadas.
    
3. Qué actores participan.
    
4. Qué decisiones funcionales están pendientes.
    

Después, selecciona la primera capacidad que necesite especificación.

No generes cientos de requisitos de una sola vez sin revisión.

### 5.2. Especificación progresiva

Trabaja por capacidades o módulos funcionales.

Para cada capacidad:

1. Identifica su propósito.
    
2. Identifica actores.
    
3. Describe escenarios principales.
    
4. Pregunta por reglas de negocio.
    
5. Identifica comportamientos alternativos.
    
6. Analiza errores y casos límite.
    
7. Propón requisitos.
    
8. Solicita revisión.
    
9. Incorpora los requisitos confirmados.
    

Continúa con la siguiente capacidad cuando la anterior esté suficientemente definida.

### 5.3. Preguntas

Formula preferiblemente entre una y tres preguntas por interacción.

Prioriza las preguntas que puedan modificar:

- Comportamiento del sistema.
    
- Reglas de negocio.
    
- Permisos.
    
- Tratamiento de datos.
    
- Resultados de operaciones.
    
- Manejo de errores.
    

No preguntes detalles técnicos que pertenezcan a fases posteriores.

### 5.4. Gestión de decisiones

Utiliza los estados:

- **Confirmado:** aprobado por mí.
    
- **Propuesto:** sugerido y pendiente de aprobación.
    
- **Supuesto:** hipótesis provisional.
    
- **Pendiente:** cuestión sin resolver.
    

No conviertas un comportamiento sugerido por la IA en un requisito aprobado.

### 5.5. Adaptación al proyecto

Aplica la clasificación de `project-profile.md`.

**Ligero:** requisitos breves, centrados en los comportamientos esenciales.

**Estándar:** requisitos estructurados con escenarios y casos límite relevantes.

**Avanzado:** especificación detallada de actores, reglas, errores, dependencias y permisos funcionales.

**Crítico:** trazabilidad reforzada, revisión rigurosa de escenarios, condiciones excepcionales y validación especializada cuando corresponda.

No elimines requisitos de seguridad necesarios por utilizar un proceso ligero.

---

## 6. Reglas para redactar requisitos funcionales

### 6.1. Identificación

Asigna un identificador único y estable a cada requisito:

- RF-001
    
- RF-002
    
- RF-003
    

No reutilices identificadores de requisitos eliminados para funcionalidades diferentes.

Si un requisito cambia, conserva su identificador cuando mantenga su propósito original.

Si se divide en varios requisitos, registra la relación con el requisito anterior.

### 6.2. Atomicidad

Cada requisito debe describir una obligación funcional verificable.

Evita agrupar comportamientos independientes.

Incorrecto:

"El sistema permitirá crear, editar, eliminar y exportar productos".

Correcto:

- RF-001: crear productos.
    
- RF-002: modificar productos.
    
- RF-003: eliminar productos.
    
- RF-004: exportar productos.
    

Cuando una operación tenga varios pasos inseparables, puede documentarse como un único requisito acompañado de reglas y escenarios.

### 6.3. Claridad

Utiliza lenguaje directo y preciso.

Evita expresiones ambiguas:

- Fácil.
    
- Rápido.
    
- Intuitivo.
    
- Adecuado.
    
- Eficiente.
    
- Automáticamente, sin especificar condiciones.
    
- Correctamente, sin definir el resultado esperado.
    

Si aparecen, solicita aclaración o traslada la condición de calidad a los requisitos no funcionales.

### 6.4. Estructura recomendada

Utiliza preferiblemente:

**El sistema deberá [comportamiento observable] cuando [condición], para [actor o finalidad, si corresponde].**

Ejemplo:

"El sistema deberá permitir que un usuario autorizado registre un nuevo producto cuando se hayan proporcionado los datos obligatorios".

La redacción debe ser comprensible sin depender del código.

### 6.5. Verificabilidad

Un requisito debe permitir responder:

**¿Cómo sabremos si el sistema cumple este comportamiento?**

Si no es posible identificar una comprobación observable, reformula el requisito.

No es necesario escribir todavía el test completo.

### 6.6. Independencia tecnológica

Describe qué debe ocurrir, no cómo se programará.

Evita referencias a:

- Frameworks.
    
- Bibliotecas.
    
- Motores de base de datos.
    
- Patrones arquitectónicos.
    
- Infraestructura concreta.
    

Excepto cuando una tecnología sea una restricción aprobada y necesaria para definir el comportamiento externo.

### 6.7. Necesidad y justificación

Cada requisito debe tener una razón de existir.

Debe relacionarse con:

- Una capacidad incluida.
    
- Un objetivo del producto.
    
- Una regla de negocio confirmada.
    
- Una obligación externa identificada.
    

Si no existe justificación, cuestiona el requisito antes de incorporarlo.

---

## 7. Estructura de cada requisito

Para proyectos estándar, avanzados o críticos, utiliza esta estructura cuando aporte valor.

### RF-XXX — Nombre del requisito

**Estado:** Propuesto / Aprobado / Pendiente / Obsoleto

**Capacidad de origen:** ALC-XXX

**Objetivo relacionado:** OBJ-XXX

**Actores:** [Actores correspondientes]

**Descripción:**

El sistema deberá [...]

**Precondiciones:**

Condiciones necesarias antes de ejecutar el comportamiento.

**Disparador:**

Evento o acción que inicia el comportamiento.

**Comportamiento esperado:**

Resultado observable que debe producir el sistema.

**Reglas de negocio:**

Reglas aplicables al comportamiento.

**Escenarios alternativos:**

Variaciones relevantes del flujo principal.

**Errores y casos límite:**

Situaciones excepcionales que deben contemplarse.

**Postcondiciones:**

Estado observable después de completar la operación.

**Dependencias:**

Otros requisitos necesarios, si existen.

**Decisiones pendientes:**

Aspectos todavía no confirmados.

**Verificación preliminar:**

Descripción breve de cómo podría comprobarse el cumplimiento.

No rellenes campos con información inventada.

Para proyectos ligeros, puedes utilizar una versión simplificada con identificador, descripción, origen, estado y verificación preliminar.

---

## 8. Identificación de actores y permisos

Para cada comportamiento, determina:

- Quién puede iniciarlo.
    
- Quién puede consultar el resultado.
    
- Quién puede modificar información.
    
- Quién puede eliminar información.
    
- Si existen restricciones por rol.
    
- Si existen restricciones por propiedad de datos.
    
- Si existen restricciones organizativas.
    

No presupongas permisos.

No confundas autenticación con autorización.

### 8.1. Aplicaciones monousuario

No generes automáticamente requisitos de cuentas, roles o inicio de sesión.

Evalúa si el acceso está limitado por el entorno de ejecución.

### 8.2. Aplicaciones multiusuario

Investiga:

- Diferencias entre usuarios.
    
- Acceso a recursos compartidos.
    
- Propiedad de información.
    
- Separación entre organizaciones.
    
- Operaciones administrativas.
    
- Acciones restringidas.
    

Si una regla de permisos está pendiente, no inventes una política permisiva.

### 8.3. Seguridad funcional

Cuando una operación esté restringida, especifica su comportamiento funcional autorizado y no autorizado.

Las medidas técnicas concretas se desarrollarán en las fases de requisitos no funcionales, diseño y seguridad.

---

## 9. Reglas de negocio

Identifica las reglas que determinan el comportamiento del producto.

Ejemplos:

- Un identificador debe ser único.
    
- Una tarea completada no puede volver a asignarse sin reabrirla.
    
- Una reserva no puede confirmarse si el recurso no está disponible.
    
- Un usuario solo puede modificar recursos para los que tiene autorización.
    

Cada regla debe:

1. Tener una descripción clara.
    
2. Estar relacionada con requisitos concretos.
    
3. Tener un origen identificable.
    
4. Ser verificable.
    
5. Estar confirmada o marcada como propuesta.
    

Utiliza identificadores cuando sea útil:

- RN-001
    
- RN-002
    

No inventes políticas empresariales.

Si una regla depende de decisiones organizativas, solicita confirmación.

---

## 10. Escenarios funcionales

Para cada capacidad relevante, identifica escenarios de comportamiento.

### 10.1. Escenario principal

Describe el flujo habitual cuando todas las condiciones necesarias se cumplen.

Incluye:

1. Actor.
    
2. Situación inicial.
    
3. Acción.
    
4. Respuesta del sistema.
    
5. Resultado final.
    

### 10.2. Escenarios alternativos

Identifica caminos válidos diferentes del escenario principal.

Ejemplos:

- Usuario cancela la operación.
    
- Se proporciona información opcional.
    
- Se utiliza un método alternativo de entrada.
    
- El recurso ya existe.
    
- El proceso requiere confirmación.
    

No presupongas que todos los escenarios alternativos son errores.

### 10.3. Escenarios de error

Identifica situaciones en las que el sistema no puede completar la operación.

Ejemplos:

- Información obligatoria ausente.
    
- Datos inválidos.
    
- Recurso inexistente.
    
- Permiso insuficiente.
    
- Conflicto con el estado actual.
    
- Dependencia externa no disponible.
    

Especifica el resultado observable esperado.

No inventes mensajes literales de error si no son necesarios.

---

## 11. Análisis de casos límite

Para cada requisito relevante, investiga los casos límite que puedan modificar su comportamiento.

Considera las siguientes categorías según corresponda.

### 11.1. Entradas

- Valores vacíos.
    
- Valores nulos.
    
- Formatos inválidos.
    
- Longitudes extremas.
    
- Caracteres especiales.
    
- Valores duplicados.
    
- Datos incompletos.
    
- Archivos vacíos o no admitidos.
    

No inventes límites numéricos.

### 11.2. Estados

- Recurso inexistente.
    
- Recurso eliminado.
    
- Recurso archivado.
    
- Operación ya completada.
    
- Estado incompatible.
    
- Información desactualizada.
    

### 11.3. Permisos

- Usuario no autenticado.
    
- Usuario sin autorización.
    
- Recurso perteneciente a otro usuario.
    
- Acceso entre organizaciones.
    
- Permiso revocado durante una operación.
    

Aplica únicamente los escenarios relevantes para el proyecto.

### 11.4. Concurrencia

Cuando existan múltiples usuarios o procesos:

- Ediciones simultáneas.
    
- Operaciones duplicadas.
    
- Conflictos de actualización.
    
- Solicitudes repetidas.
    
- Cambios concurrentes de estado.
    

No definas mecanismos técnicos de concurrencia todavía.

### 11.5. Dependencias externas

- Servicio no disponible.
    
- Respuesta incompleta.
    
- Tiempo de espera agotado.
    
- Respuesta inesperada.
    
- Operación externa parcialmente completada.
    

### 11.6. Operaciones destructivas

Cuando exista modificación o eliminación de información:

- Cancelación.
    
- Confirmación.
    
- Recuperación, si corresponde.
    
- Consecuencias de una operación fallida.
    
- Comportamiento ante ejecución repetida.
    

No presupongas que debe existir papelera o restauración si no está contemplado en el alcance.

### 11.7. Selección proporcional

No generes casos límite irrelevantes únicamente para completar una lista.

Prioriza aquellos que:

- Puedan producir errores importantes.
    
- Afecten a datos.
    
- Comprometan permisos.
    
- Modifiquen resultados.
    
- Sean frecuentes o plausibles.
    
- Resulten difíciles de corregir posteriormente.
    

---

## 12. Requisitos funcionales relacionados con IA

Aplica esta sección únicamente cuando existan capacidades de IA dentro del alcance aprobado.

### 12.1. Comportamiento observable

Especifica qué podrá solicitar el usuario y qué resultado funcional deberá ofrecer el sistema.

Ejemplo:

"El sistema deberá permitir que un usuario consulte el contenido de los documentos a los que tenga acceso".

No definas todavía si se utilizará RAG, un modelo concreto o una base de datos vectorial.

### 12.2. Resultados inciertos

Distingue entre:

- Comportamiento determinista del software.
    
- Resultado probabilístico del modelo.
    

No prometas que un modelo generativo producirá siempre una respuesta correcta.

Define comportamientos funcionales ante incertidumbre, cuando corresponda.

Por ejemplo:

"El sistema deberá informar al usuario cuando no pueda proporcionar una respuesta suficientemente fundamentada".

Los umbrales y métodos de evaluación se definirán posteriormente.

### 12.3. Acciones ejecutadas por agentes

Si la IA puede ejecutar acciones:

- Identifica las acciones permitidas.
    
- Identifica las acciones prohibidas.
    
- Determina qué operaciones requieren confirmación.
    
- Identifica qué actores pueden autorizarlas.
    
- Define qué debe ocurrir ante una denegación.
    
- Considera resultados parciales o fallidos.
    

No otorgues permisos implícitos a un agente.

### 12.4. Datos y privacidad

Identifica qué categorías de datos puede utilizar cada capacidad de IA.

No presupongas autorización para acceder a toda la información disponible.

### 12.5. Fallos funcionales

Considera:

- Ausencia de respuesta.
    
- Respuesta no utilizable.
    
- Información insuficiente.
    
- Herramienta externa fallida.
    
- Solicitud fuera del alcance.
    
- Acción no autorizada.
    
- Resultado que requiere revisión humana.
    

Las métricas de calidad, latencia, costes y seguridad se definirán en las fases correspondientes.

---

## 13. Trazabilidad obligatoria

Cada requisito aprobado debe estar vinculado a una capacidad del alcance.

Cuando corresponda, también debe vincularse a uno o varios objetivos.

### 13.1. Relación entre documentos

La cadena de trazabilidad será:

`OBJ-XXX → ALC-XXX → RF-XXX → CA-XXX → TEST-XXX`

Donde:

- `OBJ`: objetivo del producto.
    
- `ALC`: capacidad incluida en el alcance.
    
- `RF`: requisito funcional.
    
- `CA`: criterio de aceptación.
    
- `TEST`: prueba de validación.
    

En esta fase solo debes consolidar las relaciones hasta `RF`.

No inventes identificadores de criterios de aceptación o pruebas que todavía no existan.

### 13.2. Matriz de trazabilidad

Genera una matriz con:

- Objetivo.
    
- Capacidad.
    
- Requisito.
    
- Estado.
    
- Observaciones.
    

### 13.3. Cobertura del alcance

Comprueba que cada capacidad aprobada tenga requisitos suficientes o una justificación documentada de por qué permanece pendiente.

No generes requisitos para capacidades excluidas.

### 13.4. Requisitos sin origen

Si aparece un requisito sin capacidad de origen:

1. Identifica su procedencia.
    
2. Comprueba si pertenece al alcance.
    
3. Si no pertenece, propón un cambio de alcance.
    
4. Solicita aprobación.
    
5. No lo incorpores como requisito aprobado hasta resolverlo.
    

### 13.5. Estabilidad de identificadores

Mantén los identificadores existentes entre revisiones.

No renumeres todos los requisitos por motivos estéticos.

Marca los requisitos retirados como obsoletos y conserva su historial cuando sea necesario.

---

## 14. Detección de problemas en la especificación

Antes de presentar los requisitos, revisa:

### 14.1. Ambigüedad

¿Puede interpretarse el requisito de varias formas?

### 14.2. Duplicidad

¿Existen dos requisitos que describen la misma obligación?

### 14.3. Contradicción

¿Existen requisitos incompatibles?

### 14.4. Falta de información

¿Faltan condiciones necesarias para comprender el comportamiento?

### 14.5. Falta de trazabilidad

¿Existe un requisito sin relación con el alcance?

### 14.6. Falta de verificabilidad

¿Es imposible comprobar objetivamente si se cumple?

### 14.7. Mezcla de responsabilidades

¿El requisito contiene varias obligaciones independientes?

### 14.8. Solución técnica prematura

¿Describe una implementación en lugar de un comportamiento?

### 14.9. Alcance no autorizado

¿Introduce una funcionalidad que no fue aprobada?

Cuando detectes un problema, propón una corrección y solicita confirmación si afecta al significado.

---

## 15. Gestión de dependencias funcionales

Identifica dependencias entre requisitos.

Ejemplo:

RF-008 puede depender de RF-003 si necesita que exista previamente un recurso.

Distingue:

- Dependencia funcional obligatoria.
    
- Relación informativa.
    
- Restricción de negocio.
    
- Dependencia pendiente de confirmar.
    

No utilices estas dependencias para definir todavía el orden definitivo de implementación.

Ese trabajo pertenece a la planificación.

Evita dependencias circulares injustificadas.

---

## 16. Gestión de cambios

Cuando se solicite modificar un requisito:

1. Identifica su ID.
    
2. Describe el cambio.
    
3. Comprueba su origen en `scope.md`.
    
4. Analiza requisitos relacionados.
    
5. Identifica reglas de negocio afectadas.
    
6. Revisa escenarios y casos límite.
    
7. Identifica consecuencias para criterios de aceptación y pruebas existentes, si los hubiera.
    
8. Solicita aprobación cuando corresponda.
    
9. Actualiza la documentación.
    

No modifiques silenciosamente requisitos aprobados.

Si el cambio afecta al alcance, remítelo primero a la revisión de `scope.md`.

Si afecta a la visión del producto, identifica también la necesidad de revisar `vision.md`.

---

## 17. Entregable: `functional-requirements.md`

Cuando exista información suficiente, genera un documento Markdown compatible con Obsidian siguiendo esta estructura.

# Especificación de requisitos funcionales

**Proyecto:** [Nombre]  
**Versión:** 0.1  
**Estado:** Borrador / Pendiente de aprobación / Aprobado  
**Fecha:** [Fecha conocida o pendiente]

**Documentos de referencia:**

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    

## 1. Propósito

Explicar qué comportamientos funcionales se especifican y para qué se utilizará el documento.

## 2. Alcance de la especificación

Identificar las capacidades aprobadas cubiertas.

Indicar explícitamente las capacidades pendientes de especificación.

No incorporar capacidades excluidas.

## 3. Actores

|ID|Actor|Descripción|Capacidades relacionadas|
|---|---|---|---|
|ACT-001||||

Mantener consistencia con los actores identificados previamente.

## 4. Catálogo de requisitos

|ID|Requisito|Capacidad|Estado|
|---|---|---|---|
|RF-001||ALC-001||

## 5. Especificación detallada

### RF-001 — [Nombre]

**Estado:** Propuesto / Aprobado / Pendiente

**Capacidad:** ALC-XXX

**Objetivo:** OBJ-XXX

**Actores:** [...]

**Descripción:**

El sistema deberá [...]

**Precondiciones:**

- ...
    

**Disparador:**

- ...
    

**Comportamiento esperado:**

- ...
    

**Reglas de negocio:**

- ...
    

**Escenarios alternativos:**

- ...
    

**Errores y casos límite:**

- ...
    

**Postcondiciones:**

- ...
    

**Dependencias:**

- ...
    

**Decisiones pendientes:**

- ...
    

**Verificación preliminar:**

- ...
    

Repetir para los requisitos necesarios.

Omitir campos no aplicables cuando no aporten valor, especialmente en proyectos ligeros.

## 6. Reglas de negocio

|ID|Regla|Requisitos relacionados|Estado|
|---|---|---|---|
|RN-001||RF-001||

## 7. Escenarios funcionales relevantes

### ESC-F001 — [Nombre]

**Actor:**  
**Precondición:**  
**Acción:**  
**Resultado esperado:**  
**Requisitos relacionados:**

Incluir escenarios principales y alternativos cuando aporten claridad.

## 8. Casos límite y errores

|ID|Situación|Comportamiento esperado|RF relacionado|Estado|
|---|---|---|---|---|
|CL-001|||RF-001||

No inventar comportamientos no aprobados.

## 9. Matriz de trazabilidad

|Objetivo|Capacidad|Requisito|Estado|
|---|---|---|---|
|OBJ-001|ALC-001|RF-001||

## 10. Cobertura del alcance

|Capacidad|Estado de especificación|Observaciones|
|---|---|---|
|ALC-001|Completa / Parcial / Pendiente||

La cobertura completa significa que los requisitos conocidos están especificados, no que el software esté implementado.

## 11. Dependencias funcionales

|Requisito|Depende de|Motivo|
|---|---|---|
|RF-002|RF-001||

## 12. Contradicciones y problemas detectados

- Ambigüedades.
    
- Duplicidades.
    
- Conflictos.
    
- Requisitos sin origen.
    
- Cambios de alcance propuestos.
    

Indicar «Ninguno identificado» cuando corresponda, sin afirmar que la especificación está libre de defectos.

## 13. Decisiones pendientes

|ID|Decisión|Requisitos afectados|Importancia|
|---|---|---|---|
|DEC-001||||

## 14. Supuestos

|ID|Supuesto|Requisitos afectados|Consecuencia|
|---|---|---|---|
|SUP-001||||

## 15. Revisión de coherencia

### Coherencia con `scope.md`

[Resultado]

### Coherencia con `vision.md`

[Resultado]

### Coherencia con `project-profile.md`

[Resultado]

### Cambios propuestos

[Lista o «Ninguno»]

## 16. Estado de aprobación

**Estado:** Pendiente de aprobación

**Responsable:** [Pendiente]

**Fecha:** [Pendiente]

**Observaciones:** [Pendiente]

## 17. Próximo paso

**Instrucción:**

`02 - Especificaciones/04 - Requisitos no funcionales.md`

**Objetivo:**

Definir las condiciones de calidad, seguridad, rendimiento, disponibilidad, mantenibilidad y otras propiedades que debe cumplir el sistema.

---

## 18. Validación de requisitos

Antes de presentar la especificación, comprueba:

- ¿Todos los requisitos tienen identificadores únicos?
    
- ¿Cada requisito describe un comportamiento observable?
    
- ¿Los requisitos son suficientemente atómicos?
    
- ¿Se ha evitado lenguaje ambiguo?
    
- ¿Se han identificado los actores relevantes?
    
- ¿Las precondiciones importantes están documentadas?
    
- ¿Los resultados esperados son comprensibles?
    
- ¿Se han identificado las reglas de negocio?
    
- ¿Se han considerado escenarios alternativos?
    
- ¿Se han analizado casos límite relevantes?
    
- ¿Los permisos funcionales están suficientemente definidos?
    
- ¿Cada requisito tiene un origen trazable?
    
- ¿Existen requisitos fuera del alcance?
    
- ¿Se han detectado duplicidades y contradicciones?
    
- ¿Se han evitado decisiones técnicas prematuras?
    
- ¿Se han documentado las incertidumbres?
    
- ¿La especificación permite preparar criterios de aceptación?
    

Si detectas deficiencias, corrígelas cuando sea posible sin alterar decisiones aprobadas.

Si una corrección requiere decidir un comportamiento, consulta antes de consolidarlo.

---

## 19. Condiciones de finalización

La instrucción estará completada cuando:

1. Las capacidades aprobadas estén suficientemente especificadas.
    
2. Los requisitos tengan identificadores estables.
    
3. Exista trazabilidad con el alcance.
    
4. Los comportamientos principales estén definidos.
    
5. Las reglas de negocio relevantes estén documentadas.
    
6. Los errores y casos límite importantes estén identificados.
    
7. Las contradicciones bloqueantes estén resueltas.
    
8. Las decisiones pendientes estén registradas.
    
9. Se haya generado `functional-requirements.md`.
    
10. Yo haya revisado y aprobado la especificación.
    

No declares aprobado un requisito únicamente por haberlo redactado.

No avances automáticamente a la siguiente fase.

---

## 20. Comportamiento al finalizar

Presenta un resumen breve con:

**Requisitos definidos:** número y capacidades cubiertas.

**Cobertura:** capacidades completas, parciales y pendientes.

**Problemas detectados:** contradicciones, ambigüedades o posibles cambios de alcance.

**Decisiones pendientes:** cuestiones que requieren mi intervención.

**Entregable:** `functional-requirements.md`.

**Siguiente paso:** `04 - Requisitos no funcionales.md`.

Solicita mi aprobación antes de continuar.

---

## 21. Principio rector

**La IA no debe decidir qué funcionalidades necesita el producto. Debe ayudarme a convertir las funcionalidades aprobadas en comportamientos precisos y verificables.**

Un requisito bien escrito debe poder comprenderse, implementarse y comprobarse sin depender de interpretaciones improvisadas.

La calidad de la especificación es más importante que la cantidad de requisitos generados.

---

## 22. Instrucción de inicio

Si dispones de los documentos de entrada:

1. Analiza `project-profile.md`, `vision.md` y `scope.md`.
    
2. Identifica las capacidades aprobadas.
    
3. Presenta un resumen breve.
    
4. Selecciona la primera capacidad pendiente de especificación.
    
5. Formula las preguntas necesarias para definir su comportamiento.
    

Si faltan documentos, solicita la información necesaria.

No generes requisitos definitivos sin comprender el alcance aprobado.