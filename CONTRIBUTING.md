# Contributing to EquipCompare (Gear Comparison) 🛡️🔎

¡Gracias por contribuir a la ingeniería de equipo del **Séquito del Terror**! Para mantener el estándar **Diamond Tier** de **DarckRovert**, todas las contribuciones deben centrarse en la velocidad de renderizado y la precisión de los tooltips duales.

---

## 🛡️ Estándares Técnicos (Comparison Core)

Este AddOn está optimizado para **Turtle WoW** (WoW v1.12.1). Las contribuciones DEBEN cumplir con:

1.  **Rendering Efficiency**: No introduzcas lógica pesada en `GameTooltip:OnShow`. La comparativa debe ser instantánea y no causar stuttering.
2.  **No Lua 5.1+**: El motor es Lua 5.0. Prohibido el operador `#` (usa `table.getn`).
3.  **Localization Tables**: Cualquier nueva cadena de texto debe añadirse a los archivos `localization.xx.lua` correspondientes. No realices hardcoding de cadenas en inglés en los scripts principales.
4.  **UI Harmony**: La visualización de los tooltips secundarios debe alinearse perfectamente con el estilo Diamond Tier de pfUI.

## 📐 Arquetipo de Desarrollo

Si deseas contribuir:
- **`EquipCompare.lua`**: Es el motor central de detección y anclaje de tooltips.
- **`localization.lua`**: Gestión de locales base y detección de slots de equipo.
- **`EquipCompare.xml`**: Define la estructura visual de los tooltips secundarios.

## 💎 Proceso de Pull Request

1.  **Fork & Branch**: Trabaja en ramas descriptivas (`fix/ring-swap`, `feature/trinket-compare`).
2.  **Documentación**: Actualiza `CHANGELOG.md` antes de enviar el PR.
3.  **Branding**: Mantén los enlaces institucionales oficiales de **DarckRovert**.

---
© 2026 **DarckRovert** — El Séquito del Terror.
*Ingeniería de equipo para la conquista de Azeroth.*
