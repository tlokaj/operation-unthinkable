# Project Guidelines — Operation Unthinkable (HoI4 Mod)

## Environment & Paths
- **Base Game Path (Reference Only — DO NOT MODIFY):** `C:\Program Files (x86)\Steam\steamapps\common\Hearts of Iron IV`
- **Target HoI4 Version:** `1.19.*` (`Operation Postern v1.19.3.0`)
- **Mod Root Directory:** `C:\Users\tloka\OneDrive\Documents\Paradox Interactive\Hearts of Iron IV\mod\operation_unthinkable`
- **Mod Registry File:** `C:\Users\tloka\OneDrive\Documents\Paradox Interactive\Hearts of Iron IV\mod\operation_unthinkable.mod`
- **Error Logs Location:** `C:\Users\tloka\OneDrive\Documents\Paradox Interactive\Hearts of Iron IV\logs\error.log`

## HoI4 Modding Technical Rules
1. **Localisation Files (`.yml`):**
   - MUST be placed in `localisation/english/` (or other language subfolder).
   - Filename MUST end with `_l_english.yml`.
   - File encoding **MUST be UTF-8 with BOM** (`EF BB BF`), otherwise HoI4 will silently ignore the file and display raw keys.
   - First line MUST be `l_english:`.
2. **Script Files (`.txt`, `.gui`, `.gfx`):**
   - Use standard UTF-8 (no BOM) for `.txt`, `.gui`, and `.gfx` files.
   - Always check bracket `{ }` balance in Paradox Clausewitz scripts.
3. **Namespace Prefix:**
   - Prefix custom events, decisions, ideas, and flags with `unthinkable_` to avoid collisions with vanilla HoI4 or DLC content.
