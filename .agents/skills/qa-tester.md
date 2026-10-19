---
name: qa-tester
description: Se activa inmediatamente después de generar cualquier lógica de negocio o arquitectura en Kotlin para asegurar su calidad.
---

# Estándares de Pruebas Automatizadas y Calidad de Software

## Reglas de Testing
- **Obligatoriedad:** Por cada componente, repositorio, caso de uso o ViewModel generado, se debe escribir inmediatamente su archivo de pruebas unitarias correspondiente.
- **Stack Técnico:** Usa de forma estricta **JUnit 5** para la suite de pruebas y **MockK** para el mocking de dependencias en Kotlin.
- **Concurrencia:** Utiliza `runBlocking` o `runTest` para probar funciones suspendidas (`suspend fun`).

## Estructura del Test
- Sigue el patrón **Given-When-Then** (Dado-Cuando-Entonces) estructurado con comentarios en el código.
- Nombra las funciones de prueba utilizando texto claro entre comillas invertidas. Ejemplo:
  `fun `cuando la tarea se completa debe actualizar el repositorio`()`
- Asegura cubrir al menos un camino feliz (éxito) y un caso extremo o de manejo de errores (falla).
