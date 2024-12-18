# Guía Desarrollo de Software

## Investigación

- Definir objetivos: Metas concretas, medibles, alcanzables y relevantes.
- Identificar requisitos: Documentarlos de manera detallada
- Estimar los tiempos: Basandose en experiencias pasadas. Considerar márgenes para posibles imprevistos.
- Cronograma del proyecto: Dividir en fases claros, con fechas de entrega y puntos de revisión
- Evaluación de riesgos: Identificar riesgos (retrasos, cambios de requisitos, problemas técnicos...).
- Plan de contingencia: Para mitigar impacto de los potenciales riesgos.
- Selección de metodología de desarrollo: Agil, cascada, espiral o combinacion.
- Considerar el presupuesto: Asignar recursos financieros considerando todas las fases.
- Establecer plan de comunicación: Diseñar cómo será la comunicación con el cliente, para revisar progreso y resolver dudas.
- Definir los criterios de éxito y evaluación: Cómo se va a medir el éxito y qué métricas se van a usar para evaluar el progreso.
- Documentar proceso de planificación (en la memoria): mantener registro de decisiones, estrategias, acuerdos tomados en esta fase.
- Crear memoria de proyecto (documentación)

Esto tardará en torno a 1,5-2 semanas.

## Análisis

- Consultar y asegurar producto final que se desea
- Reuniones para captar requerimientos de forma detallada
- Priorizar requisitos: Usar técnicas coom MoSCoW para clasficar requisitos de más urgente a menos importante.
- Crear historias de usuario: Describe de qué manera un usuario final utiliza una app para lograr un resultado específico.
- Crear criterios de aceptación para cada requisito: Permite verificar que se ha cumplido correctamente. Especialmente importantes para las user stories.
- Crear diagrama ER u otro modelo más visual para visualizar lo que se busca. (C4)
- Identificar requisitos no funcionales (rendimiento, seguridad, disponibilidad, usabilidad, escalabilidad)
- Verificar y validar los requisitos: Reuniones para verificar que todo lo que el interesado quiere está definido como requisito.
- Documentar casos de uso y escenarios: Explica cómo interactuarán los usuarios con el sistema. Ayuda a comprender el flujo de trabajo desde la perspectiva del usuario.
- Realizar análisis de factibilidad (viabilidad técnica, financiera y de recursos para cumplir con los requisitos antes de comprometerse con ellos): Identifica restricciones que puedan afectar a la capacidad para cumplir con ciertos requisitos y ajusta expectativas en consecuencia.

Esto tardará en torno a 2 semanas.

## Diseño

- Definir arquitectura del sistema: por capas, microservicios, orientada a eventos... Considerar factores como escalabilidad, flexibilidad, rendimiento, mantenibilidad.
- Dividir sistema en módulos y componentes: Definir interfaces e interacciones entre módulos para asegurarse el desarrollo y pruebas de manera aislada.
- Crear diafragmas de diseño (modelo C4)
- Seleccionar stack apropiado y aprender previamente a usarlo: Tener en cuenta compatibilidad y escalabilidad de cada tecnología.
- Considerar requisitos no funcionales del análisis.
- Planificar la seguridad desde el diseño: Mecanismos de seguridad (autenticación, autorización, encriptación, manejo de errores seguros...) y análisis de amenazas.
- Diseñar para escalabilidad: El diseño soporta expansión del sistema a medida que crece en usuarios y/o funcionalidad.
- Evaluar y seleccionar patrones de diseño adecuados: Identificar patrones de diseño adecuados.
- Implementar estrategia de pruebas integrada en el diseño: Definir puntos de integració que permitan realizar pruebas de unidad, integración y sistema

Esto tardará en torno a 3 semanas.

## Desarrollo (Codificación)

- Definir estándares de codificación para que código sea consistente (convenciones, donde poner documentación, etc.)
- Pruebas unitarias: Para cada módulo o función clave. Automatizarlas tanto como sea posible. Emplear herramientas de pruebas continuas ayuda a encontrar errores.
- Implementar automatización (CI/CD)
- Programación modular: Módulos independientes para probar de manera aislada.
- Poner en calendario code reviews (esto se usa cuando el equipo es mayor): para detectar errores.
- Poner en calendario Refactorizaciones: Para reducir deuda técnica.
- Principios SOLID y OOP.
- Documentar código; funcionalidad y decisiones que hacen que sea así: Especialmente en áreas complejas o menos evidentes.
- Manejo de errores.
- Seguridad del código: Validación de entradas, gestión adecuada de autenticación y autorización y protección contra vulnerabilidades comunes (inyecciones SQL y XSS).
- Desarrollar en función de requisitos: Asegurar que el código cumple con requisitos definidos. Reduce probabilidad de que se necesiten correcciones después de implementación.
- Monitoreo del código en entornos de prueba: Pruebas exhaustivas en entorno de prueba que simule entorno de producción.

Esto tardará en torno a 2 meses.

## Pruebas (Testing)

- Definición de estrategia de pruebas clara: cubre integración, funcionales, de regresión, de rendimiento y de seguridad.
- Hacer pruebas con las stories creadas en el análisis.
- Automatizar pruebas repetitivas y de regresión.
- Realizar pruebas unitarias exhaustivas: cada unidad de código debe estar cubierta
- Ejecutar pruebas de integración: diferentes módulos y componentes del sistema funcionan bien juntos.
- Pruebas de Aceptación del Usuario.: El sistema cumple con las expectativas de los usuarios finales y funciona como esperan. La retroalimentación sirve para hacer ajustes finales.
- Pruebas de carga: Comportamiento del sistema bajo cargas intensas simulando múltiples usuarios simultáneos o grandes volúmenes de datos.
- Pruebas de Seguridad: Para identificar vulnerabilidades que puedan ser explotadas por ataques. Probar inyecciones SQL, ataques de fuerza bruta y acceso no autorizado.
- Pruebas de Regresión: Cuando se realizan cambios, hacer estas pruebas para asegurarse de que no introducen errores en otras partes del sistema.
- Pruebas de Compatibilidad: Distintos navegadores, distintos sitemas operativos, distintos dispositivos...
- Documentar errores encontrados. Usar herramienta de gestión de errores (JIRA o Bugzilla) para hacer seguimiento.
- Establecer criterios de aceptación para finalizar las pruebas: Indican cuando software está listo de ser desplegado.
- Análisis de resultados de pruebas y ajuste de plan de pruebas.

Esto tardará en torno a 3 semanas.

## Implementación (Despliegue)

- Planificar el despliegue: Definir estrategia de implementación clara que cubra el proceso de despliegue.
- Realizar una implementación de prueba: Con un entorno que imite el real
- Automatizar despliegue siempre que sea posible: CI/CD con Github Actions.
- Configurar monitoreo y alertas para entorno de producción.
- Preparar un rollback en caso de detectar fallos.
- Establecer canal de comunicación con usuarios finales y soporte.
- Realizar pruebas de validación en producción.
- Documentar proceso de implementación.
- Supervisar estabilidad post-despliegue.
- Recolectar feedback.
- Planificar un período de mantenimiento de post-implementación.
- Realizar evaluación post-implementación.

Esto tardará en torno a 2 semanas.

## Creación de tareas (Github Projects)

### 1. Usa Títulos Claros y Descriptivos

El título debe dar una idea clara de la tarea sin necesidad de abrirla.

Usa palabras clave, por ejemplo:

> Actualizar el formulario de registro
>
> Corregir error en autenticación

Si la tarea es para un bug, menciona el problema de forma explícita, por ejemplo:
> Error al enviar formulario en iOS

### 2. Describe el Contexto y los Objetivos Claramente

Explica qué problema resuelve o qué objetivo cumple la tarea.
Agrega contexto relevante, como en qué área del proyecto impacta o si tiene requisitos previos.
Si la tarea es técnica, incluye ejemplos de cómo se reproduce el problema o el resultado esperado.

### 3. Divide las Tareas en Pasos o Subtareas

Si la tarea es compleja, divídela en subtareas o pasos claros, por ejemplo:

```markdown
- [ ] Crear la vista del formulario
- [ ] Validar datos de entrada
- [ ] Conectar con la API
```

Esto ayuda a hacer el seguimiento del progreso y es útil para los revisores.

### 4. Agrega Criterios de Aceptación

Define claramente cuándo se considera que la tarea está completada. Por ejemplo:

> El formulario debe validar campos obligatorios.
>
> El usuario debe recibir un mensaje de error si el campo está vacío.

Esto ayuda a alinear expectativas y facilita las pruebas y revisiones.

### 5. Usa Etiquetas (Labels) para Clasificar la Tarea

Añade etiquetas como *bug*, *feature*, *enhancement*, *documentation*, *urgent*, *low-priority*, etc., para organizar y priorizar el trabajo.
Las etiquetas ayudan a filtrar tareas y entender de un vistazo qué tipo de trabajo hay pendiente.

### 6. Asigna a Personas y Agrega Fechas Límite (si son necesarias)

Asigna responsables para cada tarea para que quede claro quién está trabajando en qué.
Define fechas límite realistas en tareas críticas para asegurar que se cumplan a tiempo, pero evita poner fechas en exceso si no son necesarias, ya que puede crear presión innecesaria.

### 7. Adjunta Recursos Relevantes

Si la tarea requiere referencias a diseño, enlaces a documentación o archivos específicos, agrégalos en la descripción. Puedes adjuntar:

- Imágenes, capturas de pantalla.
- Documentos de especificaciones.
- Enlaces a archivos Figma, diseños, u otros recursos visuales.

### 8. Usa Plantillas para Estandarizar las Tareas

Puedes configurar plantillas de issues en GitHub para asegurarte de que todas las tareas tengan los mismos elementos clave.
Una plantilla básica puede incluir:

1. Descripción del problema.
2. Pasos para reproducir (si es un bug).
3. Criterios de aceptación.
4. Notas adicionales.

Las plantillas hacen que todos los miembros del equipo sigan una estructura consistente.

### 9. Mide y Prioriza la Tarea

Asigna una prioridad usando etiquetas o un sistema numérico (por ejemplo, Alta, Media, Baja).
Para tareas grandes, puedes hacer una estimación del esfuerzo en puntos, horas, o complejidad (1-5).
Establecer prioridad y tamaño ayuda a planificar el trabajo y a enfocar los esfuerzos en tareas que tienen mayor impacto.

### 10.  Involucra a los Colaboradores Desde el Inicio

Etiqueta o menciona a las personas relevantes para obtener retroalimentación o comentarios desde el principio.
Esto asegura que todos los que deben participar estén al tanto y puedan aportar ideas o corregir detalles de la tarea.

### 11.  Mantén la Tarea Actualizada y Ciérrala al Completarla

Si hay cambios en los requisitos o descubrimientos durante el desarrollo, actualiza la descripción de la tarea para reflejar el nuevo contexto.
Al terminar, cierra la tarea y, si es posible, agrega un comentario final que describa los cambios realizados o cualquier aspecto relevante.
