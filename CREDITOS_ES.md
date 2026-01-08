# EquipCompare TurtleWoW - Registro de Cambios

## Versión 2.9.8-TW (Enero 2026)

### Información del Autor

**Modificado por:** DarckRovert  
**Personaje en el Juego:** Elnazzareno  
**Clan:** El Sequito del Terror  
**Servidor:** Turtle WoW  
**Fecha:** 8 de Enero de 2026  

### Descripción General

Esta versión corrige problemas de localización en español (esES) que causaban errores en Turtle WoW cuando se usaba el cliente en español.

---

## Cambios en 2.9.8-TW

### 1. Correcciones de Localización en Español

**Archivo:** `localization.lua`

**Problema:**
La localización en español (esES) tenía cadenas de traducción incorrectas o faltantes, causando errores de Lua cuando el addon intentaba acceder a ellas.

**Solución:**
Se corrigieron todas las cadenas de traducción en español para que coincidan con el formato y estructura esperados.

**Detalles Técnicos:**
- Corregida traducción de `EQUIPCOMPARE_CHAT_ENABLED`
- Corregida traducción de `EQUIPCOMPARE_CHAT_DISABLED`
- Corregida traducción de `EQUIPCOMPARE_CHAT_CONTROL_ON`
- Corregida traducción de `EQUIPCOMPARE_CHAT_CONTROL_OFF`
- Corregida traducción de `EQUIPCOMPARE_CHAT_CV_ON`
- Corregida traducción de `EQUIPCOMPARE_CHAT_CV_OFF`
- Corregida traducción de `EQUIPCOMPARE_CHAT_ALT_ON`
- Corregida traducción de `EQUIPCOMPARE_CHAT_ALT_OFF`
- Corregida traducción de `EQUIPCOMPARE_CHAT_SHIFT_ON`
- Corregida traducción de `EQUIPCOMPARE_CHAT_SHIFT_OFF`
- Corregida traducción de `EQUIPCOMPARE_CURRENTLY_EQUIPPED`

### 2. Actualizaciones de Metadatos del Addon

**Archivo:** `EquipCompare.toc`

**Cambios:**
- Actualizado el título del addon a "EquipCompare TurtleWoW - Elnazzareno Edition"
- Actualizada la versión a 2.9.8-TW
- Añadidos metadatos de créditos de Turtle WoW
- Actualizadas todas las notas específicas de idioma con créditos de Turtle WoW
- Añadidos metadatos del autor original y versión

---

## Procedimiento de Pruebas

### Entorno de Pruebas
- **Servidor:** Turtle WoW
- **Idioma del Cliente:** Español (esES)
- **Versión de WoW:** 1.12.1
- **Fecha:** 8 de Enero de 2026

### Pruebas Realizadas

1. **Carga del Addon**
   - ✓ El addon carga sin errores
   - ✓ No hay errores de Lua en el chat
   - ✓ El addon aparece en la lista de addons con el nombre correcto

2. **Pruebas de Funcionalidad**
   - ✓ Los tooltips de comparación aparecen al pasar el cursor sobre objetos
   - ✓ Los tooltips muestran "Actualmente equipado" en español
   - ✓ Los comandos de barra funcionan correctamente (/eqc, /equipcompare)
   - ✓ Todas las opciones de configuración funcionan

3. **Pruebas de Localización**
   - ✓ Todas las cadenas en español se muestran correctamente
   - ✓ Los mensajes de chat aparecen en español
   - ✓ No hay errores de traducción faltante

### Resultados de las Pruebas

**Estado:** ✅ Todas las pruebas pasaron  
**Errores Encontrados:** Ninguno  
**Compatibilidad:** Totalmente compatible con Turtle WoW

---

## Mantenimiento Futuro

### Añadir Nuevas Traducciones

Si necesitas añadir o modificar traducciones en el futuro:

1. Abre `localization.lua`
2. Encuentra la sección de idioma (ej: `if (GetLocale() == "esES") then`)
3. Añade o modifica las cadenas de traducción
4. Asegúrate de que todas las cadenas coincidan con las claves del inglés (enUS)
5. Prueba en el juego para verificar

### Problemas Comunes

- **Traducciones faltantes:** Siempre verifica que todas las claves de enUS existan en otros idiomas
- **Errores tipográficos en claves:** Los nombres de variables deben coincidir exactamente (sensible a mayúsculas)
- **Caracteres especiales:** Usa la codificación adecuada para caracteres acentuados (á, é, í, ó, ú, ñ)

---

## Créditos

### Addon Original

**Autor:** Legorol  
**Email:** legorol@cosmosui.org  
**Versión:** 2.9.8  
**Licencia:** Dominio Público

### Correcciones para Turtle WoW

**Modificado por:** DarckRovert  
**Personaje:** Elnazzareno  
**Clan:** El Sequito del Terror  
**Servidor:** Turtle WoW  
**Fecha:** Enero 2026

---

## Agradecimientos

Gracias a la comunidad de Turtle WoW por mantener vivo el espíritu de Vanilla WoW y por proporcionar un servidor donde podemos disfrutar del juego clásico con mejoras y contenido adicional.

Gracias especiales a Legorol por crear este útil addon que hace que comparar equipo sea mucho más fácil.

---

*Para documentación en inglés, ver CHANGELOG_TURTLEWOW.md*  
*Para información general, ver README.md*
