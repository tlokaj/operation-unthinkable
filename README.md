# Operation Unthinkable (1945) — Hearts of Iron IV Mod

Historický a alternativně-historický mod pro **Hearts of Iron IV (v1.19.\* Operation Postern)** zaměřený na **Operaci Unthinkable** – britský tajný plán Winstona Churchilla z května 1945 na překvapivou ofenzívu západních Spojenců proti Sovětskému svazu s cílem vynutit svobodné Polsko a nové uspořádání střední a východní Evropy.

## Umístění modu

- **Hlavní složka modu:** `C:\Users\tloka\OneDrive\Documents\Paradox Interactive\Hearts of Iron IV\mod\operation_unthinkable`
- **Zástupce ve Workspace:** `C:\Workspace\operation_unthinkable`
- **Launcher soubor:** `C:\Users\tloka\OneDrive\Documents\Paradox Interactive\Hearts of Iron IV\mod\operation_unthinkable.mod`
- **Instalace hry:** `C:\Program Files (x86)\Steam\steamapps\common\Hearts of Iron IV`

## Struktura projektu

- `descriptor.mod` – metadata modu pro Paradox Launcher (`supported_version="1.19.*"`)
- `common/`
  - `bookmarks/` – scénáře a startovní data (např. *1. červenec 1945 – Operation Unthinkable*)
  - `decisions/` & `decisions/categories/` – politická a vojenská rozhodnutí (znovuvyzbrojení Wehrmachtu, Polské ultimátum, příprava ofenzívy)
  - `ideas/` – národní duchové (*National Spirits*)
  - `national_focus/` – stromy národních zaměření (ENG, USA, SOV, POL, GER)
  - `on_actions/` – triggery po kapitulaci Německa / konferenci v Postupimi
- `events/` – řetězce událostí (`UnthinkableEvents.txt`)
- `history/` – úpravy států, zemí a jednotek (`countries/`, `states/`, `units/`)
- `gfx/` & `interface/` – ikony, portréty a definice GUI/ikon
- `localisation/english/` – lokalizační soubory (kódování **UTF-8 s BOM**)
