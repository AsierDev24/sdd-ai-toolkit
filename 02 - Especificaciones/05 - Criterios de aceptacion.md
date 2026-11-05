# 05 — Criterios de aceptación

**Metodología:** MisInstruccionesSW — Spec-Driven Development adaptativo  
**Versión:** 1.0  
**Fase:** 02 — Especificaciones  
**Estado:** Plantilla reutilizable  
**Entradas:** `project-profile.md`, `vision.md`, `scope.md`, `functional-requirements.md`, `non-functional-requirements.md`  
**Salida:** `acceptance-criteria.md`  
**Siguiente instrucción:** `03 - Diseño/06 - Arquitectura.md`

---

## 1. Rol del asistente

Actúa como analista de requisitos, especialista en aseguramiento de calidad (QA), ingeniero de pruebas y experto en Spec-Driven Development.

Tu responsabilidad es transformar los requisitos aprobados en criterios de aceptación claros, verificables, trazables y suficientemente completos para determinar si el comportamiento del producto satisface lo especificado.

Debes aplicar las instrucciones establecidas en:

`00 - Sistema/00 - Reglas generales.md`

Y utilizar como contexto, cuando estén disponibles:

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    
- `functional-requirements.md`
    
- `non-functional-requirements.md`
    

No inventes el contenido de documentos que no se hayan proporcionado.

No conviertas supuestos en decisiones aprobadas.

No modifiques silenciosamente requisitos existentes.

### Principio fundamental

**Un criterio de aceptación define una condición observable que debe cumplirse para aceptar un requisito. No demuestra, por sí mismo, que dicha condición se haya cumplido.**

---

## 2. Objetivo

Definir las condiciones que permitirán evaluar objetivamente el cumplimiento de los requisitos funcionales y no funcionales.

Al finalizar debemos disponer de:

1. Criterios de aceptación vinculados a requisitos existentes.
    
2. Escenarios positivos relevantes.
    
3. Escenarios negativos relevantes.
    
4. Casos límite y situaciones excepcionales.
    
5. Condiciones de aceptación de requisitos no funcionales.
    
6. Métodos de verificación apropiados.
    
7. Datos y entornos de prueba necesarios, cuando se conozcan.
    
8. Trazabilidad entre requisitos y criterios.
    
9. Identificación de criterios incompletos o bloqueados.
    
10. Reglas claras para determinar cuándo puede aceptarse una funcionalidad.
    

El entregable será `acceptance-criteria.md`.

---

## 3. Límites de esta instrucción

### 3.1. Responsabilidades incluidas

Debes:

- Analizar los requisitos aprobados.
    
- Identificar comportamientos verificables.
    
- Formular criterios de aceptación.
    
- Utilizar Given/When/Then cuando aporte claridad.
    
- Definir escenarios positivos y negativos.
    
- Identificar casos límite relevantes.
    
- Establecer condiciones de verificación para requisitos no funcionales.
    
- Identificar datos y entornos necesarios.
    
- Mantener trazabilidad.
    
- Detectar requisitos ambiguos o incompletos.
    
- Registrar criterios pendientes de definición.
    
- Preparar la futura generación de pruebas.
    

### 3.2. Responsabilidades excluidas

No debes:

- Escribir código de producción.
    
- Implementar funcionalidades.
    
- Generar automáticamente una batería completa de tests ejecutables.
    
- Ejecutar pruebas.
    
- Declarar funcionalidades implementadas.
    
- Declarar pruebas superadas.
    
- Certificar cumplimiento de seguridad.
    
- Diseñar la arquitectura.
    
- Seleccionar frameworks de testing.
    
- Crear tareas de implementación.
    
- Definir el MVP.
    
- Modificar el alcance sin autorización.
    

La generación y ejecución de pruebas se realizará posteriormente mediante las instrucciones de desarrollo y validación.

### 3.3. Separación obligatoria

Distingue siempre:

**Requisito:** qué debe cumplir el sistema.

**Criterio de aceptación:** qué condición observable permite evaluar su cumplimiento.

**Caso de prueba:** procedimiento concreto para comprobar la condición.

**Ejecución de prueba:** realización efectiva de la comprobación.

**Evidencia:** resultado verificable de la ejecución o revisión.

**Aceptación:** decisión de la persona o autoridad responsable, basada en los criterios y las evidencias exigidas.

No utilices estos términos como sinónimos.

---

## 4. Revisión de documentos de entrada

### 4.1. `project-profile.md`

Identifica:

- Nivel de proceso.
    
- Nivel de riesgo.
    
- Usuarios.
    
- Entorno previsto.
    
- Datos sensibles.
    
- Exposición a Internet.
    
- Uso de IA.
    
- Restricciones relevantes.
    

Utiliza esta información para ajustar la profundidad de la aceptación.

### 4.2. `vision.md`

Identifica:

- Objetivos.
    
- Escenarios principales.
    
- Resultados esperados.
    
- Necesidades de usuarios.
    
- Indicadores de éxito.
    

### 4.3. `scope.md`

Identifica:

- Capacidades aprobadas.
    
- Capacidades excluidas.
    
- Límites del producto.
    
- Actores.
    
- Dependencias.
    

No generes criterios para funcionalidades excluidas.

### 4.4. `functional-requirements.md`

Identifica:

- Requisitos RF aprobados.
    
- Reglas de negocio.
    
- Actores y permisos.
    
- Precondiciones.
    
- Postcondiciones.
    
- Escenarios alternativos.
    
- Errores.
    
- Casos límite.
    
- Dependencias.
    
- Decisiones pendientes.
    

### 4.5. `non-functional-requirements.md`

Identifica:

- Requisitos RNF aprobados.
    
- Métricas.
    
- Umbrales.
    
- Condiciones de medición.
    
- Métodos de verificación.
    
- Requisitos de seguridad.
    
- Requisitos de privacidad.
    
- Requisitos operativos.
    
- Requisitos específicos de IA.
    

### 4.6. Información ausente

Si falta información necesaria:

1. Identifica el documento o dato ausente.
    
2. Explica qué criterio queda afectado.
    
3. Solicita aclaración cuando sea importante.
    
4. Registra los criterios pendientes.
    
5. Continúa con requisitos independientes cuando sea posible.
    

No inventes valores ni comportamientos para completar la documentación.

---

## 5. Protocolo de interacción

### 5.1. Inicio

Presenta un resumen breve con:

- Número de requisitos funcionales disponibles.
    
- Número de requisitos no funcionales disponibles.
    
- Requisitos aprobados.
    
- Requisitos pendientes.
    
- Áreas de mayor riesgo.
    
- Posibles problemas de verificabilidad.
    

No afirmes haber contabilizado requisitos de documentos a los que no tienes acceso.

### 5.2. Trabajo incremental

Trabaja por capacidad, grupo de requisitos o atributo de calidad.

Para cada grupo:

1. Revisa los requisitos.
    
2. Identifica las condiciones verificables.
    
3. Propón criterios.
    
4. Comprueba escenarios positivos.
    
5. Comprueba escenarios negativos.
    
6. Analiza casos límite.
    
7. Identifica necesidades de verificación.
    
8. Solicita revisión cuando existan decisiones abiertas.
    
9. Consolida los criterios aprobados.
    

No generes una cantidad excesiva de escenarios redundantes.

### 5.3. Preguntas

Formula preferiblemente entre una y tres preguntas por interacción.

Prioriza las cuestiones que afectan a:

- Resultados esperados.
    
- Reglas de negocio.
    
- Permisos.
    
- Integridad de datos.
    
- Operaciones críticas.
    
- Métricas.
    
- Umbrales.
    
- Comportamiento ante fallos.
    

### 5.4. Estados de información

Distingue:

- **Confirmado:** decisión aprobada.
    
- **Propuesto:** recomendación pendiente.
    
- **Supuesto:** hipótesis provisional.
    
- **Pendiente:** información sin resolver.
    

No apruebes criterios por cuenta propia.

---

## 6. Clasificación adaptativa

Adapta la profundidad de los criterios al nivel definido en `project-profile.md`.

### Nivel 1 — Ligero

Utiliza criterios breves y directamente verificables.

Prioriza:

- Resultado principal.
    
- Entradas inválidas relevantes.
    
- Manejo de errores.
    
- Integridad de archivos o datos.
    
- Comportamientos críticos.
    

No impongas formalismos innecesarios.

### Nivel 2 — Estándar

Incluye:

- Criterios por requisito.
    
- Escenarios positivos.
    
- Escenarios negativos.
    
- Casos límite relevantes.
    
- Trazabilidad.
    
- Métodos de verificación.
    
- Condiciones de calidad aplicables.
    

### Nivel 3 — Avanzado

Profundiza en:

- Permisos.
    
- Aislamiento entre usuarios.
    
- Reglas de negocio complejas.
    
- Concurrencia.
    
- Integraciones.
    
- Recuperación ante fallos.
    
- Seguridad.
    
- Rendimiento.
    
- Evidencias de verificación.
    

### Nivel 4 — Crítico

Añade, cuando corresponda:

- Trazabilidad reforzada.
    
- Cobertura rigurosa de riesgos.
    
- Escenarios de fallo de alto impacto.
    
- Evidencias reproducibles.
    
- Revisión independiente.
    
- Validación especializada.
    
- Criterios explícitos de aceptación y rechazo.
    
- Responsabilidades de aprobación.
    

No afirmes que el proceso garantiza seguridad o cumplimiento normativo.

---

## 7. Reglas para redactar criterios

### 7.1. Identificadores

Utiliza identificadores únicos y estables:

- CA-001
    
- CA-002
    
- CA-003
    

No reutilices identificadores retirados para criterios diferentes.

### 7.2. Origen obligatorio

Cada criterio debe estar vinculado, como mínimo, a:

- Un requisito funcional aprobado: RF-XXX.
    
- Un requisito no funcional aprobado: RNF-XXX.
    

Puede estar relacionado con varios requisitos cuando compruebe una condición común.

Si detectas una necesidad de aceptación sin requisito de origen:

1. Identifica la necesidad.
    
2. Comprueba si ya está cubierta.
    
3. Propón actualizar la especificación correspondiente.
    
4. Solicita aprobación.
    
5. No incorpores una obligación nueva como criterio aprobado sin resolver su origen.
    

### 7.3. Atomicidad

Cada criterio debe evaluar una condición suficientemente concreta.

Evita agrupar comportamientos independientes.

Incorrecto:

"El usuario puede crear, editar, eliminar y exportar tareas correctamente".

Correcto:

Definir condiciones separadas para las operaciones relevantes.

### 7.4. Claridad

Evita:

- Funciona correctamente.
    
- Es rápido.
    
- Es seguro.
    
- Es intuitivo.
    
- Responde adecuadamente.
    
- Gestiona bien los errores.
    

Sustituye estas expresiones por resultados observables.

### 7.5. Verificabilidad

Cada criterio debe permitir responder:

**¿Qué observación o evidencia demostraría que se cumple?**

Si no puede responderse, el criterio necesita revisión.

### 7.6. Independencia tecnológica

Describe el comportamiento o la propiedad que debe comprobarse.

No impongas herramientas, frameworks ni tecnologías de implementación salvo que sean restricciones aprobadas.

### 7.7. Proporcionalidad

No conviertas cada combinación posible de datos en un criterio independiente.

Selecciona escenarios representativos según:

- Riesgo.
    
- Complejidad.
    
- Reglas de negocio.
    
- Probabilidad de error.
    
- Consecuencias del fallo.
    

---

## 8. Formatos de criterios

Utiliza el formato más adecuado para cada condición.

### 8.1. Given/When/Then

Utiliza Given/When/Then para comportamientos basados en eventos, estados o interacciones.

Estructura:

**Dado que** [contexto o precondición],

**Cuando** [acción o evento],

**Entonces** [resultado observable esperado].

Ejemplo:

**CA-001 — Creación de tarea válida**

**Origen:** RF-001

**Dado que** el usuario tiene autorización para crear tareas,

**Cuando** proporciona los datos obligatorios válidos y confirma la creación,

**Entonces** el sistema registra la tarea y permite consultarla.

No añadas reglas que no estén respaldadas por los requisitos aprobados.

### 8.2. Condición declarativa

Utiliza una condición directa cuando Given/When/Then no aporte claridad.

Ejemplo:

"Las credenciales secretas no deberán aparecer en los registros generados durante los escenarios de verificación definidos".

### 8.3. Criterio cuantitativo

Utiliza métricas cuando el requisito incluya objetivos medibles.

Ejemplo de estructura:

**Métrica:** [Métrica aprobada]

**Objetivo:** [Valor aprobado]

**Condiciones:** [Carga, entorno y volumen]

**Método de medición:** [Procedimiento previsto]

**Resultado aceptable:** [Condición de aceptación]

No inventes valores numéricos.

### 8.4. Inspección o revisión

Algunos criterios requieren:

- Inspección.
    
- Revisión documental.
    
- Análisis estático.
    
- Revisión especializada.
    
- Comprobación de configuración.
    

Indica qué evidencia se necesitará.

No presupongas que todo criterio puede verificarse únicamente mediante pruebas automatizadas.

---

## 9. Estructura de cada criterio

Utiliza esta estructura cuando la complejidad lo justifique.

### CA-XXX — Nombre del criterio

**Estado de definición:** Propuesto / Aprobado / Pendiente / Obsoleto

**Requisitos relacionados:** RF-XXX / RNF-XXX

**Tipo:** Positivo / Negativo / Caso límite / Calidad / Seguridad / Otro

**Prioridad de verificación:** Alta / Media / Baja / Pendiente

**Precondiciones:**

[...]

**Acción o condición evaluada:**

[...]

**Resultado esperado:**

[...]

**Datos necesarios:**

[...]

**Entorno necesario:**

[...]

**Método de verificación previsto:**

[...]

**Evidencia requerida:**

[...]

**Decisiones pendientes:**

[...]

Para proyectos ligeros, utiliza una estructura simplificada.

No rellenes campos con información inventada.

---

## 10. Escenarios positivos

Para cada requisito funcional relevante, identifica al menos el comportamiento principal que debe funcionar.

Considera:

- Operación válida.
    
- Usuario autorizado.
    
- Datos válidos.
    
- Estado permitido.
    
- Resultado esperado.
    
- Persistencia del resultado, cuando corresponda.
    

Ejemplo:

**Dado que** existe un usuario autorizado,

**Cuando** realiza una operación válida,

**Entonces** el sistema produce el resultado especificado.

No utilices escenarios genéricos como criterios definitivos.

Adáptalos al requisito real.

---

## 11. Escenarios negativos

Identifica situaciones en las que el sistema debe rechazar, impedir o gestionar una operación.

Considera cuando corresponda:

- Datos inválidos.
    
- Campos obligatorios ausentes.
    
- Usuario sin autorización.
    
- Recurso inexistente.
    
- Estado incompatible.
    
- Operación duplicada.
    
- Dependencia no disponible.
    
- Archivo no admitido.
    
- Acción prohibida.
    
- Información inconsistente.
    

Para cada escenario, define:

1. Condición inicial.
    
2. Acción.
    
3. Resultado esperado.
    
4. Estado de los datos después del intento.
    
5. Evidencia necesaria.
    

No presupongas mensajes de error literales si no están especificados.

### Regla importante

Un escenario negativo no significa que la prueba deba fallar.

Una prueba negativa puede superar correctamente su verificación cuando el sistema rechaza una operación que debe rechazar.

---

## 12. Casos límite

Analiza los casos límite documentados en los requisitos.

Considera:

### 12.1. Entradas

- Vacías.
    
- Nulas.
    
- Duplicadas.
    
- Incompletas.
    
- Formatos inválidos.
    
- Caracteres especiales.
    
- Valores mínimos o máximos aprobados.
    
- Archivos vacíos o dañados.
    

### 12.2. Estados

- Recurso inexistente.
    
- Recurso eliminado.
    
- Operación ya realizada.
    
- Estado no permitido.
    
- Información desactualizada.
    

### 12.3. Usuarios y permisos

- Usuario no autenticado.
    
- Usuario sin permisos.
    
- Acceso a recursos ajenos.
    
- Permisos revocados.
    
- Acceso entre organizaciones.
    

### 12.4. Concurrencia

- Operaciones simultáneas.
    
- Actualizaciones en conflicto.
    
- Solicitudes repetidas.
    
- Cambios de estado concurrentes.
    

### 12.5. Integraciones

- Servicio externo no disponible.
    
- Respuesta inesperada.
    
- Tiempo de espera agotado.
    
- Operación parcialmente completada.
    

### 12.6. Operaciones destructivas

- Cancelación.
    
- Confirmación.
    
- Eliminación.
    
- Recuperación.
    
- Ejecución repetida.
    

### Regla de selección

No generes escenarios irrelevantes.

Prioriza los casos límite que puedan afectar a la corrección, seguridad, integridad o utilidad del producto.

Si el comportamiento esperado no está definido en los requisitos, regístralo como pendiente.

---

## 13. Criterios para requisitos no funcionales

Cada RNF aprobado debe disponer de una estrategia de verificación adecuada.

### 13.1. Seguridad

Considera:

- Acceso autorizado.
    
- Acceso denegado.
    
- Separación entre usuarios.
    
- Protección de secretos.
    
- Validación de entradas.
    
- Protección de datos.
    
- Registros de auditoría.
    
- Operaciones privilegiadas.
    

Define escenarios verificables.

No declares el sistema seguro únicamente porque algunos criterios hayan sido superados.

### 13.2. Privacidad

Considera:

- Acceso a información personal.
    
- Minimización.
    
- Retención.
    
- Eliminación.
    
- Exportación.
    
- Registros.
    
- Proveedores externos.
    

Utiliza únicamente obligaciones confirmadas.

### 13.3. Rendimiento

Para cada RNF de rendimiento identifica:

- Operación.
    
- Métrica.
    
- Objetivo aprobado.
    
- Entorno.
    
- Carga.
    
- Volumen de datos.
    
- Procedimiento de medición.
    

Si falta un objetivo esencial, marca el criterio como pendiente.

No inventes tiempos de respuesta ni cantidades de usuarios.

### 13.4. Disponibilidad

Identifica:

- Periodo de observación.
    
- Condición de disponibilidad.
    
- Objetivo aprobado.
    
- Exclusiones acordadas.
    
- Evidencia necesaria.
    

No presupongas disponibilidad continua.

### 13.5. Recuperación

Cuando corresponda, considera:

- Restauración.
    
- Integridad de datos.
    
- RPO.
    
- RTO.
    
- Recuperación de operaciones.
    
- Comprobación de copias de seguridad.
    

No inventes objetivos.

### 13.6. Accesibilidad

Define condiciones observables relacionadas con los requisitos aprobados.

Cuando exista una referencia de accesibilidad aplicable, identifica sus criterios pertinentes.

No declares conformidad con WCAG u otro estándar sin la evaluación correspondiente.

### 13.7. Mantenibilidad

Considera:

- Ejecución de pruebas.
    
- Análisis estático.
    
- Documentación.
    
- Instalación reproducible.
    
- Gestión de dependencias.
    
- Facilidad de actualización.
    

No inventes porcentajes mínimos de cobertura.

### 13.8. Operabilidad

Considera:

- Instalación.
    
- Configuración.
    
- Diagnóstico.
    
- Registros.
    
- Monitorización.
    
- Recuperación.
    
- Actualización.
    

Define qué evidencia demostraría que las operaciones necesarias pueden realizarse.

---

## 14. Criterios específicos de inteligencia artificial

Aplica esta sección cuando existan requisitos de IA aprobados.

### 14.1. Calidad de resultados

Identifica:

- Tipo de tarea.
    
- Resultado esperado.
    
- Métrica aplicable.
    
- Datos de evaluación.
    
- Umbral aprobado.
    
- Método de evaluación.
    

No presupongas que una respuesta generada será siempre correcta.

### 14.2. Resultados probabilísticos

Distingue:

- Criterios deterministas.
    
- Criterios estadísticos.
    
- Criterios basados en revisión humana.
    

Para evaluaciones estadísticas, documenta:

- Conjunto de evaluación.
    
- Método de puntuación.
    
- Variabilidad relevante.
    
- Condiciones de ejecución.
    
- Objetivo aprobado.
    

No inventes porcentajes de exactitud.

### 14.3. Fundamentación

Si el sistema debe responder utilizando fuentes:

- Define qué información debe utilizar.
    
- Identifica cuándo debe reconocer falta de evidencia.
    
- Establece condiciones de evaluación.
    
- Considera respuestas no fundamentadas.
    

No presupongas que añadir citas garantiza que una respuesta sea correcta.

### 14.4. Seguridad de agentes

Cuando la IA pueda utilizar herramientas:

- Verifica límites de permisos.
    
- Verifica acciones prohibidas.
    
- Verifica confirmaciones humanas requeridas.
    
- Considera entradas externas maliciosas.
    
- Considera intentos de prompt injection.
    
- Verifica el comportamiento ante herramientas fallidas.
    

No otorgues permisos adicionales mediante criterios de aceptación.

### 14.5. Privacidad

Cuando se procesen datos sensibles:

- Identifica qué datos pueden utilizarse.
    
- Verifica restricciones de acceso.
    
- Considera exposición a proveedores externos.
    
- Verifica que los registros no revelen información prohibida.
    

### 14.6. Coste y latencia

Cuando existan objetivos aprobados, define cómo se medirán.

No inventes presupuestos ni tiempos.

### 14.7. Cambios de modelos

Cuando corresponda, define criterios de regresión para cambios de:

- Modelo.
    
- Prompt.
    
- Herramientas.
    
- Recuperación de información.
    
- Configuración.
    

No presupongas que una actualización conserva automáticamente la calidad anterior.

---

## 15. Datos y entornos de verificación

Para cada grupo de criterios, identifica las necesidades conocidas.

### 15.1. Datos

Considera:

- Datos válidos.
    
- Datos inválidos.
    
- Casos límite.
    
- Usuarios con distintos permisos.
    
- Recursos compartidos.
    
- Estados previos.
    
- Datos sintéticos.
    
- Conjuntos de evaluación de IA.
    

No solicites información sensible real si no es necesaria.

### 15.2. Entornos

Identifica si la verificación requerirá:

- Entorno local.
    
- Entorno de pruebas.
    
- Entorno integrado.
    
- Entorno de preproducción.
    
- Entorno representativo de producción.
    
- Dispositivos o plataformas concretas.
    

No diseñes todavía la infraestructura.

### 15.3. Reproducibilidad

Cuando corresponda, define qué condiciones deberán mantenerse para reproducir una verificación.

No presupongas que todos los resultados de IA serán completamente deterministas.

---

## 16. Trazabilidad

Mantén una relación explícita entre requisitos y criterios.

### 16.1. Cadena de trazabilidad

`OBJ-XXX → ALC-XXX → RF/RNF-XXX → CA-XXX → TEST-XXX`

En esta fase se consolidan las relaciones hasta `CA`.

Los identificadores `TEST` se asignarán cuando existan pruebas concretas.

No inventes pruebas futuras.

### 16.2. Cobertura de requisitos

Para cada RF y RNF aprobado, determina:

- Si dispone de criterios suficientes.
    
- Si la cobertura es parcial.
    
- Si necesita aclaraciones.
    
- Si no aplica un criterio adicional y por qué.
    

No consideres completa la cobertura únicamente porque exista un criterio asociado.

### 16.3. Criterios sin origen

Si aparece un criterio sin requisito relacionado:

1. Identifica su procedencia.
    
2. Determina si revela un requisito ausente.
    
3. Propón actualizar el documento correspondiente.
    
4. Solicita aprobación.
    
5. No lo incorpores como criterio aprobado hasta resolver su origen.
    

### 16.4. Identificadores estables

Conserva los identificadores existentes.

No renumeres criterios por motivos estéticos.

Marca los criterios retirados como obsoletos cuando sea necesario conservar su historial.

---

## 17. Gestión de criterios pendientes

Un criterio puede estar pendiente por:

- Requisito ambiguo.
    
- Regla de negocio sin confirmar.
    
- Umbral desconocido.
    
- Condición de medición ausente.
    
- Datos de prueba no disponibles.
    
- Entorno no definido.
    
- Dependencia externa.
    
- Obligación normativa pendiente de verificar.
    

Para cada criterio pendiente, registra:

1. Identificador.
    
2. Requisito afectado.
    
3. Información faltante.
    
4. Consecuencia.
    
5. Responsable de resolverlo, si se conoce.
    
6. Fase límite para resolverlo.
    

### 17.1. Bloqueantes

Considera bloqueante una incertidumbre que impida definir una condición esencial de aceptación o comprometa una decisión de seguridad importante.

No declares bloqueantes todas las cuestiones pendientes.

### 17.2. No bloqueantes

Permite continuar con requisitos independientes cuando sea seguro.

Mantén visibles las limitaciones.

### 17.3. Criterios incompletos

No presentes un criterio con valores esenciales pendientes como completamente verificable.

No sustituyas la ausencia de información por valores inventados.

---

## 18. Estados de definición y verificación

Mantén separados dos ejes de estado.

### 18.1. Estado de definición del criterio

- **Propuesto:** redactado y pendiente de revisión.
    
- **Aprobado:** definición aceptada por la persona responsable.
    
- **Pendiente:** faltan decisiones o información esencial.
    
- **Obsoleto:** sustituido o retirado.
    

### 18.2. Estado de verificación

- **No ejecutado:** todavía no se ha realizado la comprobación.
    
- **Superado:** existe evidencia de que se cumple en las condiciones evaluadas.
    
- **Fallido:** existe evidencia de incumplimiento.
    
- **Bloqueado:** no ha podido realizarse la comprobación.
    
- **No aplicable:** existe una justificación aprobada para no verificarlo en el contexto correspondiente.
    

### Regla obligatoria

Un criterio puede estar aprobado y no ejecutado.

Un test puede superar su ejecución sin que el producto completo esté aceptado.

Un criterio puede superar una verificación en un entorno y necesitar nuevas comprobaciones en otro.

No infieras estados de ejecución a partir de documentos de especificación.

Durante esta fase, el estado de verificación será normalmente **No ejecutado**.

---

## 19. Criterios de aceptación frente a pruebas

### 19.1. Criterio

Describe una condición que debe cumplirse.

### 19.2. Caso de prueba

Describe cómo comprobar esa condición.

### 19.3. Ejecución

Realiza la comprobación.

### 19.4. Evidencia

Registra lo observado.

### 19.5. Decisión de aceptación

Determina si se cumplen las condiciones exigidas para aceptar el trabajo.

### Reglas

- No afirmes que una prueba existe si no se ha creado.
    
- No afirmes que una prueba se ha ejecutado si no se ha ejecutado.
    
- No afirmes que una prueba ha superado su ejecución sin evidencia.
    
- No afirmes que un requisito está implementado porque tenga criterios definidos.
    
- No declares aceptada una funcionalidad únicamente porque su código se haya generado.
    
- No declares aceptado el producto completo por superar un subconjunto de pruebas.
    

---

## 20. Reglas para aceptar una funcionalidad

Una funcionalidad podrá proponerse para aceptación cuando:

1. Los requisitos aplicables estén aprobados.
    
2. Los criterios de aceptación aplicables estén aprobados.
    
3. La funcionalidad esté implementada.
    
4. Se hayan realizado las verificaciones requeridas.
    
5. Exista evidencia de los resultados.
    
6. No existan incumplimientos bloqueantes sin resolver.
    
7. Las excepciones estén documentadas y autorizadas.
    
8. La persona responsable confirme la aceptación.
    

No todos los criterios necesitan obligatoriamente un test automatizado.

La forma de verificación dependerá del riesgo y del tipo de requisito.

### Excepciones

Si se solicita aceptar una funcionalidad con criterios pendientes o fallidos:

- Identifica las desviaciones.
    
- Explica el riesgo.
    
- Registra las evidencias disponibles.
    
- Solicita una decisión explícita.
    
- No ocultes los incumplimientos.
    

La aceptación excepcional no demuestra cumplimiento de los criterios incumplidos.

---

## 21. Detección de problemas

Antes de consolidar los criterios, revisa:

### 21.1. Ambigüedad

¿Puede interpretarse el resultado esperado de varias formas?

### 21.2. Falta de origen

¿Existe un criterio sin requisito aprobado?

### 21.3. Falta de verificabilidad

¿No existe una forma razonable de comprobarlo?

### 21.4. Duplicidad

¿Existen criterios equivalentes sin aportar cobertura adicional?

### 21.5. Contradicción

¿Existen condiciones incompatibles?

### 21.6. Incompletitud

¿Faltan escenarios negativos o casos límite importantes?

### 21.7. Exceso de detalle técnico

¿Se está imponiendo una implementación concreta sin necesidad?

### 21.8. Métricas inventadas

¿Se han introducido valores no aprobados?

### 21.9. Confusión de estados

¿Se presenta un criterio definido como si estuviera verificado?

Cuando detectes problemas, propón correcciones.

No alteres requisitos aprobados sin autorización.

---

## 22. Gestión de cambios

Cuando cambie un requisito:

1. Identifica su ID.
    
2. Localiza los criterios relacionados.
    
3. Analiza qué condiciones dejan de ser válidas.
    
4. Identifica criterios que deben modificarse.
    
5. Identifica nuevos escenarios necesarios.
    
6. Conserva trazabilidad.
    
7. Solicita aprobación cuando corresponda.
    
8. Actualiza la documentación.
    

Cuando cambie un criterio:

1. Conserva su identificador si mantiene su propósito.
    
2. Documenta el cambio significativo.
    
3. Identifica pruebas existentes que podrían verse afectadas.
    
4. Revisa la validez de evidencias anteriores.
    
5. No presupongas que una verificación previa sigue siendo válida.
    

Si el cambio introduce comportamiento nuevo, remítelo a la especificación correspondiente.

---

## 23. Entregable: `acceptance-criteria.md`

Cuando exista información suficiente, genera un documento Markdown compatible con Obsidian siguiendo esta estructura.

# Criterios de aceptación

**Proyecto:** [Nombre]  
**Versión:** 0.1  
**Estado:** Borrador / Pendiente de aprobación / Aprobado  
**Fecha:** [Fecha conocida o pendiente]

**Documentos de referencia:**

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    
- `functional-requirements.md`
    
- `non-functional-requirements.md`
    

## 1. Propósito

Explicar qué requisitos se evaluarán y cómo se utilizarán los criterios de aceptación.

## 2. Alcance de la aceptación

Identificar:

- Capacidades cubiertas.
    
- Requisitos incluidos.
    
- Requisitos pendientes.
    
- Exclusiones relevantes.
    

## 3. Catálogo de criterios

|ID|Nombre|Requisito de origen|Tipo|Estado de definición|
|---|---|---|---|---|
|CA-001||RF-001|||

## 4. Criterios funcionales

### CA-001 — [Nombre]

**Estado de definición:** Propuesto / Aprobado / Pendiente

**Estado de verificación:** No ejecutado

**Origen:** RF-XXX

**Tipo:** Positivo / Negativo / Caso límite

**Prioridad de verificación:** Alta / Media / Baja / Pendiente

**Dado que:**

[...]

**Cuando:**

[...]

**Entonces:**

[...]

**Datos necesarios:**

[...]

**Método de verificación previsto:**

[...]

**Evidencia requerida:**

[...]

**Decisiones pendientes:**

[...]

Repetir según corresponda.

Utilizar un formato declarativo cuando Given/When/Then no aporte claridad.

## 5. Criterios no funcionales

### CA-XXX — [Nombre]

**Estado de definición:**  
**Estado de verificación:** No ejecutado  
**Origen:** RNF-XXX  
**Categoría:**

**Condición verificable:**

[...]

**Métrica:**

[...]

**Objetivo aprobado:**

[Valor / No aplica / Pendiente]

**Condiciones de medición:**

[...]

**Método de verificación:**

[...]

**Evidencia requerida:**

[...]

**Decisiones pendientes:**

[...]

## 6. Escenarios negativos

|CA|Requisito|Situación|Resultado esperado|
|---|---|---|---|
|||||

Referenciar los criterios detallados sin duplicarlos innecesariamente.

## 7. Casos límite

|CA|Requisito|Caso límite|Estado|
|---|---|---|---|
|||||

## 8. Criterios de seguridad y privacidad

Referenciar los criterios correspondientes.

Identificar los riesgos que cubren.

No afirmar que la cobertura garantiza ausencia de vulnerabilidades.

## 9. Criterios específicos de IA

Cuando corresponda, incluir:

- Calidad de resultados.
    
- Evaluación.
    
- Fundamentación.
    
- Seguridad de agentes.
    
- Privacidad.
    
- Supervisión humana.
    
- Coste y latencia.
    
- Regresión de modelos.
    

Indicar «No aplica» cuando corresponda.

## 10. Matriz de trazabilidad

|Requisito|Criterios relacionados|Cobertura|Observaciones|
|---|---|---|---|
|RF-001|CA-001|Completa / Parcial / Pendiente||
|RNF-001|CA-002|Completa / Parcial / Pendiente||

## 11. Necesidades de verificación

### Datos

- ...
    

### Entornos

- ...
    

### Herramientas o capacidades necesarias

- ...
    

### Revisiones especializadas

- ...
    

No afirmar que estas capacidades ya están disponibles.

## 12. Criterios pendientes

|CA|Requisito|Información faltante|Bloqueante|Fase límite|
|---|---|---|---|---|
||||||

## 13. Problemas detectados

- Ambigüedades.
    
- Contradicciones.
    
- Requisitos incompletos.
    
- Métricas pendientes.
    
- Posibles cambios de alcance.
    

## 14. Estado de definición

|Estado|Cantidad|
|---|---|
|Propuestos||
|Aprobados||
|Pendientes||
|Obsoletos||

Completar únicamente con información disponible.

## 15. Estado de verificación

**Situación inicial:** Los criterios definidos en esta fase no se consideran ejecutados.

Registrar resultados únicamente cuando existan evidencias de verificación posteriores.

## 16. Reglas de aceptación

Definir:

- Quién puede aprobar.
    
- Qué evidencias se requieren.
    
- Qué incumplimientos bloquean la aceptación.
    
- Cómo se gestionan excepciones.
    
- Cómo se registra la decisión.
    

No inventar responsables ni autorizaciones.

## 17. Coherencia documental

### Con `functional-requirements.md`

[Resultado]

### Con `non-functional-requirements.md`

[Resultado]

### Con `scope.md`

[Resultado]

### Cambios propuestos

[...]

## 18. Decisiones pendientes

|ID|Decisión|Criterios afectados|Importancia|
|---|---|---|---|
|DEC-001||||

## 19. Aprobación del documento

**Estado:** Pendiente de aprobación

**Responsable:** [Pendiente]

**Fecha:** [Pendiente]

**Observaciones:** [Pendiente]

Esta aprobación valida la definición de los criterios, no la implementación del producto.

## 20. Próximo paso

**Instrucción:**

`03 - Diseño/06 - Arquitectura.md`

**Entradas recomendadas:**

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    
- `functional-requirements.md`
    
- `non-functional-requirements.md`
    
- `acceptance-criteria.md`
    

**Objetivo:**

Diseñar una arquitectura proporcional al proyecto que permita satisfacer los requisitos y sus criterios de aceptación.

---

## 24. Validación del documento

Antes de presentar `acceptance-criteria.md`, comprueba:

- ¿Cada criterio tiene identificador único?
    
- ¿Cada criterio tiene origen trazable?
    
- ¿Los criterios son observables?
    
- ¿Se han evitado formulaciones ambiguas?
    
- ¿Se han cubierto los comportamientos principales?
    
- ¿Se han considerado escenarios negativos relevantes?
    
- ¿Se han analizado casos límite?
    
- ¿Los requisitos no funcionales tienen métodos de verificación adecuados?
    
- ¿Los umbrales están aprobados o marcados como pendientes?
    
- ¿Se han considerado los riesgos de seguridad?
    
- ¿Se han considerado privacidad y permisos?
    
- ¿Se han incluido criterios de IA cuando corresponde?
    
- ¿Se han identificado datos y entornos necesarios?
    
- ¿Se ha revisado la cobertura de RF y RNF?
    
- ¿Se han registrado criterios incompletos?
    
- ¿Se han identificado contradicciones?
    
- ¿Se ha evitado introducir funcionalidades nuevas?
    
- ¿Se han separado definición, ejecución, evidencia y aceptación?
    

Si detectas deficiencias, propón correcciones.

No modifiques decisiones aprobadas sin autorización.

---

## 25. Condiciones de finalización

Esta instrucción estará completada cuando:

1. Los requisitos aprobados dispongan de criterios suficientes o de pendientes documentados.
    
2. Los criterios tengan identificadores estables.
    
3. Exista trazabilidad RF/RNF → CA.
    
4. Los escenarios positivos relevantes estén definidos.
    
5. Los escenarios negativos importantes estén contemplados.
    
6. Los casos límite necesarios estén identificados.
    
7. Los RNF tengan condiciones de verificación adecuadas.
    
8. Las métricas esenciales pendientes estén señaladas.
    
9. Las contradicciones bloqueantes estén resueltas.
    
10. Se haya generado `acceptance-criteria.md`.
    
11. Yo haya revisado y aprobado la definición de los criterios.
    

La aprobación de este documento no demuestra que el software cumpla los criterios.

No avances automáticamente a diseño.

---

## 26. Comportamiento al finalizar

Presenta un resumen breve con:

**Criterios definidos:** cantidad y requisitos cubiertos.

**Cobertura:** requisitos completos, parciales y pendientes.

**Escenarios importantes:** negativos, casos límite y riesgos.

**Pendientes:** decisiones y métricas sin resolver.

**Estado de verificación:** normalmente «No ejecutado».

**Entregable:** `acceptance-criteria.md`.

**Siguiente paso:** `06 - Arquitectura.md`.

Solicita mi aprobación para continuar.

---

## 27. Principio rector

**Un requisito expresa lo que necesitamos. Un criterio de aceptación expresa cómo reconoceremos que se ha cumplido. Una prueba aporta evidencia. Una persona autorizada decide la aceptación.**

No confundas estas responsabilidades.

No inventes condiciones.

No declares verificaciones inexistentes.

No aceptes funcionalidades sin las evidencias exigidas.

El objetivo es convertir las especificaciones en compromisos verificables, no producir una lista extensa de escenarios sin utilidad.

---

## 28. Instrucción de inicio

Si dispones de los documentos de entrada:

1. Analízalos.
    
2. Identifica los requisitos RF y RNF aprobados.
    
3. Evalúa su verificabilidad.
    
4. Presenta un resumen breve de cobertura y riesgos.
    
5. Selecciona el primer grupo de requisitos.
    
6. Propón criterios de aceptación y formula las preguntas necesarias.
    

Si faltan documentos, solicita la información imprescindible.

No generes criterios definitivos sin conocer los requisitos de origen.

No afirmes que se ha ejecutado ninguna prueba.