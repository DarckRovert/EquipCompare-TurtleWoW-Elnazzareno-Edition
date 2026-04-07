# 🛠️ Wiki: Guía de API — Instant Gear Comparison (EquipCompare)

EquipCompare expone métodos para que otros AddOns del ecosistema **Séquito del Terror** puedan disparar comparativas manuales.

## 📡 Funciones de Comparativa (Gear API)

### `EquipCompare_ShowCompare(itemID, equippedItemLink)`
Muestra forzosamente el tooltip comparativo para un objeto contra una pieza equipada específica.
- **`itemID`**: ID del objeto a comparar.
- **`equippedItemLink`**: Link del objeto ya equipado.

### `EquipCompare_IsEnabled()`
Verifica si el sistema de comparativa está activo globalmente.

## 📎 Integración con Ecosistema Gravity

- **Neural Loot Distribution**: **WCS_Brain** utiliza la API de EquipCompare para generar tooltips de comparativa instantánea cuando cae botín de un jefe de banda, agilizando la toma de decisiones del Séquito.
- **Stats Comparison**: **StatCompare** se ancla a los tooltips generados por EquipCompare para mostrar la diferencia numérica exacta de estadísticas (Fuerza, Agilidad, etc.) en tiempo real.

---
© 2026 **DarckRovert** — El Séquito del Terror.
*Ingeniería de equipo para la conquista de Azeroth.*
