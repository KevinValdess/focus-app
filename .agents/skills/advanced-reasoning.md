---
name: advanced-reasoning
description: Se activa al analizar requerimientos, imágenes de diseño visual o diagramas teóricos para desglosar la lógica de negocio antes de codificar.
---

# Habilidad de Razonamiento Avanzado y Modelado de Negocio

## Proceso de Análisis
Cuando el usuario entregue un diseño en papel, imagen o texto libre (como la app "Focus"):
1. **Identificar Entidades:** Extrae los objetos del mundo real (ej. Tarea, Grupo de Estudio, Pomodoro).
2. **Definir Estados:** Identifica los estados posibles de la interfaz (Cargando, Éxito, Error, Inactivo).
3. **Mapeo de UI a Datos:** Traduce los elementos visuales de la pantalla directamente a propiedades de Kotlin.

## Contrato de Salida
- Antes de arrojar código final, valida los impactos técnicos:
  - ¿Requiere permisos del sistema de Android? (ej. Servicios de accesibilidad para bloqueo de apps).
  - ¿Requiere concurrencia? (Asume siempre el uso de **Kotlin Coroutines** y **Flow/StateFlow** para flujos de datos reactivos).
