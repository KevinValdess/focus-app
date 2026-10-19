---
name: clean-code-kotlin
description: Se activa automáticamente cuando el usuario solicita codificar, refactorizar o definir arquitectura en Kotlin.
---

# Estándares de Arquitectura y Código Limpio para Kotlin

## Principios de Diseño
- **Inmutabilidad:** Usa `val` por defecto. Queda estrictamente prohibido el uso de `var` a menos que sea técnicamente indispensable. Prefiere colecciones inmutables (`List`, `Map`) sobre mutables.
- **Null Safety:** Explota el sistema de tipos de Kotlin. Prohibido usar el operador de aserción no nula (`!!`). Usa llamadas seguras (`?.`) y el operador Elvis (`?:`).
- **Arquitectura:** Sigue de forma estricta los patrones **MVVM** (Model-View-ViewModel) y **Clean Architecture** (separación nítida entre Capa de Dominio, Datos y UI).
- **Estructuras Modernas:** Usa `data class` para modelos de datos puros y `sealed class` o `sealed interface` para representar estados finitos de la pantalla.

## Expresiones Concisas
- Prioriza el uso de la estructura `when` como expresión.
- Utiliza funciones de alcance (`let`, `run`, `apply`, `also`) para mantener el código compacto y legible.
