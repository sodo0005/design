---
Title: Load
Description: This is our colors page.
Template: analysis
---

# Load

Load Rapport
=======================

Denna rapport är en individuell utvärdering av tre olika webbplatsers laddningstid och responsivitet.

Urval
-----------------------

Jag har valt att fortsätta min analys av webbplatserna som jag analyserade i den tidigare rapporten, de tre stora modehusen Hermés, Louis Vuitton och Gucci. Jag vill undersöka och se hur de skiljer sig i laddningstid och responsivitet. Speciellt nu under juletider när många kommer handla online så är det viktigt att ha en snabb responsiv hemsida. Från förra rapporten vet jag att de använder många bilder och videor på hemsidan så det ska bli intressant att se hur de lyckas göra detta och om sidan upplevs som långsam.

Metod
-----------------------

Verktygen som jag använde är webbläsaren Firefox Developer Edition-> Inspector verktyget -> Network fliken. Jag använde också [PageSpeed Insight](https://pagespeed.web.dev/) som ger värdefull information och betygsätter en hemsidas laddningstid och responsivitet. All data som jag samlar upp skriver jag ner i Google Sheets.

Resultat
-----------------------

### Tabell Laddningstid & Responsitivitet
<div class="table-container">
    <iframe class="load-table" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSHRbc_Efk6GJK5pBIceB0k7Ib42qkpgwzVLi71xYblwXP6szh97L2GFXrMxomtwjRcMjynI1F4XjIw/pubhtml?widget=true&amp;headers=false"></iframe>
</div>

## Hermés

![Hermés Screenshot](../image/hermes-screenshot.png?width=50%)

Hermés skulle kunna optimera stora bilder/videor och förbättra tillgängligheten ytterligare, t ex genom att lägga till ett lang attribut på html elementet.

## Louis Vuitton

![Louis Vuitton Screenshot](../image/lv-screenshot.png?width=50%)

Louis Vuitton behöver bland annat fixa sin javascript execution då det tar lång tid - 3,5s, även se över bild/video optimering.

## Gucci

![Gucci Screenshot](../image/gucci-screenshot.png?width=50%)

Gucci behöver också kolla över sitt javascript då det tar lång tid att exekvera scriptet, samt kolla över CSS kod som inte används och optimera bild/video storlekar.

Analys
-----------------------

Det vanligaste förbättringsåtgärderna för dessa tre webbplatserna verkar vara att minska INP (Interaction to Next Paint) på mobil sidorna eftersom alla webbplatserna fick ett dåligt resultat på INP. INP visar hur pass responsiv en webbplats är och hur snabbt den reagerar på användarens clicks eller interaktioner. 

En bra INP poäng ligger på max 200 ms och vi kan se att bäst poäng där fick Hermés landningssida (mobil) på 213 ms, Guccis landningssida (mobil) på 268 ms och Louis Vuittons landningssida (mobil) på 593 ms.

Om vi istället tittar på LCP poängen (mobil) så finns det garanterat förbättringspotential. LCP mäter laddningstiden på webbplatserna och bör inte ligga över 2.5 sekunder. Där utmärkte sig Guccis landningssida (Mobil) bäst på 1.3 sekunder, Louis Vuttions landningssida (Mobil) på 1.6 och Hermés Landningssida (Mobil) på 3 s.

Kollar vi istället på snitt laddningstiden på alla landningssidor vi fått från Inspect verktyget (Desktop) så kan vi se att Gucci laddar in sin sida snabbast på 1.96 s, Louis Vuitton på 2.47 s och Hermés på 2.62 s.

Baserat på resultatet från datan så skulle jag säga att vinnaren är Gucci eftersom webbplatsen laddas in snabbast och är relativt responsiv. Det finns som sagt förbättringspotential, speciellt javascriptet. Även INP poängen kan bli bättre och då är det viktigt att optimera bilder och videor.


Referenser
-----------------------

* [LCP Score](https://web.dev/articles/lcp)
* [INP Score](https://web.dev/articles/inp)
* [PageSpeed Insight](https://pagespeed.web.dev/)

Övrigt
-----------------------

Rapporten är skriven av Sophie Gustafsson - sodo21

