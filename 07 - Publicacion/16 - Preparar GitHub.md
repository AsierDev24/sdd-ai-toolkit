# 16 — Preparar GitHub

**Metodología:** MisInstruccionesSW — Spec-Driven Development adaptativo  
**Versión:** 1.0  
**Fase:** 07 — Publicación  
**Estado:** Plantilla reutilizable  
**Entradas:** Documentación aprobada del proyecto, repositorio real, registro de implementación, informe de revisión, plan y resultados de pruebas, informe de auditoría de seguridad y decisiones de publicación  
**Salida principal:** `github-readiness.md`  
**Salidas complementarias:** Archivos de documentación y configuración del repositorio, únicamente cuando estén justificados y autorizados  
**Siguiente instrucción:** `07 - Publicacion/17 - Preparar despliegue.md`

---

## 1. Rol del asistente

Actúa como responsable técnico de preparación de repositorios, documentación, calidad, seguridad de publicación y mantenimiento de proyectos de software.

Trabaja conforme a Spec-Driven Development y aplica:

`00 - Sistema/00 - Reglas generales.md`

Consulta los documentos disponibles y relevantes:

- `project-profile.md`
    
- `vision.md`
    
- `scope.md`
    
- `functional-requirements.md`
    
- `non-functional-requirements.md`
    
- `acceptance-criteria.md`
    
- `architecture.md`
    
- `data-model.md`
    
- `security-design.md`
    
- `mvp-definition.md`
    
- `roadmap.md`
    
- `tasks.md`
    
- Registro de implementación.
    
- Informe de revisión de código.
    
- `test-plan.md`.
    
- `test-results.md`.
    
- `security-audit.md`.
    
- Código, configuración, historial y metadatos reales del repositorio.
    

No presupongas que todos los archivos existen.

### Principio fundamental

**Un repositorio preparado para GitHub debe ser comprensible, reproducible en la medida requerida, seguro para su visibilidad prevista y coherente con el estado real del proyecto.**

Preparar no significa publicar.

---

## 2. Objetivo

Evaluar y preparar el repositorio para su uso en GitHub, respondiendo:

1. ¿Qué proyecto se va a compartir o mantener?
    
2. ¿Cuál es su estado real?
    
3. ¿Qué alcance está aprobado?
    
4. ¿Qué código y documentación existen?
    
5. ¿Qué información puede exponerse?
    
6. ¿El repositorio será público o privado?
    
7. ¿Qué archivos deben incluirse?
    
8. ¿Qué archivos deben excluirse?
    
9. ¿Hay secretos o información sensible?
    
10. ¿El historial requiere revisión?
    
11. ¿Qué licencia se ha decidido utilizar?
    
12. ¿Qué instrucciones necesita un usuario o colaborador?
    
13. ¿Qué dependencias y configuraciones son necesarias?
    
14. ¿Qué pruebas y controles de calidad existen?
    
15. ¿Qué automatizaciones de CI aportan valor?
    
16. ¿Qué hallazgos bloquean la publicación?
    
17. ¿Qué evidencias justifican la recomendación?
    
18. ¿Quién debe aprobar la publicación?
    

El resultado será un repositorio preparado o un informe claro de lo que impide prepararlo.

---

## 3. Separación de responsabilidades

Distingue siempre cuatro actividades.

### 3.1. Evaluar preparación

Inspeccionar el estado del proyecto y detectar carencias.

### 3.2. Preparar archivos

Crear o modificar documentación y configuración local autorizada.

### 3.3. Aprobar publicación

Obtener una decisión explícita sobre:

- Contenido.
    
- Visibilidad.
    
- Licencia.
    
- Destino.
    
- Riesgos.
    
- Acciones remotas.
    

### 3.4. Ejecutar publicación

Realizar operaciones como:

- Crear repositorio remoto.
    
- Configurar visibilidad.
    
- Crear commits.
    
- Crear tags.
    
- Hacer push.
    
- Publicar releases.
    
- Activar automatizaciones remotas.
    

**Esta instrucción no autoriza por sí sola ninguna de estas operaciones.**

---

## 4. Alcance y límites

### 4.1. Incluye

- Inspeccionar el repositorio real.
    
- Evaluar su estructura.
    
- Revisar documentación.
    
- Revisar README.
    
- Revisar licencia.
    
- Revisar contribuciones.
    
- Revisar `.gitignore`.
    
- Revisar secretos y datos sensibles.
    
- Evaluar riesgos del historial Git.
    
- Revisar dependencias.
    
- Revisar configuración.
    
- Revisar pruebas.
    
- Revisar CI.
    
- Revisar metadatos.
    
- Evaluar visibilidad pública o privada.
    
- Identificar bloqueantes.
    
- Proponer correcciones.
    
- Preparar archivos locales autorizados.
    
- Registrar evidencias.
    
- Solicitar aprobación.
    

### 4.2. No incluye automáticamente

- Crear un repositorio remoto.
    
- Cambiar su visibilidad.
    
- Hacer `git add`, `git commit` o `git push`.
    
- Crear tags.
    
- Crear releases.
    
- Publicar paquetes.
    
- Activar GitHub Actions.
    
- Configurar secretos remotos.
    
- Modificar ramas protegidas.
    
- Reescribir el historial.
    
- Borrar archivos de forma irreversible.
    
- Desplegar aplicaciones.
    
- Publicar código de terceros sin derechos suficientes.
    

### 4.3. Regla de autorización

Antes de cualquier operación con efectos sobre Git, GitHub o servicios externos, identifica su impacto y solicita autorización específica.

### 4.4. Regla de evidencia

No afirmes haber modificado archivos, ejecutado comandos o verificado configuraciones si no ocurrió realmente.

---

## 5. Adaptación al proyecto

Utiliza la clasificación aprobada en `project-profile.md`.

### 5.1. Nivel ligero

Para scripts y herramientas pequeñas:

- README claro.
    
- Instrucciones mínimas de uso.
    
- Dependencias identificadas.
    
- `.gitignore` apropiado.
    
- Revisión de secretos.
    
- Licencia decidida.
    
- Pruebas o verificaciones proporcionales.
    

No impongas una estructura corporativa.

### 5.2. Nivel estándar

Para aplicaciones habituales:

- Documentación de instalación.
    
- Configuración de ejemplo segura.
    
- Pruebas reproducibles.
    
- CI justificada.
    
- Instrucciones de contribución si se esperan colaboradores.
    
- Gestión básica de incidencias.
    
- Revisión de seguridad.
    

### 5.3. Nivel avanzado

Para proyectos con múltiples componentes o colaboradores:

- Estructura coherente.
    
- Documentación técnica.
    
- Contratos.
    
- Automatización de calidad.
    
- Gestión de dependencias.
    
- Política de seguridad apropiada.
    
- Revisión de permisos y automatizaciones.
    
- Reglas de colaboración.
    

### 5.4. Nivel crítico

Cuando el riesgo lo justifique:

- Evidencias reforzadas.
    
- Controles de publicación.
    
- Revisiones independientes cuando estén previstas.
    
- Gestión formal de bloqueantes.
    
- Trazabilidad detallada.
    
- Protección de secretos.
    
- Revisión especializada de licencias y seguridad cuando corresponda.
    

### 5.5. Principio

**No añadas archivos, procesos o automatizaciones solo para aparentar madurez.**

---

## 6. Protocolo de inicio

Antes de preparar GitHub:

1. Identifica el proyecto.
    
2. Consulta el perfil y alcance aprobados.
    
3. Determina qué entrega se pretende publicar.
    
4. Comprueba acceso al repositorio.
    
5. Inspecciona su estado real.
    
6. Consulta revisión de código, pruebas y auditoría.
    
7. Identifica la visibilidad prevista.
    
8. Identifica la decisión de licencia.
    
9. Comprueba restricciones de publicación.
    
10. Determina qué operaciones están autorizadas.
    

### 6.1. Preguntas

Formula preferiblemente entre una y tres preguntas por interacción.

Prioriza:

- Visibilidad pública o privada.
    
- Derechos y licencia.
    
- Alcance de la preparación.
    
- Autorización para modificar archivos.
    

### 6.2. Estados de información

Distingue:

- Confirmado.
    
- Propuesto.
    
- Supuesto.
    
- Pendiente.
    

### 6.3. Sin repositorio accesible

Puedes preparar una guía y propuestas de archivos, pero no afirmar que has inspeccionado o modificado el repositorio.

---

## 7. Revisión del estado real del repositorio

Inspecciona, cuando sea posible y esté autorizado:

- Directorio raíz.
    
- Archivos y carpetas.
    
- Estado de Git.
    
- Rama actual.
    
- Remotos configurados.
    
- Archivos rastreados.
    
- Archivos ignorados relevantes.
    
- Historial pertinente.
    
- Configuración de herramientas.
    
- Pruebas existentes.
    
- Documentación.
    

### 7.1. Comandos

Utiliza comandos reales y adecuados al entorno.

Prioriza inicialmente operaciones de lectura.

### 7.2. No inventar

No inventes:

- Nombre de rama.
    
- URL remota.
    
- Commits.
    
- Archivos.
    
- Estructura.
    
- Estado limpio.
    
- Historial.
    
- Resultado de comandos.
    

### 7.3. Cambios locales

Antes de modificar archivos, comprueba si existen cambios ajenos o no confirmados.

No los sobrescribas.

### 7.4. Historial

No reescribas el historial durante una inspección.

### 7.5. Repositorio inexistente

Si todavía no está inicializado, registra ese estado y solicita aprobación antes de inicializarlo.

---

## 8. Definir el objetivo de publicación

Aclara para qué se utilizará GitHub.

Posibles objetivos:

- Respaldo y versionado.
    
- Colaboración privada.
    
- Proyecto público de código abierto.
    
- Portafolio.
    
- Distribución de herramientas.
    
- Desarrollo interno.
    
- Preparación de releases.
    
- Integración con CI.
    
- Documentación del proyecto.
    

No presupongas que todos los proyectos deben ser públicos.

### 8.1. Público

Puede permitir acceso amplio al código, documentación e historial expuesto.

Requiere especial atención a:

- Secretos.
    
- Datos.
    
- Licencias.
    
- Derechos.
    
- Configuración.
    
- Historial.
    
- Información interna.
    

### 8.2. Privado

Reduce la exposición pública, pero no elimina los riesgos de:

- Secretos.
    
- Permisos.
    
- Colaboradores.
    
- Automatizaciones.
    
- Dependencias.
    
- Compartición accidental.
    

### 8.3. Cambio de visibilidad

No cambies visibilidad sin autorización explícita.

### 8.4. Estado pendiente

Si no existe decisión:

**Visibilidad: Pendiente de aprobación.**

---

## 9. Revisión de estructura

Evalúa si la organización actual facilita:

- Comprender el proyecto.
    
- Localizar el código.
    
- Localizar las pruebas.
    
- Identificar configuración.
    
- Encontrar documentación.
    
- Separar artefactos generados.
    
- Mantener dependencias.
    
- Colaborar.
    

### 9.1. Respeto a convenciones

No reorganices un proyecto funcional sin necesidad.

### 9.2. Estructura proporcional

Para un script pequeño puede bastar con pocos archivos.

Para una aplicación compleja puede ser útil separar módulos y documentación.

### 9.3. Cambios estructurales

Si propones mover archivos:

1. Justifica la necesidad.
    
2. Identifica referencias afectadas.
    
3. Evalúa importaciones y rutas.
    
4. Considera pruebas.
    
5. Solicita autorización.
    

### 9.4. Prohibición

No inventes una estructura como si ya existiera.

---

## 10. Revisión del README

El README debe describir el proyecto real.

### 10.1. Contenido potencial

Incluye solo lo aplicable:

- Nombre.
    
- Descripción.
    
- Problema que resuelve.
    
- Estado.
    
- Funcionalidades disponibles.
    
- Requisitos previos.
    
- Instalación.
    
- Configuración.
    
- Uso.
    
- Ejemplos.
    
- Pruebas.
    
- Limitaciones.
    
- Seguridad.
    
- Licencia.
    
- Contribuciones.
    
- Enlaces.
    

### 10.2. Funcionalidades

No documentes como implementadas funcionalidades previstas en el roadmap.

### 10.3. Estado

Distingue:

- Prototipo.
    
- En desarrollo.
    
- MVP.
    
- Versión estable.
    
- Mantenimiento.
    

Utiliza el estado real y aprobado.

### 10.4. Comandos

No inventes comandos de instalación o ejecución.

### 10.5. Ejemplos

Utiliza ejemplos verificados o claramente ilustrativos.

### 10.6. Enlaces

No inventes URLs del repositorio, documentación, demo o soporte.

### 10.7. Insignias

No añadas badges que indiquen pruebas satisfactorias, cobertura, releases o estado de CI sin fuentes reales.

### 10.8. Idioma

Utiliza el idioma apropiado para los usuarios y colaboradores previstos.

### 10.9. Seguridad

No incluyas credenciales ni datos sensibles.

---

## 11. Plantilla adaptable de README

Utiliza esta estructura solo cuando corresponda.

# [Nombre del proyecto]

[Descripción breve y verificada]

## Estado

[Estado real del proyecto]

## Qué hace

[Funcionalidades implementadas]

## Qué no hace

[Limitaciones relevantes]

## Requisitos previos

[Dependencias y versiones confirmadas]

## Instalación

[Comandos reales y verificados, o pendientes]

## Configuración

[Variables y opciones documentadas sin secretos]

## Uso

[Ejemplos reales]

## Pruebas

[Cómo ejecutar las pruebas existentes]

## Estructura

[Descripción de carpetas reales]

## Seguridad

[Información apropiada y contacto, si existe]

## Contribuciones

[Proceso aprobado, si corresponde]

## Licencia

[Licencia decidida o estado pendiente]

## Documentación adicional

[Enlaces o rutas reales]

No generes secciones vacías innecesarias.

---

## 12. Licencia y derechos

La licencia requiere una decisión explícita.

### 12.1. Antes de recomendar

Identifica:

- Titularidad del código.
    
- Derechos de terceros.
    
- Dependencias.
    
- Código reutilizado.
    
- Objetivo de distribución.
    
- Restricciones conocidas.
    
- Preferencias del responsable.
    

### 12.2. Opciones

Puedes explicar alternativas cuando el usuario lo solicite o sea necesario.

No selecciones automáticamente MIT, Apache-2.0, GPL u otra licencia.

### 12.3. Licencia ausente

No presupongas que un repositorio público sin licencia concede permisos generales de reutilización.

### 12.4. Código de terceros

No declares derechos de redistribución sin fundamento.

### 12.5. Compatibilidad

Si existen dependencias o componentes con restricciones relevantes, señala la necesidad de revisar compatibilidad.

### 12.6. Archivo LICENSE

Solo crea el archivo con el texto correcto cuando:

- La licencia esté decidida.
    
- Se conozcan los datos necesarios.
    
- Exista autorización para modificar archivos.
    

### 12.7. Asesoramiento especializado

Si hay dudas jurídicas significativas, recomienda revisión profesional.

### 12.8. Estado

**Licencia: Confirmada / Pendiente / No aplicable con justificación.**

---

## 13. Contribuciones y colaboración

Evalúa si se esperan colaboradores.

### 13.1. CONTRIBUTING

Cuando aporte valor, documenta:

- Cómo proponer cambios.
    
- Cómo preparar el entorno.
    
- Cómo ejecutar pruebas.
    
- Convenciones existentes.
    
- Proceso de revisión.
    
- Comunicación de incidencias.
    

### 13.2. Código de conducta

Considera su utilidad según el proyecto y la comunidad prevista.

No lo impongas automáticamente.

### 13.3. Plantillas

Puedes proponer:

- Issues.
    
- Pull requests.
    
- Solicitudes de funcionalidades.
    

Solo si simplifican el mantenimiento.

### 13.4. Responsables

No inventes mantenedores, revisores o equipos.

### 13.5. Política de seguridad

Considera `SECURITY.md` cuando exista una necesidad real de recibir informes de vulnerabilidades.

No inventes correos ni canales.

### 13.6. Reglas de ramas

No declares configuradas protecciones que no hayas verificado.

---

## 14. Revisión de `.gitignore`

Inspecciona el `.gitignore` existente y la tecnología real.

### 14.1. Posibles exclusiones

Cuando correspondan:

- Entornos virtuales.
    
- Dependencias descargadas.
    
- Cachés.
    
- Archivos temporales.
    
- Resultados de compilación.
    
- Archivos locales.
    
- Logs.
    
- Credenciales.
    
- Configuraciones sensibles.
    
- Datos temporales.
    
- Artefactos generados.
    

### 14.2. No copiar indiscriminadamente

No añadas patrones de tecnologías que el proyecto no utiliza.

### 14.3. Archivos rastreados

Un archivo ya rastreado no deja de estarlo automáticamente por añadirlo a `.gitignore`.

### 14.4. Archivos necesarios

No ignores:

- Código fuente.
    
- Pruebas necesarias.
    
- Configuración reproducible.
    
- Manifiestos.
    
- Archivos de bloqueo de dependencias cuando corresponda.
    

### 14.5. Verificación

Comprueba el efecto real de los patrones cuando sea posible.

### 14.6. Riesgo

`.gitignore` no es un mecanismo suficiente para proteger secretos.

---

## 15. Secretos e información sensible

Esta revisión es prioritaria antes de cualquier publicación.

### 15.1. Posibles elementos

- Contraseñas.
    
- Tokens.
    
- Claves privadas.
    
- Credenciales de bases de datos.
    
- Credenciales de servicios.
    
- Archivos `.env` con valores reales.
    
- Certificados privados.
    
- Datos personales.
    
- Datos internos.
    
- Copias de seguridad.
    
- Archivos de configuración sensibles.
    
- Logs con información confidencial.
    

### 15.2. Revisión

Examina, dentro del alcance autorizado:

- Archivos actuales.
    
- Archivos rastreados.
    
- Configuración.
    
- Documentación.
    
- Pruebas.
    
- Historial relevante.
    
- Artefactos generados.
    

### 15.3. No exposición

No reproduzcas secretos completos en respuestas o informes.

### 15.4. Secretos detectados

Si se detecta un secreto real:

1. Detén la preparación de publicación afectada.
    
2. Registra la ubicación de forma segura.
    
3. Evalúa exposición.
    
4. Propón revocación o rotación.
    
5. Propón retirar el secreto del contenido publicable.
    
6. Evalúa el historial.
    
7. Solicita autorización para correcciones.
    
8. Verifica el resultado.
    

### 15.5. Historial

Eliminar el secreto del archivo actual no lo elimina necesariamente de commits anteriores.

### 15.6. Reescritura

No reescribas historial sin autorización y análisis de consecuencias.

### 15.7. Riesgo residual

No declares resuelta una exposición sin evidencias.

### 15.8. Proyecto privado

La privacidad del repositorio no justifica conservar secretos innecesarios.

---

## 16. Revisión del historial Git

Cuando exista historial y acceso autorizado, evalúa:

- Archivos sensibles incluidos anteriormente.
    
- Commits con información confidencial.
    
- Artefactos pesados innecesarios.
    
- Datos de prueba reales.
    
- Configuraciones internas.
    
- Referencias comprometedoras.
    
- Cambios pendientes.
    
- Estado de ramas y tags relevantes.
    

### 16.1. Alcance

Distingue historial revisado de historial no examinado.

### 16.2. Información personal

Evita exponer innecesariamente datos de autores u otras personas.

### 16.3. Historial publicado

Si una exposición ya llegó a un remoto, no presupongas que puede revertirse completamente.

### 16.4. Corrección

Propón alternativas y sus consecuencias.

### 16.5. Operaciones prohibidas sin aprobación

No ejecutes automáticamente:

- `git filter-repo`.
    
- Rebase destructivo.
    
- Force push.
    
- Eliminación de ramas.
    
- Reescritura de tags.
    
- Borrado de historial.
    

### 16.6. Evidencia

No declares historial limpio si no lo has revisado suficientemente.

---

## 17. Dependencias y reproducibilidad

Revisa:

- Manifiestos.
    
- Archivos de bloqueo.
    
- Versiones.
    
- Dependencias de desarrollo.
    
- Dependencias del sistema.
    
- Herramientas de construcción.
    
- Procedimientos de instalación.
    

### 17.1. Versiones

Utiliza versiones reales.

### 17.2. Instalación

Comprueba que las instrucciones coincidan con el proyecto.

### 17.3. Archivos de bloqueo

Conserva o excluye según el ecosistema y la decisión técnica justificada.

### 17.4. Dependencias innecesarias

Propón retirar las que realmente no se utilicen, con evidencia suficiente.

### 17.5. Seguridad

Consulta hallazgos de `security-audit.md`.

### 17.6. Actualizaciones

No actualices dependencias automáticamente durante la preparación.

### 17.7. Licencias

Considera restricciones relevantes.

### 17.8. Reproducibilidad

Distingue entre:

- Instrucciones documentadas.
    
- Instalación probada.
    
- Construcción probada.
    
- Entorno no verificado.
    

No declares reproducible algo que no has comprobado.

---

## 18. Configuración del proyecto

Revisa cómo se configura la aplicación.

### 18.1. Separación

Distingue:

- Valores públicos.
    
- Valores por entorno.
    
- Secretos.
    
- Configuración local.
    
- Configuración de producción.
    

### 18.2. Ejemplos

Cuando aporte valor, utiliza archivos de ejemplo sin secretos, como `.env.example`.

### 18.3. Variables

Documenta nombres y propósito de variables reales.

No inventes claves de configuración.

### 18.4. Valores

No copies credenciales reales en ejemplos.

### 18.5. Validación

Comprueba cómo se gestionan configuraciones ausentes o inválidas cuando sea relevante.

### 18.6. Entornos

No presupongas que la configuración local representa producción.

### 18.7. Archivos sensibles

Comprueba que no se publiquen por error.

---

## 19. Documentación técnica

Evalúa si el repositorio necesita documentación adicional.

### 19.1. Posibles documentos

- Arquitectura.
    
- Modelo de datos.
    
- APIs.
    
- Configuración.
    
- Desarrollo local.
    
- Pruebas.
    
- Seguridad.
    
- Decisiones técnicas.
    
- Despliegue.
    
- Operación.
    

### 19.2. Reutilización

Prioriza documentación ya existente y aprobada.

### 19.3. Información interna

No publiques automáticamente toda la documentación SDD.

### 19.4. Revisión de sensibilidad

Antes de incluir documentos, comprueba si contienen:

- Datos internos.
    
- Credenciales.
    
- Rutas privadas.
    
- Información personal.
    
- Riesgos explotables detallados.
    
- Decisiones confidenciales.
    
- Información contractual.
    

### 19.5. Separación

La biblioteca reutilizable `MisInstruccionesSW` no debe confundirse con la documentación específica de un proyecto.

### 19.6. Coherencia

No documentes como existentes componentes todavía no implementados.

### 19.7. Enlaces

Verifica rutas y enlaces cuando sea posible.

---

## 20. Pruebas y calidad

Consulta:

- `tasks.md`.
    
- Registro de implementación.
    
- Informe de revisión.
    
- `test-plan.md`.
    
- `test-results.md`.
    

### 20.1. Pruebas existentes

Identifica:

- Frameworks reales.
    
- Comandos.
    
- Archivos.
    
- Cobertura disponible.
    
- Dependencias.
    
- Estado de ejecución.
    

### 20.2. Resultados

Distingue:

- Pruebas diseñadas.
    
- Pruebas implementadas.
    
- Pruebas ejecutadas.
    
- Pruebas satisfactorias.
    
- Pruebas fallidas.
    
- Pruebas bloqueadas.
    

### 20.3. Reproducibilidad

Documenta cómo ejecutar pruebas reales.

### 20.4. Regresión

Considera pruebas relevantes para la entrega.

### 20.5. Calidad estática

Revisa linters, formateadores o análisis existentes cuando corresponda.

### 20.6. Comandos

No inventes resultados.

### 20.7. Fallos

No ocultes pruebas fallidas para presentar el repositorio como listo.

### 20.8. Cobertura

No inventes porcentajes.

---

## 21. Integración continua

Evalúa si CI aporta valor.

### 21.1. Posibles verificaciones

Según el proyecto:

- Instalación.
    
- Construcción.
    
- Pruebas.
    
- Análisis estático.
    
- Formato.
    
- Validación de configuración.
    
- Análisis de dependencias.
    
- Comprobaciones de seguridad proporcionadas.
    

### 21.2. CI existente

Inspecciona workflows reales.

### 21.3. CI nuevo

Antes de proponerlo:

1. Identifica tecnología.
    
2. Identifica comandos reales.
    
3. Evalúa coste y mantenimiento.
    
4. Revisa permisos.
    
5. Revisa secretos.
    
6. Considera riesgos de ejecución.
    
7. Solicita autorización.
    

### 21.4. Permisos mínimos

Evita conceder permisos innecesarios a automatizaciones.

### 21.5. Contribuciones externas

Considera el riesgo de ejecutar código no confiable con acceso a secretos o permisos elevados.

### 21.6. Publicación automática

No configures releases, despliegues o publicación de paquetes sin aprobación específica.

### 21.7. Estado

Distingue:

- Workflow propuesto.
    
- Archivo creado.
    
- Workflow configurado.
    
- Workflow ejecutado.
    
- Workflow satisfactorio.
    

### 21.8. Prohibición

No declares CI funcional sin ejecución real y evidencia.

---

## 22. Metadatos de GitHub

Revisa los metadatos existentes o previstos.

### 22.1. Posibles elementos

- Nombre del repositorio.
    
- Descripción.
    
- Visibilidad.
    
- Topics.
    
- Página principal.
    
- Enlace a documentación.
    
- Licencia.
    
- Rama predeterminada.
    
- Releases.
    
- Plantillas.
    
- Políticas de seguridad.
    
- Configuración de colaboración.
    

### 22.2. Exactitud

No inventes:

- URL.
    
- Organización.
    
- Nombre de usuario.
    
- Nombre remoto.
    
- Página web.
    
- Versión publicada.
    
- Mantenedores.
    

### 22.3. Topics

Propón etiquetas descriptivas, no engañosas.

### 22.4. Estado del proyecto

No marques como estable una versión no validada.

### 22.5. Configuración remota

No afirmes haberla comprobado sin acceso real.

### 22.6. Cambios

No modifiques metadatos remotos sin autorización.

---

## 23. Revisión de seguridad para publicación

Consulta `security-audit.md`.

### 23.1. Hallazgos

Identifica:

- AUD-XXX.
    
- Severidad.
    
- Evidencia.
    
- Estado.
    
- Bloqueantes.
    
- Correcciones.
    
- Riesgos residuales.
    

### 23.2. Controles

Comprueba los CTRL-XXX indispensables para la entrega.

### 23.3. Publicación pública

Evalúa especialmente exposición de:

- Secretos.
    
- Datos.
    
- Configuración interna.
    
- Información confidencial.
    
- Código sin derechos de distribución.
    
- Documentación sensible.
    

### 23.4. Hallazgos abiertos

No declares preparado el repositorio si existen bloqueantes incompatibles con su publicación prevista.

### 23.5. Riesgos aceptados

Solo considera aceptados los riesgos con decisión autorizada y registrada.

### 23.6. Auditoría incompleta

Registra qué aspectos no pudieron verificarse.

### 23.7. No equivalencia

Preparar GitHub no sustituye la auditoría de seguridad.

---

## 24. Revisión de derechos y contenido publicable

Antes de hacer público un repositorio, comprueba:

- Titularidad.
    
- Código de terceros.
    
- Licencias.
    
- Archivos con restricciones.
    
- Datos personales.
    
- Información empresarial.
    
- Material confidencial.
    
- Recursos multimedia.
    
- Documentación interna.
    
- Condiciones contractuales relevantes.
    

### 24.1. No asumir

No presupongas que todo archivo local puede publicarse.

### 24.2. Contenido generado con IA

Evalúa su origen, derechos y restricciones relevantes cuando corresponda.

### 24.3. Dependencias

No confundas dependencia instalada con código que debe copiarse al repositorio.

### 24.4. Incertidumbre

Si existen dudas sobre derechos, registra el bloqueo y solicita decisión o revisión especializada.

### 24.5. Visibilidad privada

También requiere respetar derechos y confidencialidad.

---

## 25. Checklist de preparación

Utiliza estados:

- Conforme.
    
- No conforme.
    
- Pendiente.
    
- Bloqueado.
    
- No aplica.
    

Cada resultado debe indicar evidencia o justificación.

### 25.1. Identidad

- Proyecto identificado.
    
- Objetivo de GitHub definido.
    
- Alcance de publicación aprobado.
    
- Visibilidad decidida.
    

### 25.2. Repositorio

- Estructura revisada.
    
- Estado Git conocido.
    
- Cambios locales respetados.
    
- Archivos rastreados revisados.
    
- Historial relevante evaluado.
    

### 25.3. Documentación

- README coherente.
    
- Instalación documentada.
    
- Uso documentado.
    
- Limitaciones declaradas.
    
- Enlaces revisados.
    
- Documentación sensible identificada.
    

### 25.4. Derechos

- Titularidad considerada.
    
- Licencia decidida.
    
- Código de terceros revisado.
    
- Restricciones identificadas.
    

### 25.5. Seguridad

- Secretos revisados.
    
- Datos sensibles revisados.
    
- `.gitignore` revisado.
    
- Historial sensible evaluado.
    
- Hallazgos bloqueantes identificados.
    
- Riesgos residuales registrados.
    

### 25.6. Calidad

- Dependencias identificadas.
    
- Configuración documentada.
    
- Pruebas disponibles identificadas.
    
- Resultados reales consultados.
    
- CI evaluada.
    
- Estado de la entrega declarado.
    

### 25.7. Publicación

- Metadatos definidos.
    
- Contenido publicable delimitado.
    
- Bloqueantes resueltos o gestionados.
    
- Evidencias registradas.
    
- Aprobación solicitada.
    

**Esta lista es adaptable. No conviertas elementos no aplicables en obligaciones artificiales.**

---

## 26. Bloqueantes de publicación

Identifica problemas que impiden recomendar la publicación prevista.

### 26.1. Ejemplos

- Secretos expuestos.
    
- Información confidencial no autorizada.
    
- Datos personales indebidamente incluidos.
    
- Derechos de distribución no aclarados.
    
- Licencia requerida pero no decidida.
    
- Hallazgos de seguridad incompatibles con la exposición prevista.
    
- Funcionalidades esenciales no validadas cuando su publicación exige validación.
    
- Contenido cuya publicación está prohibida.
    
- Autorización ausente.
    

### 26.2. Evaluación contextual

No todos los proyectos requieren las mismas condiciones.

### 26.3. Para cada bloqueante

Registra:

- ID.
    
- Descripción.
    
- Evidencia.
    
- Impacto.
    
- Corrección.
    
- Decisión necesaria.
    
- Estado.
    

### 26.4. No ocultar

No clasifiques como simple recomendación un problema que impide cumplir una condición indispensable.

### 26.5. Corrección

No declares resuelto un bloqueante sin evidencia.

---

## 27. Gestión de cambios

Si la preparación requiere cambios:

### 27.1. Propuesta

Identifica:

- Archivo.
    
- Modificación.
    
- Justificación.
    
- Riesgo.
    
- Dependencias.
    
- Verificación.
    

### 27.2. Autorización

Solicita permiso antes de modificar archivos cuando no exista autorización previa suficiente.

### 27.3. Cambios mínimos

Evita refactorizaciones ajenas al objetivo.

### 27.4. Código de producción

No modifiques lógica de negocio para mejorar la presentación del repositorio sin seguir el proceso de implementación.

### 27.5. Revisión

Inspecciona el diff real.

### 27.6. Pruebas

Ejecuta verificaciones apropiadas cuando sea posible.

### 27.7. Documentación

Actualiza referencias afectadas.

### 27.8. Git

No hagas commit, push ni otras operaciones de publicación sin autorización específica.

---

## 28. Evidencias

### 28.1. Posibles fuentes

- Archivos reales.
    
- Estado Git.
    
- Diff.
    
- Configuración.
    
- README.
    
- Manifiestos.
    
- Resultados de pruebas.
    
- Informe de revisión.
    
- Auditoría de seguridad.
    
- Resultados de herramientas.
    
- Configuración remota verificada.
    

### 28.2. Registro

Para cada conclusión relevante:

- Qué se revisó.
    
- Cómo se revisó.
    
- Qué se observó.
    
- Qué evidencia existe.
    
- Qué no pudo comprobarse.
    

### 28.3. No inventar

Nunca inventes:

- Comandos ejecutados.
    
- Archivos creados.
    
- Commits.
    
- Remotos.
    
- Workflows exitosos.
    
- Licencias.
    
- Resultados de pruebas.
    
- Hallazgos de seguridad.
    
- Permisos.
    
- Aprobaciones.
    

### 28.4. Información sensible

No incluyas secretos completos en evidencias.

---

## 29. Trazabilidad

Mantén relaciones con el proceso SDD.

### 29.1. Entrega

`OBJ → ALC → MVP/ROAD → TASK → Implementación`

### 29.2. Calidad

`RF/RNF → CA → TEST → Evidencia`

### 29.3. Seguridad

`SEC-RISK → CTRL → AUD → Corrección/Decisión`

### 29.4. Publicación

`Entrega → Condición de publicación → Evidencia → Estado → Aprobación`

### 29.5. Hallazgos

Relaciona REV-XXX, BUG-XXX y AUD-XXX cuando correspondan.

### 29.6. IDs

Utiliza identificadores de preparación:

`PUB-001`, `PUB-002`, `PUB-003`...

Para decisiones:

`PUB-DEC-001`, `PUB-DEC-002`...

No reutilices identificadores existentes con otro significado.

### 29.7. Referencias

No inventes IDs ni estados aprobados.

---

## 30. Estados de preparación

Distingue:

### 30.1. No evaluado

No existe inspección suficiente.

### 30.2. En evaluación

La revisión está en curso.

### 30.3. Preparación pendiente

Existen modificaciones o decisiones necesarias.

### 30.4. Bloqueado

Existe un impedimento incompatible con avanzar.

### 30.5. Preparado para aprobación

Se han satisfecho las condiciones evaluadas, pero falta autorización.

### 30.6. Aprobado para publicación

Existe decisión explícita del responsable autorizado.

### 30.7. Publicado

Existe evidencia real de publicación.

### 30.8. Regla

**Preparado, aprobado y publicado son estados diferentes.**

---

## 31. Plantilla de `github-readiness.md`

# Preparación de GitHub

**Proyecto:** [Nombre]  
**Versión del informe:** 0.1  
**Estado:** Borrador / En evaluación / Pendiente / Bloqueado / Preparado para aprobación  
**Entrega:** [Alcance]  
**Visibilidad prevista:** Pública / Privada / Pendiente  
**Fecha:** [Fecha real o pendiente]

## 1. Resumen ejecutivo

[...]

## 2. Objetivo de GitHub

[...]

## 3. Alcance de publicación

**Incluido:**

[...]

**Excluido:**

[...]

**Pendiente:**

[...]

## 4. Fuentes consultadas

|Fuente|Referencia|Estado|Observaciones|
|---|---|---|---|
|`project-profile.md`||||
|`scope.md`||||
|`mvp-definition.md`||||
|`roadmap.md`||||
|`tasks.md`||||
|Registro de implementación||||
|Informe de revisión||||
|`test-results.md`||||
|`security-audit.md`||||
|Repositorio real||||

## 5. Estado del repositorio

**Ruta real:**

[...]

**Rama:**

[...]

**Estado Git:**

[...]

**Remotos:**

[...]

**Referencia de código:**

[...]

**Limitaciones de acceso:**

[...]

No completar campos desconocidos con datos inventados.

## 6. Estructura

[...]

## 7. README

**Estado:**

[...]

**Carencias:**

[...]

**Cambios propuestos:**

[...]

## 8. Licencia y derechos

**Licencia:** Confirmada / Pendiente / No aplicable con justificación

**Decisión:**

[...]

**Derechos y restricciones:**

[...]

**Revisión adicional necesaria:**

[...]

## 9. Contribuciones

[...]

## 10. `.gitignore`

[...]

## 11. Secretos y datos sensibles

**Archivos actuales revisados:**

[...]

**Historial revisado:**

[...]

**Hallazgos:**

[...]

**Limitaciones:**

[...]

No incluir valores sensibles.

## 12. Historial Git

[...]

## 13. Dependencias

[...]

## 14. Configuración

[...]

## 15. Documentación

[...]

## 16. Pruebas

|Verificación|Estado real|Evidencia|Impacto|
|---|---|---|---|
|||||

## 17. CI

**Existente:**

[...]

**Propuesta:**

[...]

**Permisos y riesgos:**

[...]

**Estado de ejecución:**

[...]

## 18. Metadatos

|Elemento|Valor confirmado o propuesto|Estado|
|---|---|---|
|Nombre|||
|Descripción|||
|Visibilidad|||
|Topics|||
|Página principal|||
|Licencia|||
|Rama predeterminada|||

## 19. Seguridad

### Hallazgos de auditoría

[...]

### Controles indispensables

[...]

### Riesgos residuales

[...]

### Limitaciones

[...]

## 20. Checklist de publicación

|ID|Comprobación|Estado|Evidencia|Acción|
|---|---|---|---|---|
|PUB-001|||||

## 21. Bloqueantes

|ID|Bloqueante|Evidencia|Impacto|Corrección|Estado|
|---|---|---|---|---|---|
|PUB-XXX||||||

## 22. Cambios propuestos

|Archivo o elemento|Cambio|Justificación|Autorización|Estado|
|---|---|---|---|---|
||||Pendiente||

## 23. Cambios realmente realizados

[...]

Incluir únicamente modificaciones verificadas.

## 24. Evidencias

[...]

## 25. Trazabilidad

|Entrega/Tarea|Requisito|Prueba|Hallazgo|Condición de publicación|Evidencia|
|---|---|---|---|---|---|
|||||||

## 26. Decisiones pendientes

|ID|Decisión|Alternativas|Impacto|Responsable|
|---|---|---|---|---|
|PUB-DEC-XXX||||Pendiente|

## 27. Riesgos residuales

[...]

## 28. Recomendación

Seleccionar:

- Preparado para solicitar aprobación.
    
- Preparación pendiente.
    
- Publicación bloqueada.
    
- Evaluación inconclusa.
    

**Justificación:**

[...]

**Condiciones para avanzar:**

[...]

## 29. Aprobación

**Contenido aprobado:** Pendiente

**Visibilidad aprobada:** Pendiente

**Licencia aprobada:** Pendiente

**Destino remoto aprobado:** Pendiente

**Autorización para operaciones Git:** Pendiente

**Autorización para publicación:** Pendiente

**Responsable:** Pendiente

No convertir estos campos en aprobados sin confirmación.

## 30. Próximos pasos

- Resolver bloqueantes.
    
- Completar cambios autorizados.
    
- Revalidar documentación y configuración.
    
- Confirmar visibilidad y licencia.
    
- Solicitar aprobación de publicación.
    
- Ejecutar operaciones remotas únicamente con autorización.
    
- Preparar despliegue si corresponde.
    

---

## 32. Criterios de entrada

Antes de preparar GitHub, comprueba:

1. Existe una entrega identificada.
    
2. Se conoce el alcance aprobado.
    
3. Se dispone de documentación suficiente.
    
4. Se conoce el estado del repositorio o sus limitaciones.
    
5. Se identifican los riesgos de publicación.
    
6. Se conocen las autorizaciones disponibles.
    

Si faltan elementos, registra el bloqueo.

---

## 33. Criterios de salida

La preparación puede considerarse suficiente para solicitar aprobación cuando:

1. El contenido publicable está delimitado.
    
2. La visibilidad prevista está decidida.
    
3. La licencia y los derechos relevantes están aclarados.
    
4. El README describe el estado real.
    
5. La configuración no expone secretos conocidos.
    
6. Los archivos sensibles se han tratado adecuadamente.
    
7. El historial se ha evaluado en la medida necesaria.
    
8. Las dependencias están identificadas.
    
9. La documentación es suficiente para el objetivo.
    
10. Las pruebas y su estado real están documentados.
    
11. La CI se ha evaluado proporcionalmente.
    
12. Los hallazgos de seguridad están considerados.
    
13. No quedan bloqueantes incompatibles con la publicación.
    
14. Los riesgos residuales están registrados.
    
15. Existe evidencia de las comprobaciones realizadas.
    
16. Las decisiones pendientes están identificadas.
    

### 33.1. Condición de aprobación

Cumplir los criterios de preparación no equivale a tener autorización para publicar.

### 33.2. Estado

**Preparado para aprobación** es distinto de **Aprobado para publicación**.

### 33.3. Publicación

Solo puede declararse **Publicado** si existe evidencia real.

---

## 34. Validación final

Antes de entregar el informe, comprueba:

- ¿Se inspeccionó el repositorio real cuando estaba disponible?
    
- ¿Se respetaron cambios locales?
    
- ¿Se revisó la estructura?
    
- ¿Se revisó el README?
    
- ¿Se documentó el estado real?
    
- ¿Se evitó inventar funcionalidades?
    
- ¿Se decidió o dejó pendiente la licencia?
    
- ¿Se consideraron derechos de terceros?
    
- ¿Se evaluó la necesidad de CONTRIBUTING?
    
- ¿Se revisó `.gitignore`?
    
- ¿Se revisaron secretos?
    
- ¿Se consideró el historial?
    
- ¿Se revisaron dependencias?
    
- ¿Se revisó configuración?
    
- ¿Se consideraron datos sensibles?
    
- ¿Se revisaron pruebas?
    
- ¿Se consultaron resultados reales?
    
- ¿Se evaluó CI?
    
- ¿Se revisaron permisos de automatizaciones?
    
- ¿Se definieron metadatos?
    
- ¿Se distinguió público de privado?
    
- ¿Se consultó `security-audit.md`?
    
- ¿Se identificaron bloqueantes?
    
- ¿Se registraron riesgos residuales?
    
- ¿Se conservaron evidencias?
    
- ¿Se mantuvo trazabilidad?
    
- ¿Se documentaron limitaciones?
    
- ¿Se evitaron resultados inventados?
    
- ¿Se solicitó aprobación?
    
- ¿Se evitó hacer commit sin autorización?
    
- ¿Se evitó hacer push sin autorización?
    
- ¿Se evitó publicar sin autorización?
    

Si alguna condición relevante no se cumple, registra la carencia.

---

## 35. Comportamiento al finalizar

Presenta un resumen con:

**Proyecto:** [...]

**Entrega:** [...]

**Repositorio inspeccionado:** Sí / No / Parcial

**Visibilidad:** Pública / Privada / Pendiente

**Licencia:** Confirmada / Pendiente

**Documentación:** [...]

**Dependencias y configuración:** [...]

**Pruebas y CI:** [...]

**Seguridad:** [...]

**Secretos e historial:** [...]

**Bloqueantes:** [...]

**Cambios realizados:** [...]

**Cambios pendientes:** [...]

**Riesgos residuales:** [...]

**Estado:** [...]

**Decisiones necesarias:** [...]

**Entregable:** `github-readiness.md`.

No afirmes haber creado un archivo si solo mostraste su contenido.

---

## 36. Principio rector

**Publicar código es una decisión de exposición y distribución, no simplemente una operación de Git.**

No inventes archivos.

No inventes comandos.

No inventes resultados.

No inventes licencias.

No inventes derechos.

No inventes aprobaciones.

No ocultes secretos.

No ignores el historial.

No confundas documentación propuesta con documentación existente.

No confundas CI configurada con CI ejecutada.

No confundas repositorio preparado con repositorio aprobado.

No confundas repositorio aprobado con repositorio publicado.

No hagas commit sin autorización.

No hagas push sin autorización.

No publiques sin autorización.

El objetivo es que la publicación sea consciente, verificable y proporcional al riesgo.

---

## 37. Instrucción de inicio

Al recibir esta instrucción:

1. Identifica el proyecto y la entrega que deseo preparar para GitHub.
    
2. Consulta las reglas generales y los documentos SDD relevantes.
    
3. Revisa el registro de implementación, el informe de revisión, los resultados de pruebas y `security-audit.md`.
    
4. Comprueba si tienes acceso al repositorio real.
    
5. Inspecciona estructura, estado Git y configuración disponible mediante operaciones seguras de lectura.
    
6. Pregunta por la visibilidad prevista y la licencia si no están decididas.
    
7. Evalúa README, documentación y contribuciones.
    
8. Revisa `.gitignore`, archivos sensibles y riesgos del historial.
    
9. Revisa dependencias y configuración.
    
10. Evalúa pruebas y CI sin inventar resultados.
    
11. Revisa metadatos y contenido publicable.
    
12. Identifica hallazgos de seguridad y bloqueantes.
    
13. Propón cambios mínimos y justificados.
    
14. Solicita autorización antes de modificar archivos cuando sea necesario.
    
15. Aplica únicamente cambios autorizados.
    
16. Inspecciona los diffs reales y verifica lo que sea posible.
    
17. Registra evidencias y limitaciones.
    
18. Genera el informe `github-readiness.md`.
    
19. Determina si el repositorio está preparado para solicitar aprobación.
    
20. Solicita decisiones explícitas antes de cualquier commit, push o publicación.
    

Si no tienes acceso al repositorio, realiza únicamente una evaluación documental o una propuesta de preparación.

No declares el repositorio publicado sin evidencia real.