# Arquitectura — EquipCompare Sequito 🏗️

mermaid
graph TD
    TOOLTIP[Game Tooltip]
    COMPARE[EquipCompare Engine]
    INV[Character Inventory]
    UI[Comparison Tooltip]

    TOOLTIP --> COMPARE
    INV --> COMPARE
    COMPARE --> UI


## Componentes
- **EquipCompare.lua**: Lógica de interceptación de tooltips y comparación de slots.
- **localization.lua**: Diccionarios de slots y estadísticas para la detección de equipo.
