# ðŸ“ Wiki: Arquitectura 'Diamond Tier' â€” EquipCompare [v1.1.0]

Estructura tÃ©cnica de la comparativa de equipo mantenida por **DarckRovert**.

## ðŸ—ï¸ JerarquÃ­a del Sistema Tooltip Hub (Gear Hierarchy)

**EquipCompare** opera mediante la intercepciÃ³n del evento de muestra de informaciÃ³n de objetos:

1.  **Tooltip Hook (`EquipCompare.lua`)**: Ganchos en `GameTooltip:SetHyperlink` y `GameTooltip:SetBagItem` para detectar quÃ© objeto estÃ¡ viendo el usuario.
2.  **Slot Analyzer (`localization.lua`)**: LÃ³gica que determina el slot de equipo del objeto (ej: "Peto", "Anillo") para buscar la pieza equipada correspondiente.
3.  **Secondary Frame (`EquipCompare.xml`)**: El contenedor visual `EquipCompareTooltip` que se posiciona automÃ¡ticamente al lado del tooltip original.
4.  **Char-Sync (`CharactersViewer`)**: MÃ³dulo opcional para comparar con el equipo de otros personajes de la misma cuenta.

---

## ðŸ§­ Diagrama de Flujo: Comparativa de BiS v9.4

```mermaid
graph TD
    A[Inicio: Hover sobre Ãtem] --> B[Hook GameTooltip_OnShow]
    B --> C[ExtracciÃ³n de Slot de Hechizo/Ãtem]
    C --> D{Â¿Pieza Equipada?}
    D -- SÃ­ --> E[BÃºsqueda de Datos de ItemEquipped]
    E --> F[Carga de Tooltip Secundario Diamond Tier]
    F --> G[AlineaciÃ³n de Anclajes dinÃ¡micos]
    G --> H[Renderizado de EstadÃ­sticas Comparativas]
    D -- No --> I[Ocultar Frame Secundario]
    H --> J[Monitoreo de Cierre de Tooltip]
    J --> I
```

## âš¡ Estrategias de IngenierÃ­a Diamond Tier

- **Smart Anchoring**: EquipCompare v9.4 calcula la posiciÃ³n de la pantalla para que el tooltip comparativo nunca se salga de los lÃ­mites visibles, ajustando el anclaje a la izquierda o derecha segÃºn sea necesario.
- **Ring/Trinket Sequence**: Al comparar anillos o abalorios, EquipCompare puede ciclar entre ambos slots equipados para ofrecer una comparativa total de BiS.
- **Asynchronous Data Fetch**: La obtenciÃ³n de los datos del objeto equipado se realiza mediante punteros de memoria rÃ¡pidos del cliente 1.12.1 para evitar latencia visual.

---
Â© 2026 **DarckRovert** â€” El SÃ©quito del Terror.
*IngenierÃ­a de equipo para la conquista de Azeroth.*

