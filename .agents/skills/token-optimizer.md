---
name: token-optimizer
description: Se activa globalmente al inicio de cada interacción para formatear respuestas, eliminar redundancias y ahorrar contexto.
---

# Habilidad de Economía de Tokens y Orquestación

## Restricciones de Salida Estrictas
- **Prohibido:** Saludos, introducciones ("¡Hola!", "Entendido, aquí tienes..."), resúmenes o conclusiones teóricas.
- **Directo al grano:** Devuelve exclusivamente los bloques de código solicitados o respuestas estructuradas en Markdown/JSON.
- **Explicaciones:** Si se requiere documentación, agrégala de forma concisa como comentarios de código (`//`) dentro del mismo archivo generado.
- **Formato:** Usa bloques de código limpios especificando el lenguaje (ej. ```kotlin).

## Planificación Previa (Chain of Thought Acotado)
- Antes de escribir cualquier código complejo, genera un bloque de comentario superior de máximo 3 líneas desglosando el plan técnico. Ejemplo:
  // PLAN:
  // 1. Crear interfaz del Repositorio
  // 2. Implementar modelo inmutable
  // 3. Definir estados de la UI
