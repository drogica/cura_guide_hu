# Indítsa el a G-kódot

Ezzel a beállítással egy kis g-kód írható, amely minden nyomtatás legelején lefut. Ezzel a g-kóddal a nyomtató beállítható, hogy készen álljon a nyomtatásra.

Néhány példa azokra a dolgokra, amelyeket általában a start g-kódban hajtanak végre:

- A fúvóka(k) alapozása.
- Az építőlemez felmelegítése.
- A fúvókák felmelegítése.
- Győződjön meg arról, hogy a megfelelő extrudert választotta ki.
- A ventilátorok, a gyorsítások vagy a rángatás beállítása.
- Automatikus ágyszintezés.
- Lineáris előrelépés konfigurálása.

Az ide írható elérhető g-kódok ésszerűen átfogó listája a [RepRap Wikiben](https://reprap.org/wiki/G-code) található.

## Hivatkozások a beállításokra

A start g-kód szerkesztésekor hivatkozhat más beállítások értékeire. Ez egy bizonyos szintaxist használ. A beállításokra a *kulcsuk* hivatkozik. Ez a kulcs a Cura belső neve. Nem látható a felhasználói felületen. Az összes kulcs teljes listáját a Cura forráskódjában található [dokumentumban](https://github.com/Ultimaker/Cura/blob/master/resources/definitions/fdmprinter.def.json) találja.

A szintaxis a globális beállítás értékének lekéréséhez a következő:

`{setting_key}`

Más szóval, írja be a beállítás kulcsát zárójelbe. Ez megkapja egy beállítás globális értékét. Sok beállítás azonban eltérhet az egyes extrudereknél. Ezekre a következőképpen kell hivatkozni:

`{setting_key, #}`

Ide a `#` szimbólum helyére annak az extrudernek a számát kell beírni, ahonnan a beállítást kapja. Az extruderek 0-tól kezdik a számlálást. A globális beállításokat egy extruder megadásával is megkaphatjuk, de ezek minden extrudernél azonosak lesznek. Ha az extruder számának megadása nélkül próbál beállítani egy extruder-specifikus hőmérsékletet, akkor az első nem letiltott extruder értékét kapja meg.

Ezeket a hivatkozásokat használhatja például a megfelelő hőmérsékletre történő előmelegítéshez vagy a gyorsulások beállításához. Íme néhány példa:

`M104 S{material_print_temperature_layer_0, 0} ;pre-heat`

`M140 S{material_bed_temperature_layer_0} ;heat bed`

`M204 P{acceleration_print, 0} T{acceleration_travel, 0}`

`M205 X{jerk_print, 0}`

Legyen óvatos a sebességekkel. A G-code általában milliméter/ *perc-* ben fogadja el az előtolási sebességet, míg a beállítások milliméter/ *másodpercben* vannak megadva. Jelenleg nincs mód a megfelelő előtolás kiválasztására. Ezekben a hivatkozásokban a számítások elvégzése lehetetlen.

## Egyéb információk

A beállításokra való hivatkozásokkal megegyező szintaxis révén néhány kiegészítő információ is elérhető:

- `{time}` a szeletelt nap aktuális helyi idejére utal.
- `{date}` a felvágás dátumára utal.
- `{day}` a hét azon napjára utal, amelyen fel lett vágva.
- `{initial_extruder_nr}` arra az extruderre utal, amellyel a nyomtatás elindul.

<!--if cura_version>=4.12-->

- `{material_id}` az aktív anyag egyedi azonosítójára utal. Adja meg az extrudert a többi beállításhoz hasonlóan.
- `{material_name}` az aktív anyag nevére utal. Általában ez a név az adott anyagot árusító webhelyen.
- `{material_type}` az aktív anyagok osztályára utal, például PLA vagy ABS.
- `{material_brand}` az aktív anyag gyártójára utal.
- `{print_time}` a nyomtatás becsült időtartamára utal (ISO-8601 szerint formázva).
- `{filament_amount}` az egyes extruderekhez használt izzószál hosszát jelenti méterben. Ez egy lista formájában lesz formázva, körülöttük szögletes zárójelekkel.
- `{filament_weight}` a felhasznált izzószál tömegére vonatkozik grammban, minden egyes extruderhez külön, szögletes zárójeles lista formájában. Ha az orsó súlya ismeretlen, ez 0 lesz.
- `{filament_cost}` a használt izzószál költségére vonatkozik, minden extruderre külön-külön. A költség mértékegysége megegyezik a preferenciáknál az anyagkezelési oldalon szereplővel. Ha ismeretlen, akkor ez 0 lesz.

<!--endif-->

## Fűtés a rajt előtt g-kód

A Cura automatikusan kiadja a fűtési parancsokat, mielőtt a start g-kód elkezdődik. Így a start g-kódnak nem kell figyelembe vennie, hogy a fúvókának fel kell melegednie. Azonnal megkezdheti a fúvóka alapozását. Ha a kezdő g-kód hivatkozást tartalmaz bármely hőmérsékletre (a fúvóka vagy az ágy esetében), ez le lesz tiltva (illetve a fúvókánál vagy az ágynál).

**Ez a beállítás gépbeállítás, így nem jelenik meg a normál beállításlistában. Ezt úgy módosíthatja, hogy a beállítások képernyőn a nyomtatók listájára lép, és rákattint a "Gépbeállítások" elemre.**
