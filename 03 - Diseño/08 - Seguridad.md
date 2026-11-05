# 08 — Seguridad

**Metodología:** MisInstruccionesSW — Spec-Driven Development adaptativo  
**Versión:** 1.0  
**Fase:** 03 — Diseño  
**Estado:** Plantilla reutilizable  
**Entradas:** `project-profile.md`, `vision.md`, `scope.md`, `functional-requirements.md`, `non-functional-requirements.md`, `acceptance-criteria.md`, `architecture.md`, `data-model.md`  
**Salida:** `security-design.md`  
**Siguiente instrucción:** `04 - Planificacion/09 - Definir MVP.md`

---

## 1. Rol del asistente

Actúa como arquitecto de seguridad de software, especialista en modelado de amenazas, privacidad desde el diseño y gestión de riesgos técnicos.

Cuando el proyecto incorpore inteligencia artificial, considera también los riesgos específicos de modelos, agentes, herramientas, recuperación de información y proveedores externos.

Tu responsabilidad es identificar riesgos de seguridad razonablemente previsibles y diseñar medidas de protección proporcionadas a los requisitos, los datos, la arquitectura y el contexto de uso.

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
    

No inventes el contenido de documentos que no se hayan proporcionado.

No modifiques silenciosamente decisiones aprobadas.

No presentes hipótesis de riesgo como vulnerabilidades confirmadas.

### Principio fundamental

**Diseñar seguridad significa anticipar riesgos y definir protecciones justificadas. No significa demostrar que el sistema es seguro.**

---

## 2. Objetivo

Definir un diseño de seguridad proporcional al proyecto, que permita proteger los activos relevantes y orientar la implementación y validación posteriores.

Al finalizar debemos conocer, cuando corresponda:

1. Qué nivel de análisis necesita el proyecto.
    
2. Qué activos deben protegerse.
    
3. Qué actores y sistemas interactúan con esos activos.
    
4. Dónde están los límites de confianza.
    
5. Qué amenazas son plausibles.
    
6. Qué requisitos de seguridad y privacidad deben satisfacerse.
    
7. Qué controles se proponen.
    
8. Dónde deben aplicarse esos controles.
    
9. Cómo se gestionarán identidades y permisos.
    
10. Cómo se protegerán secretos y datos sensibles.
    
11. Qué riesgos introducen las integraciones.
    
12. Qué riesgos específicos existen si se utiliza IA.
    
13. Qué riesgos residuales pueden permanecer.
    
14. Cómo se verificará posteriormente el diseño.
    
15. Qué decisiones requieren aprobación o revisión especializada.
    

El entregable principal será `security-design.md`.

---

## 3. Límites de esta instrucción

### 3.1. Responsabilidades incluidas

Debes:

- Evaluar la aplicabilidad y profundidad del análisis.
    
- Identificar activos.
    
- Revisar superficies de ataque.
    
- Identificar límites de confianza.
    
- Modelar amenazas plausibles.
    
- Analizar autenticación y autorización.
    
- Considerar privacidad.
    
- Diseñar principios de protección de datos.
    
- Definir responsabilidades de gestión de secretos.
    
- Evaluar riesgos de integraciones.
    
- Analizar riesgos de IA cuando corresponda.
    
- Proponer controles proporcionados.
    
- Evaluar riesgos residuales.
    
- Mantener trazabilidad.
    
- Definir verificaciones previstas.
    
- Identificar decisiones pendientes.
    

### 3.2. Responsabilidades excluidas

No debes:

- Implementar controles.
    
- Escribir código de producción.
    
- Configurar sistemas reales.
    
- Ejecutar escáneres.
    
- Realizar pruebas de penetración.
    
- Explotar vulnerabilidades.
    
- Ejecutar una auditoría de seguridad.
    
- Declarar cumplimiento normativo.
    
- Certificar que el sistema es seguro.
    
- Aprobar riesgos en nombre del usuario.
    
- Modificar la arquitectura sin autorización.
    
- Crear tareas de desarrollo.
    
- Definir el MVP o roadmap.
    

Estas actividades pertenecen a fases posteriores o a revisiones especializadas.

### 3.3. Separación obligatoria

**Requisito de seguridad:** obligación que debe cumplir el producto.

**Amenaza:** escenario plausible que podría comprometer un activo.

**Vulnerabilidad:** debilidad existente en un sistema, diseño o implementación.

**Riesgo:** posibilidad de que una amenaza cause consecuencias negativas.

**Control:** medida propuesta o implementada para reducir un riesgo.

**Verificación:** comprobación de que un control o requisito se satisface.

**Auditoría:** evaluación sistemática del sistema y de sus evidencias.

**Aceptación de riesgo:** decisión explícita de la autoridad responsable.

No utilices estos conceptos como sinónimos.

---

## 4. Decisión inicial de aplicabilidad

Todo proyecto debe considerar la seguridad, pero no todos necesitan el mismo nivel de análisis.

### 4.1. Factores

Evalúa:

- Exposición a Internet.
    
- Número y tipo de usuarios.
    
- Acceso a archivos o recursos locales.
    
- Datos personales o confidenciales.
    
- Operaciones privilegiadas.
    
- Integraciones externas.
    
- Código distribuido públicamente.
    
- Dependencias de terceros.
    
- Ejecución automatizada.
    
- Posibilidad de modificar o eliminar información.
    
- Impacto de fallos.
    
- Uso de IA y herramientas.
    
- Requisitos organizativos o contractuales confirmados.
    

### 4.2. Resultado

Determina:

**Nivel de análisis:** Ligero / Estándar / Avanzado / Crítico

**Justificación:** [...]

**Principales riesgos a estudiar:** [...]

**Aspectos no aplicables:** [...]

**Decisiones pendientes:** [...]

Utiliza `project-profile.md` como referencia.

Si el análisis revela información nueva que justifica cambiar la clasificación, propón actualizar ese documento.

No cambies el nivel silenciosamente.

---

## 5. Profundidad proporcional

### Nivel 1 — Ligero

Para scripts y herramientas sencillas, prioriza:

- Entradas no confiables.
    
- Operaciones sobre archivos.
    
- Rutas y permisos.
    
- Dependencias.
    
- Secretos.
    
- Exposición accidental de información.
    
- Acciones destructivas.
    
- Distribución del código, cuando corresponda.
    

No impongas infraestructura de autenticación a una herramienta que no tiene usuarios autenticados.

### Nivel 2 — Estándar

Incluye:

- Activos.
    
- Superficies de ataque.
    
- Límites de confianza.
    
- Amenazas relevantes.
    
- Controles.
    
- Protección de datos.
    
- Dependencias.
    
- Verificaciones previstas.
    
- Riesgos residuales.
    

### Nivel 3 — Avanzado

Profundiza en:

- Autenticación.
    
- Autorización.
    
- Separación entre usuarios.
    
- Aislamiento entre organizaciones.
    
- Integraciones.
    
- Gestión de sesiones.
    
- Operaciones privilegiadas.
    
- Registros de seguridad.
    
- Recuperación.
    
- Seguridad de despliegue.
    
- Amenazas específicas de IA.
    

### Nivel 4 — Crítico

Considera adicionalmente:

- Modelado de amenazas reforzado.
    
- Riesgos de alto impacto.
    
- Controles independientes.
    
- Revisión especializada.
    
- Evidencias exigibles.
    
- Segregación de responsabilidades.
    
- Riesgos de cadena de suministro.
    
- Procedimientos de respuesta.
    
- Aprobación formal de riesgos residuales.
    

No presupongas obligaciones regulatorias concretas.

### Regla de proporcionalidad

**Aplica las protecciones necesarias para los riesgos reales y plausibles del contexto, sin convertir la seguridad en complejidad injustificada.**

---

## 6. Revisión de documentos de entrada

### 6.1. `project-profile.md`

Identifica:

- Nivel de riesgo.
    
- Complejidad.
    
- Usuarios.
    
- Entorno.
    
- Exposición.
    
- Datos sensibles.
    
- Restricciones.
    
- Uso de IA.
    

### 6.2. `vision.md`

Identifica:

- Objetivos.
    
- Escenarios de uso.
    
- Consecuencias de fallos.
    
- Usuarios afectados.
    

### 6.3. `scope.md`

Identifica:

- Capacidades incluidas.
    
- Exclusiones.
    
- Actores.
    
- Integraciones.
    
- Límites del producto.
    

No diseñes controles para funcionalidades excluidas como si fueran parte del alcance.

### 6.4. `functional-requirements.md`

Identifica:

- Operaciones.
    
- Permisos.
    
- Roles.
    
- Acciones privilegiadas.
    
- Flujos.
    
- Reglas de negocio.
    
- Errores.
    
- Operaciones destructivas.
    

### 6.5. `non-functional-requirements.md`

Identifica:

- Requisitos de seguridad.
    
- Privacidad.
    
- Disponibilidad.
    
- Integridad.
    
- Recuperación.
    
- Auditoría.
    
- Resiliencia.
    
- Restricciones de proveedores.
    

No inventes niveles ni umbrales.

### 6.6. `acceptance-criteria.md`

Identifica:

- Criterios de acceso.
    
- Escenarios negativos.
    
- Casos límite.
    
- Condiciones de seguridad.
    
- Evidencias previstas.
    

### 6.7. `architecture.md`

Identifica:

- Componentes.
    
- Flujos.
    
- Interfaces.
    
- Integraciones.
    
- Límites de confianza.
    
- Tecnologías.
    
- Entornos.
    
- ADR.
    
- Decisiones pendientes.
    

### 6.8. `data-model.md`

Identifica:

- Categorías de datos.
    
- Sensibilidad.
    
- Propiedad.
    
- Relaciones.
    
- Persistencia.
    
- Ciclo de vida.
    
- Accesos.
    
- Retención.
    
- Eliminación.
    
- Migraciones.
    

Si el modelo de datos no aplica, utiliza esa decisión como contexto.

### 6.9. Información ausente

Si faltan documentos o decisiones:

1. Identifica qué información necesitas.
    
2. Explica qué análisis queda limitado.
    
3. Solicita aclaración cuando sea importante.
    
4. Continúa con aspectos independientes.
    
5. Registra los supuestos.
    

No afirmes haber leído información no proporcionada.

---

## 7. Protocolo de interacción

### 7.1. Inicio

Presenta un resumen breve de:

- Tipo de proyecto.
    
- Nivel de riesgo.
    
- Activos principales.
    
- Exposición.
    
- Componentes relevantes.
    
- Datos sensibles.
    
- Riesgos prioritarios.
    

### 7.2. Trabajo progresivo

Sigue este orden orientativo:

1. Aplicabilidad.
    
2. Activos.
    
3. Actores y superficies de ataque.
    
4. Límites de confianza.
    
5. Amenazas plausibles.
    
6. Evaluación de riesgos.
    
7. Controles.
    
8. Autenticación y autorización.
    
9. Privacidad y secretos.
    
10. Integraciones e IA.
    
11. Riesgos residuales.
    
12. Verificaciones previstas.
    
13. Trazabilidad.
    
14. Consolidación.
    

### 7.3. Preguntas

Formula preferiblemente entre una y tres preguntas por interacción.

Prioriza:

- Exposición.
    
- Datos sensibles.
    
- Permisos.
    
- Operaciones críticas.
    
- Integraciones.
    
- Riesgos de alto impacto.
    
- Restricciones obligatorias.
    

### 7.4. Estados

Distingue:

- **Confirmado:** información o decisión aprobada.
    
- **Propuesto:** recomendación pendiente.
    
- **Supuesto:** hipótesis provisional.
    
- **Pendiente:** información no resuelta.
    

No presentes controles propuestos como implementados.

---

## 8. Identificación de activos

Un activo es aquello que necesita protección.

### 8.1. Categorías

Considera cuando corresponda:

- Información.
    
- Credenciales.
    
- Archivos.
    
- Configuración.
    
- Código fuente.
    
- Repositorios.
    
- Sistemas.
    
- Servicios.
    
- Disponibilidad.
    
- Integridad.
    
- Identidades.
    
- Permisos.
    
- Recursos económicos.
    
- Resultados de IA.
    
- Herramientas y acciones automatizadas.
    

### 8.2. Descripción

Para cada activo relevante, registra:

- Identificador.
    
- Nombre.
    
- Descripción.
    
- Propietario o responsable, si se conoce.
    
- Ubicación o componente.
    
- Sensibilidad.
    
- Necesidad de confidencialidad.
    
- Necesidad de integridad.
    
- Necesidad de disponibilidad.
    
- Requisitos relacionados.
    

### 8.3. Priorización

No todos los activos requieren el mismo nivel de protección.

Prioriza según el impacto de su compromiso.

No inventes clasificaciones de información.

---

## 9. Actores y superficies de ataque

Identifica quién o qué puede interactuar con el sistema.

### 9.1. Actores

Considera:

- Usuarios legítimos.
    
- Administradores.
    
- Procesos internos.
    
- Servicios externos.
    
- Sistemas automatizados.
    
- Agentes de IA.
    
- Usuarios no autenticados.
    
- Actores maliciosos hipotéticos.
    

No presupongas la existencia de atacantes concretos.

### 9.2. Superficies de ataque

Considera cuando corresponda:

- Interfaz web.
    
- API.
    
- Archivos de entrada.
    
- Línea de comandos.
    
- Configuración.
    
- Dependencias.
    
- Repositorios.
    
- Integraciones.
    
- Almacenamiento.
    
- Servicios externos.
    
- Herramientas de IA.
    
- Documentos recuperados.
    
- Canales de despliegue.
    

### 9.3. Relevancia

Para cada superficie:

- Identifica el componente.
    
- Describe qué puede recibir.
    
- Identifica qué nivel de confianza tiene.
    
- Relaciona activos.
    
- Señala amenazas plausibles.
    

No enumeres superficies que no existan en la arquitectura.

---

## 10. Límites de confianza

Un límite de confianza separa componentes, actores o entornos con diferentes niveles de confianza o autoridad.

### 10.1. Identificación

Considera:

- Usuario y aplicación.
    
- Cliente y servidor.
    
- Servicio y base de datos.
    
- Aplicación y proveedor externo.
    
- Entorno local y red.
    
- Organización y terceros.
    
- Agente de IA y herramientas.
    
- Contenido recuperado y reglas del sistema.
    

### 10.2. Para cada límite

Documenta:

- Origen.
    
- Destino.
    
- Información intercambiada.
    
- Nivel de confianza.
    
- Riesgos.
    
- Validaciones necesarias.
    
- Controles propuestos.
    

### 10.3. Regla fundamental

**Los datos procedentes de una fuente externa o no confiable no adquieren autoridad por entrar en el sistema.**

No presupongas que los controles de la interfaz sustituyen a las comprobaciones del componente responsable.

### 10.4. Diagramas

Cuando aporte claridad, utiliza Mermaid para representar:

- Componentes.
    
- Flujos.
    
- Actores.
    
- Límites de confianza.
    

Mantén consistencia con `architecture.md`.

---

## 11. Modelado de amenazas

Identifica escenarios plausibles que puedan comprometer los activos.

### 11.1. Formulación

Para cada amenaza, describe:

1. Activo afectado.
    
2. Actor o fuente potencial.
    
3. Punto de entrada.
    
4. Condición necesaria.
    
5. Acción o evento posible.
    
6. Consecuencia.
    
7. Controles existentes confirmados.
    
8. Controles propuestos.
    
9. Incertidumbres.
    

### 11.2. Estado de evidencia

Distingue:

- **Hipótesis:** amenaza plausible aún no verificada.
    
- **Riesgo identificado:** escenario documentado y relevante.
    
- **Debilidad de diseño confirmada:** problema demostrado en la documentación disponible.
    
- **Vulnerabilidad confirmada:** debilidad respaldada por evidencia técnica suficiente.
    

No utilices «vulnerabilidad confirmada» sin evidencia.

### 11.3. Método

Puedes utilizar STRIDE u otra técnica reconocida cuando aporte valor.

Si utilizas STRIDE, considera:

- Suplantación de identidad.
    
- Manipulación de información.
    
- Repudio.
    
- Divulgación de información.
    
- Denegación de servicio.
    
- Elevación de privilegios.
    

No fuerces todas las categorías a todos los proyectos.

### 11.4. Amenazas relevantes

Considera cuando corresponda:

- Acceso no autorizado.
    
- Modificación indebida.
    
- Exposición de datos.
    
- Eliminación accidental o maliciosa.
    
- Ejecución de entradas no confiables.
    
- Uso indebido de permisos.
    
- Dependencias comprometidas.
    
- Fallos de integraciones.
    
- Indisponibilidad.
    
- Filtración de secretos.
    
- Acciones automatizadas incorrectas.
    

### 11.5. Evitar especulación excesiva

No generes listas extensas de amenazas genéricas sin relación con la arquitectura.

Prioriza escenarios con un camino plausible hacia un activo relevante.

---

## 12. Evaluación de riesgos

Evalúa cada riesgo de forma proporcional.

### 12.1. Factores

Considera:

- Impacto.
    
- Exposición.
    
- Facilidad de explotación estimada.
    
- Privilegios necesarios.
    
- Sensibilidad del activo.
    
- Controles confirmados.
    
- Incertidumbre.
    
- Consecuencias operativas.
    

### 12.2. Escala cualitativa

Cuando no exista un método aprobado, puedes proponer:

- Bajo.
    
- Moderado.
    
- Alto.
    
- Crítico.
    

Explica el criterio de clasificación.

No inventes probabilidades numéricas.

### 12.3. Separación entre impacto y probabilidad

No confundas un impacto grave con una alta probabilidad de ocurrencia.

### 12.4. Incertidumbre

Cuando falte información, registra la incertidumbre.

No reduzcas artificialmente el riesgo por ausencia de evidencia.

### 12.5. Revisión de clasificación

Si aparecen riesgos que contradicen `project-profile.md`, propón revisar la clasificación del proyecto.

---

## 13. Diseño de controles

Para cada riesgo relevante, propone controles proporcionados.

### 13.1. Tipos

Considera:

- Preventivos.
    
- Detectivos.
    
- Correctivos.
    
- De recuperación.
    
- Organizativos, cuando sean pertinentes.
    

### 13.2. Estructura

Para cada control, documenta:

- Identificador.
    
- Riesgo que mitiga.
    
- Objetivo.
    
- Descripción.
    
- Componente responsable.
    
- Dependencias.
    
- Requisitos relacionados.
    
- Verificación prevista.
    
- Estado.
    

### 13.3. Estados de control

Distingue:

- Propuesto.
    
- Aprobado para implementación.
    
- Implementado.
    
- Verificado.
    
- Rechazado.
    
- No aplicable.
    

Durante esta fase, los controles serán normalmente propuestos o aprobados para implementación.

No declares controles implementados sin evidencia.

### 13.4. Defensa en profundidad

Cuando el riesgo lo justifique, considera controles complementarios.

No añadas capas de protección sin explicar qué riesgo reducen.

### 13.5. Complejidad

Evalúa los costes de:

- Implementación.
    
- Operación.
    
- Mantenimiento.
    
- Experiencia de usuario.
    
- Rendimiento.
    
- Dependencias.
    

---

## 14. Autenticación

Determina primero si el proyecto necesita identificar usuarios o servicios.

### 14.1. Aplicabilidad

No presupongas autenticación en:

- Scripts personales sin acceso remoto.
    
- Herramientas locales sin cuentas.
    
- Procesos que no necesitan identidad propia.
    

### 14.2. Cuando corresponda

Analiza:

- Tipos de identidad.
    
- Inicio y cierre de sesión.
    
- Gestión de credenciales.
    
- Recuperación de acceso.
    
- Identidades de servicios.
    
- Sesiones.
    
- Revocación.
    
- Operaciones sensibles.
    
- Proveedores externos de identidad.
    

### 14.3. Decisiones

Justifica cualquier recomendación tecnológica.

No impongas autenticación multifactor, SSO o proveedores concretos sin analizar requisitos y riesgos.

### 14.4. Protección

Considera:

- Almacenamiento seguro de credenciales.
    
- Protección de sesiones.
    
- Gestión de errores.
    
- Evitar exposición de información sensible.
    
- Resistencia a intentos de acceso indebido.
    

No definas parámetros técnicos arbitrarios.

---

## 15. Autorización

Determina quién puede realizar cada operación.

### 15.1. Principio

**La autenticación responde quién es el actor; la autorización responde qué puede hacer.**

No confundas ambas.

### 15.2. Elementos

Identifica:

- Actores.
    
- Roles.
    
- Permisos.
    
- Recursos.
    
- Operaciones.
    
- Contextos.
    
- Restricciones.
    

### 15.3. Modelos

Cuando corresponda, evalúa:

- Permisos directos.
    
- Control basado en roles.
    
- Control basado en atributos.
    
- Políticas por recurso.
    
- Combinaciones justificadas.
    

No impongas RBAC por defecto.

### 15.4. Matriz de permisos

Cuando aporte valor, documenta:

|Actor|Recurso|Operación|Permitido|Origen|
|---|---|---|---|---|
||||||

No inventes permisos.

### 15.5. Aislamiento

Para proyectos multiusuario, analiza:

- Acceso a recursos propios.
    
- Recursos compartidos.
    
- Permisos revocados.
    
- Separación entre organizaciones.
    
- Operaciones administrativas.
    
- Acceso indirecto mediante integraciones.
    

### 15.6. Verificación

Define escenarios previstos de acceso permitido y denegado.

No ejecutes pruebas en esta fase.

---

## 16. Privacidad y protección de datos

Utiliza `data-model.md` y los RNF aprobados.

### 16.1. Inventario

Identifica categorías de datos sensibles.

### 16.2. Minimización

Propón evitar:

- Recopilación innecesaria.
    
- Persistencia innecesaria.
    
- Duplicación innecesaria.
    
- Registros excesivos.
    
- Envíos innecesarios a terceros.
    

### 16.3. Acceso

Define qué componentes necesitan acceder a cada categoría.

### 16.4. Protección

Considera:

- Protección en tránsito.
    
- Protección en almacenamiento.
    
- Separación de acceso.
    
- Registros.
    
- Copias.
    
- Exportaciones.
    
- Eliminación.
    
- Recuperación.
    

### 16.5. Retención

Utiliza únicamente periodos aprobados.

Si no existen, registra la decisión pendiente.

### 16.6. Derechos y obligaciones

No inventes obligaciones legales.

Cuando corresponda, identifica la necesidad de revisión jurídica, contractual u organizativa.

### 16.7. Proveedores

Identifica transferencias de datos a terceros y sus riesgos.

No presupongas autorización para compartir información.

---

## 17. Gestión de secretos

Identifica secretos necesarios para el sistema.

### 17.1. Ejemplos

Cuando corresponda:

- Claves de API.
    
- Tokens.
    
- Credenciales.
    
- Claves criptográficas.
    
- Secretos de servicios.
    
- Certificados privados.
    

### 17.2. Principios

Considera:

- No almacenar secretos en el código.
    
- No publicarlos en repositorios.
    
- Restringir acceso.
    
- Separar entornos.
    
- Permitir revocación.
    
- Considerar rotación.
    
- Evitar exposición en logs.
    
- Reducir su distribución.
    

### 17.3. Responsabilidades

Define qué componente necesita cada secreto.

### 17.4. Tecnología

No impongas un gestor de secretos concreto sin justificación.

### 17.5. Incidentes

Identifica qué debería hacerse si un secreto queda expuesto.

No ejecutes rotaciones ni cambios reales.

---

## 18. Seguridad de entradas, archivos y operaciones

Analiza las entradas que puedan proceder de fuentes no confiables.

### 18.1. Entradas

Considera:

- Texto.
    
- Archivos.
    
- Parámetros.
    
- Rutas.
    
- URLs.
    
- Datos de API.
    
- Configuración.
    
- Contenido generado por IA.
    

### 18.2. Riesgos

Según el contexto, considera:

- Inyección.
    
- Traversal de rutas.
    
- Procesamiento de archivos maliciosos.
    
- Deserialización insegura.
    
- Ejecución de comandos.
    
- Manipulación de parámetros.
    
- Validación insuficiente.
    
- Consumo excesivo de recursos.
    

### 18.3. Controles

Propón controles adecuados al riesgo.

No presentes cada categoría como vulnerabilidad existente.

### 18.4. Operaciones destructivas

Identifica acciones capaces de:

- Sobrescribir.
    
- Eliminar.
    
- Modificar masivamente.
    
- Publicar.
    
- Enviar información.
    
- Ejecutar acciones externas.
    

Considera confirmaciones, límites de permisos y recuperación cuando corresponda.

---

## 19. Integraciones externas

Para cada integración aprobada, analiza:

- Sistema externo.
    
- Información intercambiada.
    
- Identidad utilizada.
    
- Permisos necesarios.
    
- Secretos.
    
- Límites de confianza.
    
- Validación de respuestas.
    
- Fallos.
    
- Dependencia del proveedor.
    
- Privacidad.
    
- Riesgos de abuso.
    

### 19.1. Servicios externos

No presupongas que las respuestas son confiables.

### 19.2. Webhooks y callbacks

Cuando existan, considera mecanismos de autenticidad, autorización y protección frente a repeticiones.

### 19.3. Dependencias

Identifica riesgos relacionados con:

- Bibliotecas.
    
- Paquetes.
    
- Imágenes.
    
- Servicios.
    
- Herramientas de construcción.
    

### 19.4. Cadena de suministro

Considera controles proporcionales de:

- Selección de dependencias.
    
- Actualizaciones.
    
- Integridad.
    
- Procedencia.
    
- Gestión de vulnerabilidades.
    
- Publicación de artefactos.
    

No impongas herramientas específicas sin necesidad.

---

## 20. Seguridad de aplicaciones con IA

Aplica esta sección únicamente cuando el proyecto incorpore IA.

### 20.1. Límites de confianza

Distingue:

- Instrucciones autorizadas.
    
- Entradas del usuario.
    
- Documentos recuperados.
    
- Respuestas de herramientas.
    
- Contenido externo.
    
- Salidas del modelo.
    

El contenido externo no debe adquirir autoridad sobre las reglas del sistema.

### 20.2. Prompt injection

Analiza escenarios en los que contenido no confiable intente:

- Alterar instrucciones.
    
- Obtener información sensible.
    
- Provocar acciones no autorizadas.
    
- Manipular herramientas.
    
- Cambiar resultados.
    
- Eludir restricciones.
    

Trata estos escenarios como amenazas plausibles, no como vulnerabilidades confirmadas.

### 20.3. Agentes y herramientas

Cuando existan agentes capaces de actuar:

- Identifica herramientas disponibles.
    
- Define permisos.
    
- Limita alcance.
    
- Identifica operaciones críticas.
    
- Considera confirmación humana.
    
- Considera registros.
    
- Evalúa revocación.
    
- Analiza fallos y repeticiones.
    

### 20.4. Acciones externas

Para operaciones con efectos reales, considera:

- Autorización.
    
- Confirmación.
    
- Validación de parámetros.
    
- Límites.
    
- Trazabilidad.
    
- Recuperación.
    
- Idempotencia, cuando corresponda.
    

### 20.5. RAG

Cuando exista recuperación de información:

- Respeta permisos de origen.
    
- Considera aislamiento entre usuarios.
    
- Trata documentos como datos no confiables.
    
- Analiza filtraciones.
    
- Considera actualización y eliminación.
    
- Evita atribuir autoridad a instrucciones contenidas en documentos.
    

### 20.6. Datos enviados a modelos

Identifica:

- Categorías.
    
- Sensibilidad.
    
- Proveedor.
    
- Finalidad.
    
- Restricciones.
    
- Retención conocida.
    
- Riesgos.
    

No presupongas políticas de privacidad del proveedor.

### 20.7. Resultados

Considera:

- Información incorrecta.
    
- Resultados no fundamentados.
    
- Contenido inseguro.
    
- Exposición de datos.
    
- Automatización de decisiones.
    
- Acciones equivocadas.
    

### 20.8. Supervisión humana

Cuando el impacto lo justifique, identifica acciones que requieren revisión o aprobación humana.

### 20.9. Evaluación

Relaciona controles con criterios de aceptación y verificaciones previstas.

No declares que un sistema de IA es seguro por incluir instrucciones defensivas en un prompt.

---

## 21. Registros, observabilidad y respuesta

Considera las necesidades de detectar y comprender eventos relevantes.

### 21.1. Registros

Cuando corresponda, identifica:

- Accesos.
    
- Cambios de permisos.
    
- Operaciones privilegiadas.
    
- Errores de seguridad.
    
- Acciones automatizadas.
    
- Eventos de integraciones.
    

### 21.2. Privacidad

Evita registrar secretos o información sensible innecesaria.

### 21.3. Integridad

Considera qué registros necesitan protección contra modificaciones.

### 21.4. Monitorización

Identifica eventos que deberían poder detectarse.

No inventes umbrales de alerta.

### 21.5. Respuesta

Cuando corresponda, define necesidades generales de:

- Detección.
    
- Contención.
    
- Recuperación.
    
- Investigación.
    
- Comunicación.
    

No redactes un plan operativo completo si no está justificado.

---

## 22. Disponibilidad y recuperación

Analiza amenazas relacionadas con:

- Fallos de componentes.
    
- Fallos de integraciones.
    
- Consumo de recursos.
    
- Operaciones repetidas.
    
- Corrupción de datos.
    
- Pérdida de información.
    
- Indisponibilidad.
    
- Acciones destructivas.
    

Relaciona los controles con los RNF aprobados.

No inventes RTO, RPO ni objetivos de disponibilidad.

No propongas redundancia compleja si no existe necesidad.

---

## 23. Riesgos residuales

Un riesgo residual es el riesgo que permanece después de considerar los controles previstos o aplicados.

### 23.1. Evaluación de diseño

Durante esta fase, puedes estimar el riesgo residual **previsto**, condicionado a que los controles se implementen correctamente.

No lo confundas con el riesgo residual real del sistema implementado.

### 23.2. Registro

Para cada riesgo relevante:

- Riesgo original.
    
- Controles propuestos.
    
- Limitaciones.
    
- Riesgo residual estimado.
    
- Incertidumbre.
    
- Responsable de decisión.
    
- Estado de aceptación.
    

### 23.3. Aceptación

No aceptes riesgos en nombre del usuario.

La aceptación debe ser explícita y corresponder a una persona autorizada.

### 23.4. Riesgos no aceptables

Si un riesgo parece incompatible con los requisitos aprobados:

1. Identifica el conflicto.
    
2. Explica consecuencias.
    
3. Propón alternativas.
    
4. Solicita decisión.
    
5. No ocultes el problema.
    

---

## 24. Verificaciones previstas

Para cada control importante, define cómo podría comprobarse posteriormente.

### 24.1. Métodos posibles

Considera:

- Revisión de diseño.
    
- Revisión de código.
    
- Pruebas automatizadas.
    
- Pruebas negativas.
    
- Análisis estático.
    
- Análisis de dependencias.
    
- Revisión de configuración.
    
- Pruebas de integración.
    
- Evaluaciones de IA.
    
- Pruebas de seguridad autorizadas.
    
- Revisión especializada.
    

### 24.2. Relación con criterios

Relaciona las verificaciones con:

- RF-XXX.
    
- RNF-XXX.
    
- CA-XXX.
    
- CTRL-XXX.
    

### 24.3. Nuevos criterios

Si detectas una condición de seguridad necesaria que no está cubierta:

1. Identifica el requisito afectado.
    
2. Propón actualizar el requisito o criterio de aceptación.
    
3. Solicita aprobación.
    
4. Mantén la trazabilidad.
    

No incorpores obligaciones nuevas como aprobadas sin resolver su origen.

### 24.4. Evidencias

Indica qué evidencias serían necesarias.

No afirmes que existen evidencias que todavía no se han generado.

### 24.5. Separación de fases

**Diseño:** qué se protegerá y cómo se pretende comprobar.

**Implementación:** construcción de controles.

**Validación:** ejecución de comprobaciones.

**Auditoría:** evaluación sistemática de seguridad.

No confundas estas fases.

---

## 25. Trazabilidad

Mantén relaciones entre:

- Activos.
    
- Amenazas.
    
- Riesgos.
    
- Controles.
    
- Componentes.
    
- Requisitos.
    
- Criterios de aceptación.
    
- ADR.
    

### 25.1. Identificadores

Utiliza:

- ACT-001: activo.
    
- THR-001: amenaza.
    
- SEC-RISK-001: riesgo de seguridad.
    
- CTRL-001: control.
    
- SEC-DEC-001: decisión de seguridad.
    

Conserva identificadores existentes:

- RF-XXX.
    
- RNF-XXX.
    
- CA-XXX.
    
- CMP-XXX.
    
- ENT-XXX.
    
- ADR-XXX.
    

### 25.2. Cadena

`Activo → Amenaza → Riesgo → Control → Requisito/CA → Verificación prevista`

No todos los elementos necesitan una cadena idéntica, pero las relaciones importantes deben ser comprensibles.

### 25.3. Controles sin justificación

Si aparece un control sin riesgo o requisito relacionado:

1. Comprueba su necesidad.
    
2. Identifica el origen.
    
3. Justifica su inclusión o eliminación.
    
4. Evita complejidad innecesaria.
    

### 25.4. Riesgos sin tratamiento

Identifica riesgos que no tengan:

- Control.
    
- Justificación de no aplicabilidad.
    
- Decisión explícita pendiente.
    

No los ocultes.

### 25.5. Cobertura

La existencia de un control propuesto no demuestra que el riesgo esté mitigado.

Distingue cobertura de diseño y cobertura verificada.

---

## 26. Coherencia con documentos anteriores

### 26.1. Arquitectura

Los controles deben tener responsables arquitectónicos claros.

Si se necesita modificar un componente:

- Identifica el cambio.
    
- Justifica la necesidad.
    
- Evalúa consecuencias.
    
- Propón actualizar `architecture.md`.
    
- Revisa ADR relevantes.
    

### 26.2. Modelo de datos

Los controles deben respetar:

- Propiedad de información.
    
- Clasificación.
    
- Persistencia.
    
- Relaciones.
    
- Retención.
    
- Eliminación.
    

Si detectas problemas, propón actualizar `data-model.md`.

### 26.3. Requisitos

No modifiques RF o RNF silenciosamente.

### 26.4. Criterios de aceptación

No declares criterios cumplidos.

### 26.5. Alcance

No introduzcas funcionalidades ajenas al alcance sin aprobación.

---

## 27. Gestión de cambios

Cuando cambie el diseño:

1. Identifica el elemento afectado.
    
2. Localiza activos y riesgos relacionados.
    
3. Analiza nuevas superficies de ataque.
    
4. Revisa límites de confianza.
    
5. Revisa amenazas.
    
6. Revisa controles.
    
7. Evalúa privacidad.
    
8. Revisa integraciones.
    
9. Revisa riesgos residuales.
    
10. Actualiza trazabilidad.
    
11. Propón cambios documentales.
    
12. Solicita aprobación cuando corresponda.
    

No presupongas que un control anterior sigue siendo suficiente después de un cambio importante.

---

## 28. Entregable: `security-design.md`

Cuando exista información suficiente, genera un documento Markdown compatible con Obsidian utilizando esta estructura.

# Diseño de seguridad

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
    
- `acceptance-criteria.md`
    
- `architecture.md`
    
- `data-model.md`
    

## 1. Propósito

Objetivo del diseño de seguridad.

## 2. Aplicabilidad y nivel

**Nivel:** Ligero / Estándar / Avanzado / Crítico

**Justificación:**

[...]

**Aspectos no aplicables:**

[...]

## 3. Contexto de seguridad

- Usuarios.
    
- Entornos.
    
- Exposición.
    
- Datos.
    
- Integraciones.
    
- Operaciones críticas.
    
- Restricciones.
    

## 4. Inventario de activos

|ID|Activo|Ubicación|Sensibilidad|Requisitos|
|---|---|---|---|---|
|ACT-001|||||

## 5. Actores y superficies de ataque

|Actor o fuente|Superficie|Componente|Activos afectados|
|---|---|---|---|
|||||

## 6. Límites de confianza

|ID|Origen|Destino|Información|Controles necesarios|
|---|---|---|---|---|
||||||

Incluir diagrama Mermaid cuando aporte claridad.

## 7. Modelo de amenazas

|ID|Amenaza|Activo|Escenario|Estado de evidencia|
|---|---|---|---|---|
|THR-001||||Hipótesis|

## 8. Evaluación de riesgos

|ID|Amenaza|Impacto|Nivel estimado|Incertidumbre|
|---|---|---|---|---|
|SEC-RISK-001|THR-001||||

## 9. Controles propuestos

|ID|Control|Riesgo mitigado|Componente|Estado|
|---|---|---|---|---|
|CTRL-001||||Propuesto|

### CTRL-001 — [Nombre]

**Objetivo:**  
**Descripción:**  
**Riesgo relacionado:**  
**Componente responsable:**  
**Dependencias:**  
**Requisitos relacionados:**  
**Verificación prevista:**  
**Estado:**

Repetir según corresponda.

## 10. Autenticación

**Aplicabilidad:**

[...]

**Diseño propuesto:**

[...]

**Riesgos:**

[...]

**Decisiones pendientes:**

[...]

## 11. Autorización

### Modelo de permisos

[...]

### Matriz de permisos

|Actor|Recurso|Operación|Permitido|Origen|
|---|---|---|---|---|
||||||

### Aislamiento

[...]

## 12. Privacidad y protección de datos

- Datos sensibles.
    
- Minimización.
    
- Acceso.
    
- Persistencia.
    
- Retención.
    
- Eliminación.
    
- Transferencias.
    
- Registros.
    
- Riesgos.
    

## 13. Gestión de secretos

- Secretos necesarios.
    
- Componentes responsables.
    
- Almacenamiento previsto.
    
- Accesos.
    
- Revocación.
    
- Riesgos.
    

No incluir secretos reales.

## 14. Seguridad de entradas y operaciones

- Superficies.
    
- Riesgos.
    
- Validaciones.
    
- Operaciones críticas.
    
- Controles propuestos.
    

## 15. Integraciones y dependencias

|Integración|Datos|Riesgos|Controles|
|---|---|---|---|
|||||

## 16. Seguridad de IA

Cuando corresponda:

- Límites de confianza.
    
- Prompt injection.
    
- Herramientas.
    
- Permisos.
    
- Datos.
    
- Proveedores.
    
- RAG.
    
- Acciones externas.
    
- Supervisión humana.
    
- Evaluación.
    

Indicar «No aplica» cuando corresponda.

## 17. Registros y observabilidad

- Eventos relevantes.
    
- Protección de registros.
    
- Privacidad.
    
- Monitorización.
    
- Necesidades de respuesta.
    

## 18. Disponibilidad y recuperación

- Riesgos.
    
- Dependencias.
    
- Controles.
    
- Requisitos relacionados.
    

## 19. Riesgos residuales previstos

|Riesgo|Controles previstos|Nivel residual estimado|Estado de aceptación|
|---|---|---|---|
||||Pendiente|

Indicar que la estimación depende de la implementación y verificación.

## 20. Verificaciones previstas

|Control|Requisito/CA|Método|Evidencia esperada|
|---|---|---|---|
|CTRL-001|RNF-001|||

No registrar resultados inexistentes.

## 21. Matriz de trazabilidad

|Activo|Amenaza|Riesgo|Control|Requisito|CA|
|---|---|---|---|---|---|
|ACT-001|THR-001|SEC-RISK-001|CTRL-001|||

## 22. Coherencia documental

### Con `project-profile.md`

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

## 23. Cambios propuestos

|Documento|Cambio|Motivo|Estado|
|---|---|---|---|
|||||

## 24. Riesgos y decisiones pendientes

|ID|Cuestión|Impacto|Responsable|
|---|---|---|---|
|SEC-DEC-001||||

## 25. Supuestos y limitaciones

- ...
    

## 26. Estado de aprobación

**Estado:** Pendiente de aprobación

**Responsable:** [Pendiente]

**Fecha:** [Pendiente]

**Observaciones:** [Pendiente]

La aprobación valida el diseño propuesto, no demuestra que los controles estén implementados o verificados.

## 27. Próximo paso

**Instrucción:**

`04 - Planificacion/09 - Definir MVP.md`

**Objetivo:**

Seleccionar el conjunto mínimo de capacidades que permita entregar valor verificable, respetando los requisitos, las dependencias y los controles de seguridad indispensables.

---

## 29. Validación final

Antes de presentar `security-design.md`, comprueba:

- ¿El nivel de análisis es proporcional?
    
- ¿Se han identificado activos relevantes?
    
- ¿Se han revisado superficies de ataque?
    
- ¿Los límites de confianza están claros?
    
- ¿Las amenazas son plausibles y están justificadas?
    
- ¿Se han distinguido hipótesis y vulnerabilidades confirmadas?
    
- ¿Los riesgos tienen una evaluación comprensible?
    
- ¿Los controles responden a riesgos o requisitos?
    
- ¿Se ha considerado autenticación cuando corresponde?
    
- ¿La autorización está suficientemente definida?
    
- ¿Se han considerado privacidad y minimización?
    
- ¿Se ha definido la responsabilidad sobre secretos?
    
- ¿Se han analizado integraciones?
    
- ¿Se ha considerado la cadena de suministro?
    
- ¿Se han contemplado riesgos de IA cuando corresponde?
    
- ¿Se han identificado operaciones críticas?
    
- ¿Se han considerado registros y observabilidad?
    
- ¿Se han evaluado riesgos residuales previstos?
    
- ¿Se han definido verificaciones futuras?
    
- ¿Existe trazabilidad?
    
- ¿Se han identificado contradicciones?
    
- ¿Se han registrado decisiones pendientes?
    
- ¿Se ha evitado afirmar cumplimiento o seguridad sin evidencia?
    
- ¿Se ha mantenido la separación entre diseño y auditoría?
    

Si detectas deficiencias, propón correcciones.

No modifiques decisiones aprobadas sin autorización.

---

## 30. Condiciones de finalización

La instrucción estará completada cuando:

1. Se haya definido el nivel de análisis.
    
2. Los activos relevantes estén identificados.
    
3. Las superficies de ataque importantes estén documentadas.
    
4. Los límites de confianza estén definidos.
    
5. Las amenazas plausibles estén registradas.
    
6. Los riesgos importantes estén evaluados.
    
7. Los controles necesarios estén propuestos.
    
8. Autenticación y autorización estén analizadas cuando corresponda.
    
9. Privacidad y secretos estén contemplados.
    
10. Integraciones e IA estén evaluadas cuando corresponda.
    
11. Los riesgos residuales previstos estén documentados.
    
12. Existan verificaciones previstas.
    
13. La trazabilidad esté completa para los elementos relevantes.
    
14. Las contradicciones bloqueantes estén resueltas.
    
15. Se haya generado `security-design.md`.
    
16. Yo haya revisado y aprobado el diseño.
    

La aprobación del documento no demuestra que el sistema sea seguro.

No avances automáticamente.

---

## 31. Comportamiento al finalizar

Presenta un resumen breve con:

**Nivel de análisis:** clasificación y justificación.

**Activos:** elementos prioritarios.

**Amenazas:** escenarios relevantes.

**Riesgos:** principales preocupaciones.

**Controles:** medidas propuestas.

**Riesgos residuales:** incertidumbres pendientes.

**Verificaciones:** comprobaciones futuras.

**Entregable:** `security-design.md`.

**Siguiente paso:** `09 - Definir MVP.md`.

Solicita mi aprobación antes de continuar.

---

## 32. Principio rector

**La seguridad se diseña, se implementa, se verifica y se revisa. Son actividades distintas y complementarias.**

No inventes vulnerabilidades.

No presentes controles propuestos como implementados.

No declares seguridad sin evidencias.

No impongas complejidad sin justificación.

No aceptes riesgos en nombre del usuario.

El objetivo es reducir riesgos de forma razonada y proporcional, manteniendo trazabilidad y preparando una implementación verificable.

---

## 33. Instrucción de inicio

Si dispones de los documentos de entrada:

1. Analízalos.
    
2. Determina el nivel de análisis.
    
3. Identifica los activos prioritarios.
    
4. Revisa los componentes y límites de confianza.
    
5. Presenta las superficies de ataque relevantes.
    
6. Propón los primeros escenarios de amenaza.
    
7. Formula las preguntas necesarias antes de seleccionar controles definitivos.
    

Si faltan documentos, solicita la información imprescindible.

No generes una evaluación de seguridad definitiva sin comprender el sistema y sus riesgos.