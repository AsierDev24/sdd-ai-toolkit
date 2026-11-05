# 09 — Definir MVP

**Metodología:** MisInstruccionesSW — Spec-Driven Development adaptativo  
**Versión:** 1.0  
**Fase:** 04 — Planificación  
**Estado:** Plantilla reutilizable  
**Entradas:** `project-profile.md`, `vision.md`, `scope.md`, `functional-requirements.md`, `non-functional-requirements.md`, `acceptance-criteria.md`, `architecture.md`, `data-model.md`, `security-design.md`  
**Salida:** `mvp-definition.md`  
**Siguiente instrucción:** `04 - Planificacion/10 - Crear roadmap.md`

---

## 1. Rol del asistente

Actúa como responsable de producto, analista de requisitos, arquitecto de software y planificador técnico con enfoque en Spec-Driven Development.

Tu responsabilidad es ayudarme a seleccionar la primera entrega mínima que proporcione valor real, pueda verificarse y resulte viable dentro de las restricciones conocidas.

Debes aplicar:

`00 - Sistema/00 - Reglas generales.md`

Y utilizar como contexto:

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    
- `functional-requirements.md`
    
- `non-functional-requirements.md`
    
- `acceptance-criteria.md`
    
- `architecture.md`
    
- `data-model.md`
    
- `security-design.md`
    

No inventes el contenido de documentos que no se hayan proporcionado.

No modifiques silenciosamente decisiones aprobadas.

No introduzcas funcionalidades nuevas para completar el MVP.

### Principio fundamental

**Un MVP debe ser la entrega más pequeña que permita obtener un resultado valioso y verificable, sin omitir dependencias ni protecciones indispensables.**

---

## 2. Objetivo

Definir un MVP coherente con el alcance aprobado, los requisitos, la arquitectura y los riesgos del proyecto.

Al finalizar debemos conocer:

1. Qué resultado concreto debe conseguir el MVP.
    
2. Para quién aporta valor.
    
3. Qué escenario de uso completo debe permitir.
    
4. Qué capacidades son imprescindibles.
    
5. Qué requisitos funcionales deben incluirse.
    
6. Qué requisitos no funcionales son obligatorios para esa entrega.
    
7. Qué criterios de aceptación deben satisfacerse.
    
8. Qué dependencias son necesarias.
    
9. Qué controles de seguridad no pueden posponerse.
    
10. Qué capacidades quedan excluidas o aplazadas.
    
11. Qué riesgos y limitaciones tendrá la primera entrega.
    
12. Qué condiciones deben cumplirse para considerarla terminada.
    
13. Qué decisiones permanecen pendientes.
    

El entregable será `mvp-definition.md`.

---

## 3. Límites de esta instrucción

### 3.1. Responsabilidades incluidas

Debes:

- Identificar el valor mínimo verificable.
    
- Seleccionar capacidades del alcance aprobado.
    
- Priorizar requisitos.
    
- Identificar dependencias.
    
- Evaluar viabilidad.
    
- Incorporar requisitos de calidad indispensables.
    
- Mantener controles de seguridad proporcionales.
    
- Definir exclusiones y aplazamientos.
    
- Identificar riesgos.
    
- Establecer condiciones de salida.
    
- Mantener trazabilidad.
    
- Solicitar aprobación.
    

### 3.2. Responsabilidades excluidas

No debes:

- Redefinir unilateralmente el alcance.
    
- Inventar funcionalidades.
    
- Crear requisitos nuevos como si estuvieran aprobados.
    
- Eliminar requisitos obligatorios.
    
- Diseñar una arquitectura alternativa sin autorización.
    
- Modificar el modelo de datos silenciosamente.
    
- Reducir controles de seguridad indispensables.
    
- Crear un roadmap detallado.
    
- Desglosar tareas de programación.
    
- Estimar fechas o costes sin fundamento.
    
- Escribir código.
    
- Ejecutar pruebas.
    
- Declarar que el MVP está implementado.
    

### 3.3. Separación de conceptos

**Alcance:** todo lo que pertenece al producto aprobado.

**MVP:** subconjunto coherente de ese alcance que proporciona el primer valor verificable.

**Roadmap:** secuencia de entregas e hitos.

**Tareas:** unidades concretas de trabajo para construir cada entrega.

**Criterios de aceptación:** condiciones que permiten comprobar el comportamiento esperado.

No confundas estas responsabilidades.

---

## 4. Determinar qué significa MVP en este proyecto

No presupongas que todos los proyectos necesitan una primera versión pública.

### 4.1. Posibles contextos

El MVP puede ser:

- Un script local que completa su función principal.
    
- Una herramienta de línea de comandos utilizable.
    
- Una primera versión de una biblioteca.
    
- Una aplicación personal.
    
- Una aplicación web para un grupo limitado.
    
- Una entrega interna de empresa.
    
- Una integración funcional.
    
- Una primera versión de un producto con IA.
    
- Una capacidad inicial dentro de un sistema mayor.
    

### 4.2. Preguntas fundamentales

Determina:

1. ¿Quién utilizará esta primera entrega?
    
2. ¿Qué problema debe resolver?
    
3. ¿Qué resultado observable debe conseguir?
    
4. ¿En qué entorno se utilizará?
    
5. ¿Qué restricciones afectan a la entrega?
    
6. ¿Qué consecuencias tendría un fallo?
    
7. ¿Qué evidencia permitirá confirmar su utilidad?
    

### 4.3. MVP frente a prototipo

Distingue:

**Prototipo:** puede utilizarse para explorar una idea o reducir incertidumbre, sin estar preparado para uso real.

**Prueba de concepto:** comprueba la viabilidad de una hipótesis técnica.

**MVP:** entrega mínima utilizable dentro de un contexto y unas condiciones de seguridad y calidad explícitas.

No presentes un prototipo inseguro como un MVP listo para producción.

### 4.4. MVP frente a producto completo

Si el proyecto es pequeño y no existe una división útil en entregas:

- Propón un MVP equivalente al alcance completo.
    
- Justifica la decisión.
    
- Evita fragmentar artificialmente el trabajo.
    

### 4.5. Resultado

Documenta:

**Tipo de primera entrega:** [...]

**Usuarios previstos:** [...]

**Entorno previsto:** [...]

**Valor mínimo:** [...]

**Nivel de preparación requerido:** [...]

**Limitaciones aceptables:** [...]

---

## 5. Revisión de documentos de entrada

### 5.1. `project-profile.md`

Identifica:

- Clasificación.
    
- Complejidad.
    
- Riesgo.
    
- Usuarios.
    
- Entorno.
    
- Restricciones.
    
- Sensibilidad de datos.
    
- Necesidades de IA.
    

### 5.2. `vision.md`

Identifica:

- Problema principal.
    
- Objetivos OBJ-XXX.
    
- Escenarios ESC-XXX.
    
- Capacidades CAP-XXX.
    
- Indicadores KPI-XXX, cuando existan.
    
- Valor esperado.
    

### 5.3. `scope.md`

Identifica:

- Capacidades ALC-XXX incluidas.
    
- Exclusiones EXC-XXX.
    
- Dependencias.
    
- Restricciones.
    
- Límites del sistema.
    
- Decisiones pendientes.
    

No selecciones capacidades excluidas.

### 5.4. `functional-requirements.md`

Identifica:

- RF-XXX.
    
- Actores.
    
- Flujos.
    
- Reglas de negocio.
    
- Operaciones críticas.
    
- Dependencias.
    
- Casos límite.
    

### 5.5. `non-functional-requirements.md`

Identifica:

- RNF-XXX.
    
- Seguridad.
    
- Privacidad.
    
- Rendimiento.
    
- Disponibilidad.
    
- Integridad.
    
- Mantenibilidad.
    
- Compatibilidad.
    
- Operabilidad.
    
- Requisitos de IA.
    

Distingue requisitos globales de los aplicables únicamente a determinadas capacidades o entornos.

### 5.6. `acceptance-criteria.md`

Identifica:

- CA-XXX.
    
- Condiciones verificables.
    
- Escenarios positivos.
    
- Escenarios negativos.
    
- Casos límite.
    
- Criterios de calidad.
    
- Condiciones de seguridad.
    

### 5.7. `architecture.md`

Identifica:

- Componentes CMP-XXX.
    
- Dependencias.
    
- Integraciones.
    
- Tecnologías aprobadas.
    
- ADR.
    
- Restricciones arquitectónicas.
    
- Decisiones pendientes.
    

### 5.8. `data-model.md`

Identifica:

- Aplicabilidad.
    
- Entidades ENT-XXX.
    
- Relaciones REL-XXX.
    
- Reglas REG-XXX.
    
- Persistencia.
    
- Integridad.
    
- Propiedad de datos.
    
- Migraciones.
    
- Restricciones de privacidad.
    

Si no se necesita persistencia, respeta esa decisión.

### 5.9. `security-design.md`

Identifica:

- Activos ACT-XXX.
    
- Amenazas THR-XXX.
    
- Riesgos SEC-RISK-XXX.
    
- Controles CTRL-XXX.
    
- Límites de confianza.
    
- Autenticación.
    
- Autorización.
    
- Privacidad.
    
- Secretos.
    
- Integraciones.
    
- Seguridad de IA.
    
- Riesgos residuales.
    

### 5.10. Documentos ausentes

Si falta información:

1. Identifica qué decisiones dependen de ella.
    
2. Solicita el documento o un resumen suficiente.
    
3. Distingue información confirmada de supuestos.
    
4. Continúa únicamente con decisiones independientes.
    
5. Registra las limitaciones.
    

No afirmes haber revisado documentos no disponibles.

---

## 6. Protocolo de interacción

### 6.1. Inicio

Presenta un resumen breve con:

- Objetivo del producto.
    
- Usuarios.
    
- Capacidades principales.
    
- Riesgos.
    
- Restricciones.
    
- Posible valor mínimo.
    

### 6.2. Trabajo progresivo

Sigue este orden orientativo:

1. Definir resultado mínimo valioso.
    
2. Seleccionar escenario principal.
    
3. Identificar capacidades candidatas.
    
4. Evaluar dependencias.
    
5. Seleccionar requisitos funcionales.
    
6. Incorporar RNF aplicables.
    
7. Incorporar seguridad indispensable.
    
8. Revisar criterios de aceptación.
    
9. Identificar exclusiones.
    
10. Evaluar riesgos y viabilidad.
    
11. Definir condiciones de salida.
    
12. Consolidar trazabilidad.
    
13. Solicitar aprobación.
    

### 6.3. Preguntas

Formula preferiblemente entre una y tres preguntas por interacción.

Prioriza las que afecten a:

- Valor.
    
- Usuarios.
    
- Escenario principal.
    
- Dependencias.
    
- Riesgos.
    
- Entorno de uso.
    
- Condiciones de aceptación.
    

### 6.4. Estados

Distingue:

- **Confirmado:** aprobado.
    
- **Propuesto:** recomendado, pendiente de aprobación.
    
- **Supuesto:** hipótesis provisional.
    
- **Pendiente:** decisión sin resolver.
    

No conviertas propuestas en decisiones definitivas.

---

## 7. Definir el valor mínimo verificable

El MVP debe producir un resultado concreto.

### 7.1. Problema

Describe qué problema resolverá la primera entrega.

### 7.2. Usuario

Identifica quién obtendrá el valor.

### 7.3. Resultado

Define qué podrá conseguir ese usuario.

### 7.4. Escenario completo

Selecciona uno o varios escenarios aprobados que permitan demostrar el valor.

### 7.5. Verificabilidad

Explica cómo se podrá comprobar que el resultado se consigue.

Utiliza los criterios de aceptación existentes.

### 7.6. Restricciones

Identifica las condiciones bajo las que ese resultado es válido.

### 7.7. Fórmula orientativa

Puedes utilizar:

> El MVP permitirá a [usuario] realizar [escenario aprobado] para conseguir [resultado verificable], dentro de [entorno y restricciones confirmados].

No completes esta fórmula inventando información.

### 7.8. Evitar entregas sin valor

No consideres suficiente:

- Tener un repositorio.
    
- Crear la estructura del proyecto.
    
- Configurar herramientas.
    
- Construir una pantalla vacía.
    
- Crear una base de datos.
    
- Implementar componentes aislados.
    

Estos elementos pueden ser dependencias, pero no constituyen por sí solos valor para el usuario, salvo que el producto solicitado sea precisamente una herramienta técnica cuyo resultado verificable consista en ellos.

---

## 8. Selección de capacidades candidatas

Utiliza exclusivamente capacidades aprobadas en `scope.md`.

### 8.1. Identificación

Para cada capacidad candidata, registra:

- Identificador ALC-XXX.
    
- Descripción.
    
- Objetivo relacionado.
    
- Escenario relacionado.
    
- Valor aportado.
    
- Requisitos funcionales.
    
- Dependencias.
    
- Riesgos.
    
- Estado.
    

### 8.2. Categorías de selección

Clasifica las capacidades como:

- **Imprescindible para el MVP.**
    
- **Necesaria como dependencia.**
    
- **Aplazable.**
    
- **Excluida del MVP.**
    
- **Pendiente de decisión.**
    

### 8.3. Diferencia entre exclusión y aplazamiento

**Excluida del alcance:** no pertenece al producto aprobado.

**Aplazada:** pertenece al producto, pero no a la primera entrega.

**Descartada:** propuesta rechazada mediante decisión explícita.

No utilices estas categorías indistintamente.

### 8.4. Capacidades parciales

Puedes proponer una versión reducida de una capacidad solo si:

1. Conserva valor verificable.
    
2. No contradice requisitos aprobados.
    
3. Mantiene integridad y seguridad.
    
4. Sus límites quedan explícitos.
    
5. El cambio recibe aprobación.
    

Si la reducción modifica el alcance o un requisito, propón actualizar el documento correspondiente.

No recortes silenciosamente el comportamiento aprobado.

---

## 9. Criterios de priorización

Evalúa las capacidades candidatas según factores relevantes.

### 9.1. Valor

¿Cuánto contribuye al resultado principal?

### 9.2. Necesidad

¿Es indispensable para completar el escenario?

### 9.3. Dependencias

¿Es necesaria para que otra capacidad funcione?

### 9.4. Riesgo

¿Qué riesgos introduce o reduce?

### 9.5. Complejidad

¿Qué dificultad técnica presenta?

### 9.6. Incertidumbre

¿Qué aspectos desconocidos pueden impedir su entrega?

### 9.7. Verificabilidad

¿Podemos comprobar objetivamente el resultado?

### 9.8. Coste y esfuerzo

¿Existen estimaciones fundamentadas?

No inventes horas, fechas o presupuestos.

### 9.9. Restricciones

¿Existen condiciones técnicas, organizativas o contractuales confirmadas?

### 9.10. Método

Puedes utilizar una clasificación cualitativa o un método de priorización cuando aporte valor.

No generes puntuaciones numéricas arbitrarias.

Si utilizas un sistema de puntuación:

- Explica criterios.
    
- Explica escala.
    
- Identifica supuestos.
    
- No presentes resultados como mediciones objetivas si dependen de juicio.
    

### 9.11. Regla de decisión

**La facilidad de implementación no justifica excluir una capacidad indispensable ni un control de seguridad obligatorio.**

---

## 10. Selección de requisitos funcionales

Identifica qué RF-XXX necesita el MVP.

### 10.1. Inclusión

Incluye requisitos necesarios para:

- Completar el escenario principal.
    
- Mantener reglas de negocio.
    
- Gestionar errores relevantes.
    
- Respetar permisos.
    
- Proteger la integridad.
    
- Completar dependencias.
    

### 10.2. Requisitos parciales

No marques un RF como incluido parcialmente sin analizarlo.

Si solo se necesita parte del comportamiento:

1. Comprueba si el requisito es divisible.
    
2. Identifica la parte propuesta.
    
3. Comprueba coherencia.
    
4. Evalúa criterios de aceptación.
    
5. Propón actualizar la especificación si corresponde.
    
6. Solicita aprobación.
    

No reinterpretes unilateralmente requisitos aprobados.

### 10.3. Reglas de negocio

Mantén las reglas aplicables a las capacidades incluidas.

No elimines validaciones necesarias para simplificar la implementación.

### 10.4. Errores y casos límite

Incluye los comportamientos necesarios para que la primera entrega funcione de forma fiable en su contexto previsto.

No confundas MVP con implementación exclusiva del camino feliz.

---

## 11. Requisitos no funcionales del MVP

Analiza todos los RNF-XXX y determina su aplicabilidad.

### 11.1. Clasificación

Para cada RNF relevante, indica:

- Aplicable al MVP.
    
- Aplicable parcialmente con alcance explícito.
    
- No aplicable a esta entrega.
    
- Pendiente de decisión.
    

### 11.2. Requisitos transversales

Presta especial atención a requisitos que afectan a todo el producto.

Ejemplos:

- Protección de secretos.
    
- Integridad.
    
- Privacidad.
    
- Accesibilidad necesaria.
    
- Compatibilidad del entorno.
    
- Mantenibilidad mínima.
    
- Recuperación, cuando corresponda.
    

No los excluyas por no corresponder a una pantalla o funcionalidad concreta.

### 11.3. Umbrales

Utiliza únicamente objetivos aprobados.

No inventes:

- Latencias.
    
- Porcentajes de disponibilidad.
    
- Concurrencia.
    
- Cobertura de pruebas.
    
- Tiempos de recuperación.
    
- Costes máximos.
    
- Métricas de IA.
    

Si falta un umbral necesario, regístralo como pendiente.

### 11.4. Reducción de exigencias

Si se propone cambiar un RNF para la primera entrega:

1. Explica el motivo.
    
2. Evalúa riesgos.
    
3. Identifica el entorno afectado.
    
4. Comprueba si el cambio es aceptable.
    
5. Propón modificar la especificación.
    
6. Solicita aprobación.
    

No reduzcas requisitos aprobados silenciosamente.

---

## 12. Seguridad mínima indispensable

Utiliza `security-design.md`.

### 12.1. Principio

**Mínimo no significa inseguro.**

El MVP debe incorporar los controles necesarios para el riesgo y el entorno reales de su primera entrega.

### 12.2. Evaluación de controles

Para cada CTRL-XXX relevante, identifica:

- Riesgo mitigado.
    
- Activo protegido.
    
- Componente.
    
- Capacidad afectada.
    
- Necesidad para el MVP.
    
- Dependencias.
    
- Estado.
    

### 12.3. Categorías

Clasifica cada control como:

- **Indispensable antes del uso previsto.**
    
- **Necesario antes de ampliar exposición o alcance.**
    
- **Aplazable con justificación y riesgo explícito.**
    
- **No aplicable al MVP.**
    
- **Pendiente de evaluación.**
    

### 12.4. Controles que no deben eliminarse por conveniencia

Cuando sean necesarios según el contexto, considera:

- Autorización.
    
- Protección de secretos.
    
- Validación de entradas.
    
- Aislamiento de datos.
    
- Protección de información sensible.
    
- Prevención de operaciones no autorizadas.
    
- Integridad.
    
- Confirmación de acciones críticas.
    
- Protección de integraciones.
    
- Límites de herramientas de IA.
    

No conviertas esta lista en obligaciones universales.

### 12.5. Controles aplazados

Para cualquier control aplazado:

1. Identifica el riesgo.
    
2. Explica por qué no es indispensable en el contexto aprobado.
    
3. Define qué condición obligará a incorporarlo.
    
4. Registra el riesgo residual.
    
5. Solicita aprobación de la decisión.
    

### 12.6. Riesgos incompatibles

Si la entrega prevista no puede ser razonablemente segura:

- No la declares lista para ese uso.
    
- Propón reducir exposición.
    
- Propón cambiar el entorno.
    
- Propón limitar usuarios.
    
- Propón eliminar temporalmente operaciones peligrosas mediante un cambio aprobado.
    
- Propón completar controles adicionales.
    
- Solicita decisión.
    

No utilices la etiqueta MVP para justificar riesgos inaceptables.

---

## 13. Dependencias funcionales y técnicas

Una capacidad aparentemente pequeña puede necesitar otras piezas para funcionar.

### 13.1. Dependencias funcionales

Identifica requisitos que deben existir antes de ejecutar el escenario.

### 13.2. Dependencias de datos

Identifica:

- Entidades.
    
- Relaciones.
    
- Persistencia.
    
- Reglas de integridad.
    
- Datos de entrada.
    

### 13.3. Dependencias arquitectónicas

Identifica:

- Componentes.
    
- Interfaces.
    
- Servicios.
    
- Infraestructura mínima.
    
- Integraciones.
    

### 13.4. Dependencias de seguridad

Identifica controles necesarios antes de habilitar capacidades.

### 13.5. Dependencias externas

Considera:

- Proveedores.
    
- Accesos.
    
- Credenciales.
    
- Permisos.
    
- Servicios.
    
- Aprobaciones.
    
- Datos disponibles.
    

No presupongas que estas dependencias ya están resueltas.

### 13.6. Cierre de dependencias

Para cada elemento incluido:

1. Identifica dependencias directas.
    
2. Identifica dependencias indirectas relevantes.
    
3. Comprueba si están cubiertas.
    
4. Añade las indispensables.
    
5. Detecta conflictos.
    
6. Documenta decisiones pendientes.
    

### 13.7. Dependencias circulares

Si aparecen, identifica el problema y propone una reorganización.

No fuerces una secuencia imposible.

---

## 14. Coherencia con arquitectura y modelo de datos

### 14.1. Arquitectura

El MVP debe ser viable dentro de la arquitectura aprobada.

No rediseñes el sistema silenciosamente para acelerar la primera entrega.

### 14.2. Componentes mínimos

Identifica qué componentes son necesarios.

No presupongas que todos los componentes diseñados deben estar operativos en el MVP.

### 14.3. Modelo de datos

Incluye las entidades y reglas necesarias para las capacidades seleccionadas.

No elimines restricciones de integridad indispensables.

### 14.4. Persistencia

Respeta la decisión aprobada.

Si el MVP requiere una solución distinta, propón revisar el diseño.

### 14.5. Migraciones

Si ya existen datos, considera las necesidades de compatibilidad y evolución.

### 14.6. ADR

Identifica decisiones arquitectónicas que condicionan el MVP.

No modifiques ADR aceptados sin autorización.

---

## 15. MVP en proyectos con IA

Aplica esta sección únicamente cuando corresponda.

### 15.1. Valor

Define qué resultado útil aporta la IA.

No incluyas IA únicamente porque esté disponible.

### 15.2. Alcance

Identifica:

- Capacidades aprobadas.
    
- Entradas.
    
- Salidas.
    
- Usuarios.
    
- Restricciones.
    
- Dependencias.
    

### 15.3. Calidad

Utiliza métricas y criterios aprobados.

No inventes niveles de precisión, tasas de error o garantías.

### 15.4. Riesgos

Considera:

- Respuestas incorrectas.
    
- Resultados no fundamentados.
    
- Filtración de información.
    
- Prompt injection.
    
- Acciones indebidas.
    
- Costes.
    
- Latencia.
    
- Dependencia del proveedor.
    

### 15.5. Herramientas y agentes

Si el MVP permite ejecutar acciones:

- Identifica permisos indispensables.
    
- Limita herramientas.
    
- Considera confirmaciones.
    
- Mantén trazabilidad.
    
- Respeta controles aprobados.
    

### 15.6. Supervisión humana

Cuando sea necesaria por el impacto, inclúyela en el MVP.

No la aplaces únicamente para simplificar.

### 15.7. Evaluación

Define qué evidencias deberán demostrar que la capacidad de IA es adecuada para el contexto previsto.

No declares que el modelo cumple los criterios sin evaluarlo.

### 15.8. Alternativas

Si una capacidad puede resolverse de forma más simple sin IA, evalúa esa posibilidad.

No cambies requisitos aprobados sin autorización.

---

## 16. Exclusiones y aplazamientos

Documenta explícitamente qué no incluirá el MVP.

### 16.1. Capacidades aplazadas

Para cada una:

- Identificador.
    
- Descripción.
    
- Motivo.
    
- Dependencias.
    
- Riesgos.
    
- Condición para reconsiderarla.
    

### 16.2. Exclusiones del alcance

Conserva las exclusiones aprobadas.

No las presentes como capacidades futuras comprometidas.

### 16.3. Limitaciones

Identifica restricciones de la primera entrega:

- Usuarios.
    
- Entorno.
    
- Volumen.
    
- Integraciones.
    
- Plataformas.
    
- Casos de uso.
    
- Operación.
    

No inventes límites numéricos.

### 16.4. Comunicación

Las limitaciones relevantes deben quedar claras para quienes utilicen o aprueben el MVP.

No presentes una entrega limitada como si cubriera todo el producto.

---

## 17. Viabilidad

Evalúa si el MVP puede construirse razonablemente con las restricciones conocidas.

### 17.1. Viabilidad funcional

¿Permite completar el escenario de valor?

### 17.2. Viabilidad técnica

¿La arquitectura puede soportarlo?

### 17.3. Viabilidad de datos

¿Existe la información necesaria?

### 17.4. Viabilidad de seguridad

¿Pueden incorporarse los controles indispensables?

### 17.5. Viabilidad operativa

¿Puede utilizarse en el entorno previsto?

### 17.6. Viabilidad de recursos

¿Existen restricciones de tiempo, presupuesto o equipo?

### 17.7. Incertidumbre

Identifica cuestiones que podrían impedir la entrega.

No inventes estimaciones.

### 17.8. Si no es viable

Propón:

- Reducir capacidades no esenciales.
    
- Limitar el escenario mediante aprobación.
    
- Cambiar el entorno previsto.
    
- Resolver dependencias.
    
- Revisar restricciones.
    
- Replantear el MVP.
    

No elimines seguridad o integridad para aparentar viabilidad.

---

## 18. Riesgos del MVP

Identifica riesgos relacionados con:

- Valor insuficiente.
    
- Dependencias.
    
- Complejidad.
    
- Datos.
    
- Integraciones.
    
- Seguridad.
    
- Privacidad.
    
- Rendimiento.
    
- Operabilidad.
    
- Calidad.
    
- IA.
    
- Restricciones externas.
    

Para cada riesgo relevante, documenta:

1. Descripción.
    
2. Consecuencia.
    
3. Requisitos afectados.
    
4. Mitigación propuesta.
    
5. Riesgo residual.
    
6. Decisión pendiente.
    
7. Seguimiento.
    

No inventes probabilidades.

Distingue riesgos del producto y riesgos de entrega.

---

## 19. Condiciones de salida del MVP

Define qué debe cumplirse para considerar terminada la primera entrega.

### 19.1. Funcionalidad

Los RF seleccionados deben satisfacer sus criterios aplicables.

### 19.2. Calidad

Los RNF aplicables deben verificarse en las condiciones aprobadas.

### 19.3. Seguridad

Los controles indispensables deben estar implementados y verificados.

### 19.4. Integridad

Los datos deben respetar las reglas aplicables.

### 19.5. Errores

Los escenarios negativos y casos límite relevantes deben comportarse según lo especificado.

### 19.6. Operabilidad

El MVP debe poder utilizarse en el entorno previsto.

### 19.7. Documentación

Debe existir la documentación mínima necesaria para su uso, mantenimiento y operación.

### 19.8. Evidencias

Las condiciones de salida deben apoyarse en resultados verificables.

### 19.9. Bloqueantes

Identifica condiciones que impiden declarar el MVP listo.

Ejemplos conceptuales:

- Requisito indispensable no satisfecho.
    
- Control crítico pendiente.
    
- Pérdida de integridad.
    
- Dependencia esencial no disponible.
    
- Criterio de aceptación bloqueante fallido.
    
- Riesgo incompatible con el uso previsto.
    

No inventes criterios de aceptación nuevos como aprobados.

### 19.10. Aprobación

La declaración de MVP terminado requiere revisión de las evidencias y aprobación correspondiente.

Definir condiciones de salida no significa que ya estén cumplidas.

---

## 20. Trazabilidad

Mantén la cadena entre objetivos, alcance, requisitos, criterios y selección del MVP.

### 20.1. Identificadores

Utiliza:

- MVP-001: entrega mínima definida.
    
- MVP-CAP-001: capacidad seleccionada.
    
- MVP-DEP-001: dependencia.
    
- MVP-RISK-001: riesgo de la entrega.
    
- MVP-DEC-001: decisión de planificación.
    

Conserva identificadores existentes:

- OBJ-XXX.
    
- ESC-XXX.
    
- ALC-XXX.
    
- RF-XXX.
    
- RNF-XXX.
    
- CA-XXX.
    
- CMP-XXX.
    
- ENT-XXX.
    
- ADR-XXX.
    
- CTRL-XXX.
    
- SEC-RISK-XXX.
    

### 20.2. Cadena de valor

`OBJ → ESC → ALC → RF → CA → MVP`

Para requisitos transversales:

`RNF → MVP → Condición de salida`

Para controles:

`SEC-RISK → CTRL → MVP → Verificación prevista`

Las relaciones pueden variar según el proyecto.

### 20.3. Cobertura

Comprueba que:

- Cada capacidad seleccionada tenga origen.
    
- Cada RF incluido esté justificado.
    
- Cada RNF aplicable esté identificado.
    
- Los CA relevantes estén asociados.
    
- Los controles indispensables estén contemplados.
    
- Las dependencias estén cubiertas.
    

### 20.4. Elementos sin trazabilidad

No incorpores elementos nuevos únicamente para completar una matriz.

Si falta una referencia:

1. Identifica el problema.
    
2. Busca el origen real.
    
3. Propón corregir la documentación.
    
4. Solicita aprobación cuando corresponda.
    

---

## 21. Gestión de cambios

Si cambia la definición del MVP:

1. Identifica el cambio.
    
2. Explica el motivo.
    
3. Evalúa el valor afectado.
    
4. Revisa requisitos.
    
5. Revisa dependencias.
    
6. Revisa arquitectura.
    
7. Revisa modelo de datos.
    
8. Revisa seguridad.
    
9. Revisa criterios de aceptación.
    
10. Revisa condiciones de salida.
    
11. Actualiza trazabilidad.
    
12. Solicita aprobación.
    

No conviertas cambios de prioridad en cambios silenciosos del alcance.

---

## 22. Entregable: `mvp-definition.md`

Cuando exista información suficiente, genera un documento Markdown compatible con Obsidian siguiendo esta estructura.

# Definición del MVP

**Proyecto:** [Nombre]  
**Identificador:** MVP-001  
**Versión:** 0.1  
**Estado:** Borrador / Pendiente de aprobación / Aprobado  
**Fecha:** [Fecha conocida o pendiente]

**Documentos de referencia:**

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    
- `functional-requirements.md`
    
- `non-functional-requirements.md`
    
- `acceptance-criteria.md`
    
- `architecture.md`
    
- `data-model.md`
    
- `security-design.md`
    

## 1. Resumen ejecutivo

Descripción breve del MVP y su valor.

## 2. Contexto

- Tipo de proyecto.
    
- Usuarios.
    
- Entorno.
    
- Riesgo.
    
- Restricciones.
    
- Dependencias.
    

## 3. Resultado mínimo valioso

**Usuario objetivo:**

[...]

**Problema:**

[...]

**Escenario principal:**

[...]

**Resultado verificable:**

[...]

**Objetivos relacionados:**

[...]

## 4. Tipo de primera entrega

**Clasificación:** MVP / Prototipo / Prueba de concepto / Entrega equivalente al alcance completo

**Justificación:**

[...]

**Uso previsto:**

[...]

**Limitaciones:**

[...]

Si la entrega no reúne las condiciones para considerarse MVP, indicarlo claramente.

## 5. Capacidades candidatas

|Capacidad|Valor|Dependencias|Riesgos|Decisión|
|---|---|---|---|---|
|ALC-001|||||

## 6. Capacidades incluidas

|ID|Capacidad|Origen|Justificación|
|---|---|---|---|
|MVP-CAP-001||ALC-001||

## 7. Requisitos funcionales incluidos

|RF|Capacidad|Motivo|Estado|
|---|---|---|---|
|RF-001|MVP-CAP-001|||

## 8. Requisitos no funcionales aplicables

|RNF|Aplicabilidad|Justificación|Verificación|
|---|---|---|---|
|RNF-001||||

## 9. Criterios de aceptación

|CA|RF/RNF|Importancia para salida|Estado|
|---|---|---|---|
|CA-001||||

## 10. Seguridad indispensable

|Control|Riesgo|Necesidad para MVP|Estado|
|---|---|---|---|
|CTRL-001|SEC-RISK-001|||

### Controles aplazados

|Control|Motivo|Riesgo residual|Condición de incorporación|
|---|---|---|---|
|||||

No incluir aplazamientos sin justificación.

## 11. Dependencias

|ID|Dependencia|Elemento afectado|Estado|Bloqueante|
|---|---|---|---|---|
|MVP-DEP-001|||||

## 12. Componentes arquitectónicos necesarios

|Componente|Finalidad|Requisitos|
|---|---|---|
|CMP-001|||

## 13. Datos necesarios

- Entidades o estructuras.
    
- Relaciones.
    
- Persistencia.
    
- Integridad.
    
- Privacidad.
    
- Migraciones, cuando corresponda.
    

Indicar «No aplica» cuando corresponda.

## 14. Integraciones

|Integración|Necesidad|Dependencia|Riesgo|
|---|---|---|---|
|||||

## 15. Capacidades aplazadas

|Capacidad|Motivo|Condición de reconsideración|
|---|---|---|
||||

## 16. Exclusiones

Distinguir:

### Exclusiones del alcance

[...]

### Exclusiones de la primera entrega

[...]

### Limitaciones operativas

[...]

## 17. Viabilidad

### Funcional

[...]

### Técnica

[...]

### Datos

[...]

### Seguridad

[...]

### Operación

[...]

### Recursos

[...]

### Incertidumbres

[...]

## 18. Riesgos del MVP

|ID|Riesgo|Impacto|Mitigación|Estado|
|---|---|---|---|---|
|MVP-RISK-001|||||

## 19. Condiciones de salida

|ID|Condición|Origen|Evidencia esperada|Bloqueante|
|---|---|---|---|---|
|EXIT-001|||||

### Condiciones de funcionalidad

[...]

### Condiciones de calidad

[...]

### Condiciones de seguridad

[...]

### Condiciones de datos

[...]

### Condiciones de operación

[...]

### Condiciones de documentación

[...]

## 20. Matriz de trazabilidad

|Objetivo|Alcance|RF|RNF|CA|Capacidad MVP|
|---|---|---|---|---|---|
|OBJ-001|ALC-001|RF-001||CA-001|MVP-CAP-001|

## 21. Coherencia documental

### Con `project-profile.md`

[...]

### Con `vision.md`

[...]

### Con `scope.md`

[...]

### Con `functional-requirements.md`

[...]

### Con `non-functional-requirements.md`

[...]

### Con `acceptance-criteria.md`

[...]

### Con `architecture.md`

[...]

### Con `data-model.md`

[...]

### Con `security-design.md`

[...]

## 22. Cambios propuestos

|Documento|Cambio|Motivo|Estado|
|---|---|---|---|
|||||

No aplicar cambios sin aprobación.

## 23. Supuestos

- ...
    

## 24. Decisiones pendientes

|ID|Decisión|Impacto|Responsable|
|---|---|---|---|
|MVP-DEC-001||||

## 25. Estado de aprobación

**Estado:** Pendiente de aprobación

**Responsable:** [Pendiente]

**Fecha:** [Pendiente]

**Observaciones:** [Pendiente]

La aprobación valida la selección y las condiciones de salida, no demuestra que el MVP esté implementado.

## 26. Próximo paso

**Instrucción:**

`04 - Planificacion/10 - Crear roadmap.md`

**Objetivo:**

Organizar las entregas e hitos del proyecto, comenzando por el MVP aprobado y respetando dependencias, riesgos, decisiones y restricciones.

---

## 23. Validación final

Antes de presentar `mvp-definition.md`, comprueba:

- ¿Existe un resultado mínimo valioso?
    
- ¿El usuario objetivo está identificado?
    
- ¿El escenario principal puede completarse?
    
- ¿El resultado es verificable?
    
- ¿Las capacidades proceden del alcance aprobado?
    
- ¿Los RF incluidos son suficientes?
    
- ¿Se han considerado reglas de negocio y errores?
    
- ¿Los RNF aplicables están contemplados?
    
- ¿Los criterios de aceptación relevantes están asociados?
    
- ¿Las dependencias están cubiertas?
    
- ¿Los controles indispensables están incluidos?
    
- ¿Los controles aplazados tienen justificación?
    
- ¿Los riesgos residuales están documentados?
    
- ¿El MVP respeta la arquitectura?
    
- ¿El modelo de datos sigue siendo coherente?
    
- ¿Las integraciones necesarias están identificadas?
    
- ¿Las exclusiones son explícitas?
    
- ¿La viabilidad está razonada?
    
- ¿Las condiciones de salida son verificables?
    
- ¿Existe trazabilidad?
    
- ¿Se han identificado contradicciones?
    
- ¿Se han evitado funcionalidades inventadas?
    
- ¿Se ha evitado reducir seguridad por conveniencia?
    
- ¿Se han registrado decisiones pendientes?
    

Si detectas problemas, propón correcciones.

No modifiques decisiones aprobadas sin autorización.

---

## 24. Condiciones de finalización

La instrucción estará completada cuando:

1. Se haya definido el valor mínimo.
    
2. El escenario principal esté identificado.
    
3. Las capacidades incluidas estén justificadas.
    
4. Los RF seleccionados estén documentados.
    
5. Los RNF aplicables estén identificados.
    
6. Los CA relevantes estén asociados.
    
7. Las dependencias estén cubiertas o registradas como bloqueantes.
    
8. Los controles de seguridad indispensables estén incluidos.
    
9. Los aplazamientos estén justificados.
    
10. Las exclusiones estén claras.
    
11. La viabilidad esté evaluada.
    
12. Los riesgos estén documentados.
    
13. Las condiciones de salida sean verificables.
    
14. Exista trazabilidad.
    
15. Las contradicciones bloqueantes estén resueltas.
    
16. Se haya generado `mvp-definition.md`.
    
17. Yo haya revisado y aprobado la definición.
    

No avances automáticamente.

---

## 25. Comportamiento al finalizar

Presenta un resumen breve con:

**Valor del MVP:** resultado principal.

**Capacidades:** elementos incluidos.

**Requisitos:** RF y RNF relevantes.

**Seguridad:** controles indispensables.

**Dependencias:** elementos bloqueantes.

**Exclusiones:** capacidades aplazadas.

**Riesgos:** principales incertidumbres.

**Condiciones de salida:** cómo sabremos que está terminado.

**Entregable:** `mvp-definition.md`.

**Siguiente paso:** `10 - Crear roadmap.md`.

Solicita mi aprobación antes de continuar.

---

## 26. Principio rector

**El MVP debe ser mínimo en alcance, no en responsabilidad.**

No incluyas funcionalidades que no aportan al primer valor.

No elimines dependencias indispensables.

No ignores casos negativos relevantes.

No reduzcas controles de seguridad necesarios.

No inventes requisitos.

No declares que el MVP está listo sin evidencias.

El objetivo es entregar el menor producto coherente que pueda utilizarse y verificarse en las condiciones aprobadas.

---

## 27. Instrucción de inicio

Si dispones de los documentos de entrada:

1. Analízalos.
    
2. Resume el objetivo del producto.
    
3. Identifica el escenario de mayor valor para la primera entrega.
    
4. Propón una definición preliminar del resultado mínimo.
    
5. Identifica capacidades candidatas.
    
6. Formula las preguntas necesarias antes de cerrar la selección.
    

Si faltan documentos, solicita la información imprescindible.

No selecciones definitivamente el MVP sin comprender sus dependencias, riesgos y condiciones de salida.