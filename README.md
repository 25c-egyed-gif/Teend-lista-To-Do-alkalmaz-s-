# Cím
Teendő lista (To-Do alkalmazás)

# Klubprojekt

## Készítők
- Norman
- Bálint

## Cél
Készítsünk egy olyan alkalmazást, amiben tudjuk vezetni a napi teendőinket.

## Indítás
A `teendolista.html` megnyitása böngészőben. A `style.css` és a `script.js` fájlnak ugyanabban a mappában kell lennie, mint a HTML-nek. A Bootstrap betöltéséhez internetkapcsolat kell.

## Kész funkciók
- Új feladat hozzáadása (gombbal vagy Enterrel)
- Feladat törlése
- Kész feladatok megjelölése (áthúzott szöveg)
- Kész / összes feladat számláló
- Feladatok mentése LocalStorage-ba, így újratöltés után is megmaradnak
- Üres feladat felvételének tiltása
- Reszponzív megjelenés (telefonon is használható)

## Tesztelés
Kézzel teszteltük Chrome-ban és Edge-ben:
- Hozzáadtunk több feladatot, majd újratöltöttük az oldalt: a lista megmaradt.
- Üres szöveggel és csak szóközökkel próbáltunk feladatot felvenni: nem adta hozzá.
- Kipipáltunk, majd töröltünk feladatokat: a számláló jól frissült.
- Nagyon hosszú szöveget is beírtunk: a szöveg tördelődik, nem lóg ki a kártyából.
- Szűkített böngészőablakban és telefonon is megnéztük a megjelenést.

## Feladatmegosztás
Norman - GitHub kezelés, JavaScript, BootStrap
Bálint - HTML, Kommitolás

## Források és átvett részek
- Bootstrap 5.3.3 (CDN-ről betöltve): https://getbootstrap.com
- Az alap kódot MI-asszisztens (Claude) segítségével készítettük, majd átnéztük és a saját igényeinkre alakítottuk.

## Ismert hibák
- Akadtak gondok a kommitolással, többször ütköztek a változtatások, mert egyszerre szerkesztettük ugyanazt a fájlt.
- A README-ben először `index.html` szerepelt, pedig a fájl neve `teendolista.html`.
- A feladatokat nem lehet szerkeszteni, csak törölni és újra felvenni.
- A törlés megerősítés nélkül azonnal megtörténik, így véletlenül is el lehet veszíteni egy feladatot.
- A LocalStorage böngészőnként külön tárol, ezért másik böngészőben vagy gépen üres a lista.
- Privát (inkognitó) módban bezáráskor törlődnek a mentett feladatok.
- Internet nélkül a Bootstrap nem töltődik be, ilyenkor csúnyább az oldal.
- A feladatokat nem lehet átrendezni, mindig a hozzáadás sorrendjében jelennek meg.