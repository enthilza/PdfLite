# PdfLite

Prenosný PDF prehliadač a ľahký editor pre Windows 10/11 (64-bit). Celá aplikácia
je jediný súbor `PdfLite.exe` — bez inštalácie a bez runtime, ktorý by sa musel
sťahovať.

## Stiahnutie

Najnovšia verzia: [Releases](../../releases/latest) → `PdfLite.exe`.

1. Stiahni `PdfLite.exe` do priečinka, do ktorého môžeš zapisovať (nie
   `Program Files`).
2. Spusť ho. Prvú verziu treba nainštalovať ručne.
3. Ďalšie verzie sa už aktualizujú samé, vždy až po tvojom potvrdení.

Rozhranie je predvolene slovenské; angličtinu prepneš v **Nastavenia → Jazyk**.

## Aktualizácie

Tento repozitár slúži **iba na distribúciu aktualizácií**. Obsahuje výhradne
`PdfLite.exe` a podpísaný manifest (`update.json`, `update.sig`) v releases.
Zdrojový kód tu nie je.

- Aplikácia kontroluje `releases/latest/download/update.json`.
- Manifest je podpísaný RSA-3072 / SHA-256, verejný kľúč je súčasťou EXE.
- Sťahovaný súbor musí sedieť na veľkosť, SHA-256 aj verziu z manifestu.
- Aktualizácia sa nainštaluje len po potvrdení; pri zlyhaní sa obnoví
  predchádzajúca verzia.

## Systémové požiadavky

- Windows 10 alebo Windows 11, 64-bit
- .NET Framework 4.8 (je súčasťou Windows)

## Poznámky

- Editor slúži na anotácie a prácu so stranami; existujúci obsah strán nemení.
- Formuláre AcroForm sa zobrazujú, ale nedajú sa vypĺňať.
- Uloženie digitálne podpísaného PDF zneplatní podpis, rovnako ako v iných
  editoroch.
