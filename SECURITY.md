# Security Policy — Instant Gear Comparison (EquipCompare) 🔒🔎

Protegemos tu visualización de equipo en **Turtle WoW**.

## 🛡️ Soporte por Versión
| Versión | Estado |
| --- | --- |
| v9.4.x | ✅ Soportada |
| v9.3.x | ⚠️ Crítico |

## 🛡️ Reporte de Vulnerabilidades
Si descubres un bug que compromise la estabilidad del cliente de WoW durante la generación de tooltips duales o que cause cuídas de FPS al linkear objetos masivamente en el chat:

1.  **NO publique el exploit masivamente.**
2.  Reporta vía **Discord oficial** de **DarckRovert**.
3.  Incluye el log de `EquipCompare -> EquipCompare.lua`.

## 🛡️ Protecciones Integradas
- **UI Safety Hook**: El renderizado secundario de EquipCompare se libera automáticamente si el tooltip principal se cierra, evitando fugas de memoria (memory leaks).
- **ID Validation**: EquipCompare verifica que las IDs de los objetos sean legítimas antes de intentar generar una comparativa Diamond Tier.

---
© 2026 **DarckRovert** — El Séquito del Terror.
*Ingeniería de equipo segura para Azeroth.*
