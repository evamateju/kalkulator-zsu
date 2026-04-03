# Kalkulátor ZSU – Historie verzí

---

## Struktura souborů

Od verze v1.1.1 existují ke každé verzi pouze dva soubory:

**zsu_v[verze].html** – veřejný soubor. Jeden a ten samý soubor se nahrává na WordPress (evamateju.cz), na GitHub (jako index.html) i slouží pro offline použití. Kód je uvnitř zabalený v base64, protože WordPress neumí mít složitý JavaScript přímo v HTML – rozbije ho. Base64 wrapper to řeší. Navenek je badge vždy v1.1 · 2026-03-29.

**zsu_SOURCE_v[verze].html** – trezorová verze. Obsahuje čitelný zdrojový kód s anglickými názvy proměnných a komentáři. Slouží výhradně autorce jako ochrana duševního vlastnictví a podklad pro budoucí úpravy. Nikam se nenahrává. Badge odpovídá skutečné interní verzi.

Dřívější dělení na wordpress / standalone / index.html bylo zbytečné – všechny tři soubory byly identické. Od v1.1.1 je jeden veřejný soubor pro všechna použití.

---

## v1.1.2 · 2026-04-03 (SOURCE only)

**PDF export přes pdfmake – přímé stažení PDF souboru bez tiskového dialogu.**

- PDF export nyní generuje soubor přímo ke stažení (ZSU_JmenoPrijmeni_RRRR-MM-DD.pdf)
- Bez vyskakovacího okna, bez tiskového dialogu
- Knihovna pdfmake se načítá z CDN při prvním exportu (Roboto font s plnou češtinou)
- Při nedostupnosti CDN automatický fallback na původní metodu s tiskovým oknem
- Upraven disclaimer: „Obsah případu zůstává výhradně v prohlížeči uživatele a není odesílán na server."

---

## v1.1.1 · 2026-04-03 (SOURCE only)

**Refaktoring pod kapotou – bez viditelných změn pro uživatele.**

- Přechod z base64+eval wrapperu na Terser minifikaci + base64 wrapper (profesionální build pipeline)
- Refaktoring interních proměnných: sémantické anglické názvy (FRAMEWORK_AMOUNTS, QUALIFIER_VALUES, DOMAIN_DATA, ITEM_DESCRIPTIONS)
- Přidány JSDoc anotace ke všem veřejným i interním funkcím
- Přidán strict mode ("use strict") do obou IIFE bloků
- Sjednocení veřejných verzí do jednoho souboru (wordpress = standalone = index)
- Výpočetní logika, vizuální stránka a výstupy zůstávají beze změn

---

## v1.1 · 2026-03-29

- Přidána možnost uložit rozpracovaný případ na disk (JSON soubor)
- Přidána možnost načíst dříve uložený případ
- Data se ukládají lokálně na počítač znalce, bez odesílání na server
- Aktualizován informační text o správě dat
- Nastavena výchozí rámcová částka pro rok 2026 na 19 686 000 Kč

---

## v1.0 · 2026-03-20

**První veřejná verze**

- Výpočet ZSU dle Metodiky Nejvyššího soudu k § 2958 o. z. s využitím principů MKF/ICF
- 9 domén (D1–D9), 74 položek, relativní váhy dle Metodiky
- Kvalifikátory 0–4 s možností vlastního procenta (kapacita i výkon)
- Automatická rámcová částka dle roku ustálení zdravotního stavu (2014–2026)
- Modifikační koeficient
- Textová pole pro odůvodnění kvalifikátoru (max 1000 znaků, přenos do PDF)
- Export do PDF – 4 varianty (s/bez částky v Kč × s/bez popisu obsahu domény)
- Volitelné uvedení zdroje výpočtu v PDF výstupu
- Doménový zámek (evamateju.cz, soudniznalecbrno.cz, GitHub Pages)
- Optimalizace pro desktop, mobilní brána s možností pokračování
- Žádná data se neukládají na server – vše v prohlížeči, vymazáno po zavření

---

*© 2026 MUDr. Eva Matějů, Ph.D. & MUDr. Svatava Duchaňová*
