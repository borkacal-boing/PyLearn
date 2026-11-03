# Python krok za krokem

Webová aplikace (PWA) na učení Pythonu od úplných základů na telefonu.

- 18 kapitol a 63 lekcí, každá s teorií a příklady
- 233 úloh ve třech obtížnostech (lehká, střední, těžká)
- automatická kontrola, nápovědy, vzorová řešení a české vysvětlení chyb
- Python běží přímo v prohlížeči díky [Pyodide](https://pyodide.org), nic se neodesílá na server
- postup se ukládá v prohlížeči

## Soubory

| Soubor | K čemu je |
|---|---|
| `index.html` | celá aplikace včetně lekcí a úloh |
| `manifest.webmanifest` | název, ikona a barvy aplikace pro instalaci na plochu |
| `sw.js` | service worker, díky kterému aplikace funguje i offline |
| `icon-*.png` | ikony |

## Zveřejnění na GitHub Pages

1. Na GitHubu vytvoř nový repozitář, třeba `python-krok-za-krokem` (Public).
2. Klikni na **Add file → Upload files** a nahraj všechny soubory z této složky. Potvrď **Commit changes**.
3. Otevři **Settings → Pages**. U **Source** zvol **Deploy from a branch**, branch **main** a složku **/ (root)**. Ulož.
4. Za minutu až dvě bude aplikace na adrese `https://<tvoje-jmeno>.github.io/python-krok-za-krokem/`.

## Instalace na iPhone

1. Otevři adresu v **Safari**.
2. Počkej, až se nahoře objeví **Python připraven** (poprvé to může trvat i půl minuty).
3. Klepni na **Sdílet → Přidat na plochu**.

Po prvním načtení funguje aplikace i bez internetu.

## Aktualizace

Když upravíš `index.html` a nahraješ ho znovu, telefon si novou verzi stáhne při dalším otevření s internetem.
Pokud změníš `sw.js`, zvyš číslo verze v `APP_CACHE` (např. `pykrok-app-v2`).
