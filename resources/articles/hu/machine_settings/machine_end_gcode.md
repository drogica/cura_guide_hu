# Vége a G-kódnak

Ezzel a beállítással egy kis g-kód írható, amely minden nyomtatás legvégén lefut. Ezzel a g-kóddal a nyomtató kikapcsolhatja alkatrészeit, és nyomtatás után megtisztíthatja.

Néhány példa azokra a dolgokra, amelyeket általában a g-kód végén hajtanak végre:

- Az anyag visszahúzása.
- A fúvókák lehűtése.
- Az építőlemez lehűtése.
- A ventilátorok kikapcsolása.

Az ide írható elérhető g-kódok ésszerűen átfogó listája a [RepRap Wikiben](https://reprap.org/wiki/G-code) található.

## Hivatkozások a beállításokra

A vég g-kód szerkesztésekor hivatkozhat más beállítások értékeire. Ez egy bizonyos szintaxist használ. A beállításokra a *kulcsuk* hivatkozik. Ez a kulcs a Cura belső neve. Nem látható a felhasználói felületen. Az összes kulcs teljes listáját a Cura forráskódjában található [dokumentumban](https://github.com/Ultimaker/Cura/blob/master/resources/definitions/fdmprinter.def.json) találja.

A szintaxis a globális beállítás értékének lekéréséhez a következő:

`{setting_key}`

Más szóval, írja be a beállítás kulcsát zárójelbe. Ez megkapja egy beállítás globális értékét. Sok beállítás azonban eltérhet az egyes extrudereknél. Ezekre a következőképpen kell hivatkozni:

`{setting_key, #}`

Ide a `#` szimbólum helyére annak az extrudernek a számát kell beírni, ahonnan a beállítást kapja. Az extruderek 0-tól kezdik a számlálást. A globális beállításokat egy extruder megadásával is megkaphatjuk, de ezek minden extrudernél azonosak lesznek. Ha az extruder számának megadása nélkül próbál beállítani egy extruder-specifikus hőmérsékletet, akkor az első nem letiltott extruder értékét kapja meg.

Ezeket a hivatkozásokat használhatja például a készenléti hőmérsékletre való lehűtéshez, vagy a nyomtató alapértelmezett gyorsításának és rángatásának visszaállításához. Íme néhány példa:

`M104 T0 S{material_standby_temperature, 0} ;stand-by for the next print`

`M104 T1 S{material_standby_temperature, 1}`

`M204 P{machine_acceleration} T{machine_acceleration}`

Legyen óvatos a sebességekkel. A G-code általában milliméter/ *perc-* ben fogadja el az előtolási sebességet, míg a beállítások milliméter/ *másodpercben* vannak megadva. Jelenleg nincs mód a megfelelő előtolás kiválasztására. Ezekben a hivatkozásokban a számítások elvégzése lehetetlen.

## Egyéb információk

Ugyanazzal a szintaxissal, mint a beállításokra való hivatkozásokkal, néhány segédinformáció is elérhető:

- `{time}` a szeletelt nap aktuális helyi idejére utal.
- `{date}` a felvágás dátumára utal.
- `{day}` a hét azon napjára utal, amelyen fel lett vágva.
- `{initial_extruder_nr}` arra az extruderre utal, amellyel a nyomtatás elindul.

<!--if cura_version>=4.12-->

- `{material_id}` az aktív anyag egyedi azonosítójára utal. Adja meg az extrudert a többi beállításhoz hasonlóan.
- `{material_name}` az aktív anyag nevére utal. Általában ez a név az adott anyagot árusító webhelyen.
- `{material_type}` az aktív anyagok osztályára utal, például PLA vagy ABS.
- `{material_brand}` az aktív anyag gyártójára utal.

<!--endif-->

**Ez a beállítás gépbeállítás, így nem jelenik meg a normál beállításlistában. Ezt úgy módosíthatja, hogy a beállítások képernyőn a nyomtatók listájára lép, és rákattint a "Gépbeállítások" elemre.**
