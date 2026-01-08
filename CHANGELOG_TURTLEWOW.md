# EquipCompare TurtleWoW - Changelog

## Version 2.9.8-TW (January 2026)

### Author Information

**Modified by:** DarckRovert  
**In-Game Character:** Elnazzareno  
**Guild:** El Sequito del Terror  
**Server:** Turtle WoW  
**Date:** January 8, 2026  

### Overview

This version fixes Spanish (esES) localization issues that were causing errors on Turtle WoW when using the Spanish client.

---

## Changes in 2.9.8-TW

### 1. Spanish Localization Fixes

**File:** `localization.lua`

**Problem:**
The Spanish (esES) localization had incorrect or missing translation strings, causing Lua errors when the addon tried to access them.

**Solution:**
Corrected all Spanish translation strings to match the expected format and structure.

**Technical Details:**
- Fixed `EQUIPCOMPARE_CHAT_ENABLED` translation
- Fixed `EQUIPCOMPARE_CHAT_DISABLED` translation
- Fixed `EQUIPCOMPARE_CHAT_CONTROL_ON` translation
- Fixed `EQUIPCOMPARE_CHAT_CONTROL_OFF` translation
- Fixed `EQUIPCOMPARE_CHAT_CV_ON` translation
- Fixed `EQUIPCOMPARE_CHAT_CV_OFF` translation
- Fixed `EQUIPCOMPARE_CHAT_ALT_ON` translation
- Fixed `EQUIPCOMPARE_CHAT_ALT_OFF` translation
- Fixed `EQUIPCOMPARE_CHAT_SHIFT_ON` translation
- Fixed `EQUIPCOMPARE_CHAT_SHIFT_OFF` translation
- Fixed `EQUIPCOMPARE_CURRENTLY_EQUIPPED` translation

### 2. Addon Metadata Updates

**File:** `EquipCompare.toc`

**Changes:**
- Updated addon title to "EquipCompare TurtleWoW - Elnazzareno Edition"
- Updated version to 2.9.8-TW
- Added Turtle WoW credits metadata
- Updated all language-specific notes with Turtle WoW credits
- Added original author and version metadata

---

## Testing Procedure

### Test Environment
- **Server:** Turtle WoW
- **Client Language:** Spanish (esES)
- **WoW Version:** 1.12.1
- **Date:** January 8, 2026

### Tests Performed

1. **Addon Loading**
   - ✓ Addon loads without errors
   - ✓ No Lua errors in chat
   - ✓ Addon appears in addon list with correct name

2. **Functionality Tests**
   - ✓ Comparison tooltips appear when hovering over items
   - ✓ Tooltips show "Actualmente equipado" (Currently Equipped) in Spanish
   - ✓ Slash commands work correctly (/eqc, /equipcompare)
   - ✓ All configuration options work

3. **Localization Tests**
   - ✓ All Spanish strings display correctly
   - ✓ Chat messages appear in Spanish
   - ✓ No missing translation errors

### Test Results

**Status:** ✅ All tests passed  
**Errors Found:** None  
**Compatibility:** Fully compatible with Turtle WoW

---

## Future Maintenance

### Adding New Translations

If you need to add or modify translations in the future:

1. Open `localization.lua`
2. Find the language section (e.g., `if (GetLocale() == "esES") then`)
3. Add or modify the translation strings
4. Make sure all strings match the English (enUS) keys
5. Test in-game to verify

### Common Issues

- **Missing translations:** Always check that all keys from enUS exist in other languages
- **Typos in keys:** Variable names must match exactly (case-sensitive)
- **Special characters:** Use proper encoding for accented characters (á, é, í, ó, ú, ñ)

---

## Credits

### Original Addon

**Author:** Legorol  
**Email:** legorol@cosmosui.org  
**Version:** 2.9.8  
**License:** Public Domain

### Turtle WoW Fixes

**Modified by:** DarckRovert  
**Character:** Elnazzareno  
**Guild:** El Sequito del Terror  
**Server:** Turtle WoW  
**Date:** January 2026

---

*For Spanish documentation, see CREDITOS_ES.md*
*For general information, see README.md*
