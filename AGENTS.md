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

## Available Agent Skills & Toolkits
- **HOI4 Agent Tools MCP (`hoi4_agent_tools`):**
  - Integrated via MCP server (`hoi4-agent-tools.cmd`).
  - Provides offline focus tree rendering/linting, event chain inspections, scripted GUI previews, probability/weight analysis, and game documentation search.
- **Mod Diagnostics & Audit Scripts:**
  - `powershell -ExecutionPolicy Bypass -File .agents/skills/hoi4-review-debug/scripts/audit-hoi4-mod.ps1` (HOI4 Mod Doctor)
  - `powershell -ExecutionPolicy Bypass -File .agents/skills/hoi4-review-debug/scripts/analyze-hoi4-log.ps1` (Error log parser)
  - `powershell -ExecutionPolicy Bypass -File .agents/skills/hoi4-review-debug/scripts/audit-localisation.ps1` (Localisation format & key audit)
- **Agent Skills (`.agents/skills/`):**
  - `hoi4-modding`: Comprehensive syntax, scopes, effects, triggers, and templates across all HoI4 systems.
  - `hoi4-review-debug`: Mod Doctor diagnostics, error log analysis, and regression checks.
  - `hoi4-pdx-modding`: Paradox script language standards, lifecycle rules, and UTF-8 BOM encoding.
  - `hoi4-content-builder`: Structured workflows and kits for creating events, decisions, focuses, and ideas.
  - Modular skills: `hoi4-focus-trees`, `hoi4-events`, `hoi4-decisions-missions`, `hoi4-ideas-modifiers`, `hoi4-characters-leaders`, `hoi4-scripted-gui`, `hoi4-map-states`, `hoi4-super-events`.
- **Offline Wiki Reference (`.agents/references/paradox_wiki/`):**
  - Complete snapshot of Paradox Interactive HOI4 Wiki for fast, hallucination-free lookups.
