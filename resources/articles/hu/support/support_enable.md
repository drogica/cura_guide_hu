# Támogatás létrehozása

Az olvasztott izzószálas gyártású 3D nyomtatók úgy működnek, hogy egy szál olvadt műanyagot helyeznek el a megfelelő helyre. Ha ezt a műanyagot nem támasztják alá, akkor leereszkedik, mert jelentős erővel és a gravitáció hatására kiszorul a fúvókán. Hacsak a modell nincs alatta az új réteg megtámasztásához, egy további tartószerkezettel kell alátámasztani, amelyet a modell kinyomtatása után eltávolítanak és eldobnak.

Ez a beállítás lehetővé teszi az objektumot támasztó struktúrák létrehozását a nyomtatás közben. A Cura alapértelmezés szerint nem engedélyezi ezt a támogatást, de pirosra jelöli a modell felületét, ha úgy gondolja, hogy az ott lévő anyag nagyon megereszkedhet, ha a támogatás nincs engedélyezve.

<!--screenshot {
"image_path": "support_enable_prepare_mode.png",
"models": [{"script": "pipe_corner.scad"}],
"camera_position": [77, 197, 40],
"layer": -1
}-->

<!--screenshot {
"image_path": "support_enable.png",
"models": [{"script": "pipe_corner.scad"}],
"camera_position": [77, 197, 40],
"settings": {"support_enable": true},
"colours": 64
}-->

![A modell piros jelölése, ahol támogatásra van szükség](../images/support_enable_prepare_mode.png)![Tartószerkezet (cián színben) a modell megtámasztására a nyomtatás során](../images/support_enable.png)

A nyomtatás támogatása jelentős időt és anyagot igényel. Ahol a támaszték hozzáér a modellhez, azt később, a nyomtatás befejezése után le kell törni vagy le kell vágni. Ez hajlamos heget hagyni a felületen.

A támogatás azonban néha teljesen szükséges. Például, ha a modellnek van egy darabja, amely lefelé mutat az építőlemez felé, akkor ez a darab egyébként csak a levegőben lógna.

## Kialakítás a támogatás megakadályozására

Bár néha szükséges, a nyomtatás támogatását lehetőség szerint meg kell akadályozni. Számos technika létezik a támogatás nyomtatásának elkerülésére. Ez a 3D nyomtatás modelltervezésének nagy része. Íme néhány technika, amellyel a 3D-s modell módosítható, hogy ne legyen szüksége támogatásra.

- Állítsa be a modellt úgy, hogy ne legyen sík felület magasabb, mint az építőlemez.
- Amennyire csak lehetséges, kerülje a túlnyúlások tervezését.
- Ha van felület közvetlenül az építőlemez felett, húzza le az építőlemezhez.
- A kis párkányok 45 fokos dőlésszöggel támaszthatók meg, áthelyezve a túlnyúlást a modellbe.
- A nagyobb túlnyúlások áthidalhatók, ha mindkét oldalon alátámasztják őket. A Cura automatikusan úgy irányítja a túlnyúlás alsó oldalának vonalait, hogy azok egyenes vonalban menjenek át a hídon. E vonalak nyomtatása során a fúvóka feszültséget tart a gyöngyön, hogy az ne ereszkedjen le. Ez elegendő időt ad neki, hogy megszilárduljon, hogy önmagában is megállja a helyét.
- Ha a túlnyúlásban rés van, akkor áldozati hidat lehet kialakítani. Ez az egyik réteg, amelyben a rés zárva van. Ez jó áthidalást tesz lehetővé, így a második réteg ráépítheti a rés megfelelő falait a tetejére. Nyomtatás után a rés késsel nyitható, hiszen csak egy réteg vastag.
