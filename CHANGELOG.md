CHANGELOG_verejny
Kalkulátor ZSU – Historie verzí
Výpočetní pravidla podle Metodiky Nejvyššího soudu k § 2958 o. z. zůstávají ve všech verzích stejná. Mění se ovládání, výstupy a hodnoty, které stanoví právní předpis.

v1.2.2 · 21.09.2026
Kalkulátor se přizpůsobuje místu, které na stránce skutečně dostal.

Rozložení tabulky i chování bočního panelu se nově řídí šířkou, kterou má kalkulátor na stránce k dispozici, ne šířkou okna prohlížeče. Na webech, kde je kalkulátor vložený do užšího sloupce nebo do rámu, se dosud část obsahu mačkala nebo ořízla
Boční panel s průběžným stavem se přicvakne vedle kalkulátoru všude, kde je na něj vedle něj místo. Kde by se musel vysunout přes obsah, ukáže se jen na dostatečně široké stránce. Dřív se držel okraje okna, tedy někdy daleko od tabulky
Na úzké stránce se panel neukáže vůbec a tabulka přepne do úsporného rozložení, místo aby přetékala
Opraveno načítání dříve uloženého případu: formulář se před vložením dat vyprázdní, takže se nemohou smíchat hodnoty dvou případů. Podnět Petra Kalouse
Doplněna deklarace kódování, bez které se u souboru otevřeného přímo z disku mohla rozsypat diakritika
v1.2 · 17.09.2026
Ochrana rozpracovaného případu, přehlednější práce s dlouhou tabulkou a přestavěné výstupy do PDF.

Práce s případem

Rozpracovaný případ se průběžně zálohuje v paměti okna prohlížeče. Když se stránka zasekne nebo ji omylem obnovíte, kalkulátor nabídne vrácení zadaných hodnot. Záloha se zavřením okna ztrácí a nikam se neodesílá
Kalkulátor upozorní při zavírání okna, pokud máte rozpracovaný a neuložený případ
Plovoucí boční panel drží průběžný stav při rolování tabulkou: počet vyplněných položek, součet procent, koeficient, výši ZSU a tlačítka pro uložení a načtení případu
Panel slouží i jako rozcestník. Kliknutím na doménu se doména otevře a stránka na ni odroluje
Domény se sbalují. Otevřená je vždy jen jedna, ostatní v hlavičce ukazují, kolik mají vyplněno a jakých procent dosáhly. Lze přepnout na rozbalení všech
Modifikační koeficient je nově i pod výpočtem, obě pole jsou propojená
Načíst a Uložit případ jsou nově i v úvodní kartě
Zobrazení

Kódy MKF se píší malým písmenem, tedy d1 až d9 a d110 až d950
Procenta a relativní váhy se zobrazují s českou desetinnou čárkou
Texty o tom, kde zůstávají zadaná data, přepsány srozumitelněji a doplněny o rozbalovací vysvětlení „Kde jsou vaše data?“
Výstupy do PDF

Na začátku výstupu je souhrn se součtem korigovaných procent a u variant s částkou i s vypočtenou výší ZSU
Stránky se číslují ve tvaru 1 / 10. Odstraněno zápatí, do kterého u delších výstupů zasahoval text
Přibyla třetí varianta výstupu, přehledný soupis jen s vyplněnými položkami, bez odůvodnění znalce a bez popisu obsahu domén
Volba výstupu přestavěna na tři karty s přehledem, co bude ve výstupu obsaženo
Mezi doménami je volný řádek, hodnocení znalce se tiskne normálním písmem a popis obsahu domény kurzívou
Zdroj výpočtu se uvádí na začátku i na konci výstupu
Datum ustálení zdravotního stavu se tiskne ve tvaru DD.MM.RRRR
v1.1.3 · 22.05.2026
Zpřesnění výchozí rámcové částky pro rok 2026 a sjednocení formulace nápovědy.

Výchozí rámcová částka pro rok 2026 upravena na 19 686 000 Kč (předchozí hodnota 19 200 000 Kč již neodpovídala aktuální výši)
Odstraněno označení „orientační" u rámcové částky pro rok 2026 – nápověda nyní pro všechny roky zobrazuje jednotně „Rok [RRRR]"
Změna byla podnětem oddělení škod na zdraví České podnikatelské pojišťovny (ČPP)
v1.1.2 · 18.04.2026
Zvětšení písma ve výstupu do PDF pro lepší čitelnost.

v1.1.1 · 06.04.2026
Vymezení autorství a doplnění ochranných prvků copyright.

v1.1 · 29.03.2026
Přidána možnost uložit rozpracovaný případ na disk jako soubor
Přidána možnost načíst dříve uložený případ
Data zůstávají v počítači uživatele, neodesílají se na server
Aktualizován informační text o správě dat
v1.0 · 20.03.2026
První veřejná verze

Výpočet ZSU dle Metodiky Nejvyššího soudu k § 2958 o. z. s využitím principů MKF/ICF
9 domén, 74 položek, relativní váhy dle Metodiky
Kvalifikátory 0–4 s možností vlastního procenta pro kapacitu i výkon
Automatická rámcová částka dle roku ustálení zdravotního stavu (2014–2026)
Modifikační koeficient
Textová pole pro odůvodnění kvalifikátoru (max 1000 znaků, přenos do PDF)
Export do PDF ve variantách s částkou i bez ní, s popisem obsahu domény i bez něj
Optimalizace pro práci na počítači
Žádná data se neukládají na server, vše zůstává v prohlížeči a po zavření se maže
© 2026 MUDr. Eva Matějů, Ph.D. & MUDr. Svatava Duchaňová
Volně k použití pro znaleckou praxi. Kopírování, úprava nebo další distribuce bez souhlasu autorek není povolena.
