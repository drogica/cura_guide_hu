# G-kód íz

Míg a g-kód egy szabványos formátum az utasítások CNC gépekkel, például 3D nyomtatókkal történő továbbítására, még mindig vannak különbségek abban, hogy az egyes nyomtatók melyik g-kódokat támogatják, mi a kezdeti állapotuk, és néha abban, hogyan értelmezik a parancsokat. A g-code ízzel nagyrészt jelezheti, hogy a nyomtató milyen parancsokat fogad el.

A különbség ezek között a g-kód ízek között általában meglehetősen kicsi. A legfontosabb parancsok, mint például a mozgás és a fúvóka melegítése, általában ugyanazok.

A megfelelő g-kód íz kiválasztásához olvassa el a nyomtató firmware-ének dokumentációját. Meg kell mondania, hogy mely funkciók támogatottak és melyek nem. Ezek a Cura-ban elérhető ízek, és ezek különbségei.

## Marlin

A Marlin az alapértelmezett g-kódos íz. A fő [Marlin firmware-](https://marlinfw.org/) hez készült, amely a legnépszerűbb 3D nyomtatás firmware és a legtöbb alternatív firmware alapja.

## Marlin (térfogat)

Ez egy olyan változat a Marlinon, ahol az extrudálási parancsok határozzák meg, hogy mennyit extrudálnak köbmilliméterben, nem pedig az izzószál hosszában. Ezek a figyelemre méltó változások:

- A `G1` parancs `E` paramétere köbmilliméterben, a betáplált műanyag térfogatában, nem pedig a mozgás során betáplálandó izzószál hosszában kerül kiszámításra.
- A g-kód elején található statisztikák a használt izzószálat köbmilliméterben is feltüntetik.

## RepRap

Ez egy olyan íz, amely a [RepRap projektből](https://reprap.org/wiki/RepRap) fejlődött nyomtatók támogatására összpontosít. Számos figyelemre méltó kivétel van:

- A kezdeti réteghőmérséklet beállításakor mindig említse meg az extrudert, még akkor is, ha csak egy extruder van.
- A nyomtatás után térjen vissza a relatív extrudáláshoz.
- Módosítsa a gyorsulásokat az `M204` parancs `P` és `T` paramétereivel, a nyomtatási gyorsulás és az utazási gyorsulás esetén az `S` paraméter helyett.
- Változtassa meg a rángatást az `M566` paranccsal az `M205` parancs helyett.

## Ultimaker 2

Ez a g-kódos íz az Ultimaker 2 család számára készült. Ennek a családnak a firmware-ének az a furcsa ötlete támadt, hogy a szeletelő helyett a nyomtatónak kellene lehetővé tennie az anyaggal kapcsolatos beállítások vezérlését. Ezek a kivételek:

- A g-kódban nem lesznek nyomtatási hőmérsékleti parancsok.
- A g-kódban nem lesznek felépítési lemez hőmérsékleti parancsok.
- A g-kódban nem lesznek felépítési térfogat hőmérsékleti parancsok.
- Feltételezzük, hogy az első fúvóka a [kezdeti rétegnyomtatási hőmérséklettel](../material/material_print_temperature_layer_0.md) rendelkezik a nyomtatás megkezdésekor.
- Feltételezzük, hogy az építőlemez a [kezdeti réteg felépítő lemez hőmérsékletével](../material/material_bed_temperature_layer_0.md) rendelkezik a nyomtatás megkezdésekor.
- A `G1` parancs `E` paramétere köbmilliméterben, a betáplált műanyag térfogatában, nem pedig a mozgás során betáplálandó izzószál hosszában kerül kiszámításra.
- A g-kód elején található statisztika köbmilliméterben tünteti fel a használt izzószálat.

## Griffmadár

Ez a g-kód íz a modern Ultimaker nyomtatókhoz, az Ultimaker 3-hoz és újabbhoz. Ezeknek a nyomtatóknak egy csomó metaadatra van szükségük bizonyos formátumban a g-kód elején. A különbségek ebben a g-kód ízben a következők:

- A g-kód elején egy nagy fejléc található, amely metaadat-információkat tartalmaz, például a nyomtatás időtartamát, a nyomtatási feladat nevét, és néhány gyakorlati információt, például a kezdő hőmérsékletet és a nyomtatás határolódobozát.
- A g-kódban nem lesznek felépítési térfogat hőmérsékleti parancsok.
- Feltételezzük, hogy az első fúvóka a [kezdeti rétegnyomtatási hőmérséklettel](../material/material_print_temperature_layer_0.md) rendelkezik a nyomtatás megkezdésekor.
- Feltételezzük, hogy az építőlemez a [kezdeti réteg felépítő lemez hőmérsékletével](../material/material_bed_temperature_layer_0.md) rendelkezik a nyomtatás megkezdésekor.
- Feltételezzük, hogy a nyomtató nem az első extruderen indul, ezért mindig a nyomtatás elején egy `T` paranccsal átvált az indító extruderre.
- Minden extruderhez egy elsődleges blobot nyomtat `G280` a visszahúzás helyett, amikor először elkezdi a nyomtatást.

## Makerbot

Ez egy g-kód íz, amelyet [a Sailfish](https://www.sailfishfirmware.com/) alapú firmware-hez terveztek. Ezt a firmware-t az eredeti Makerbot nyomtatók utódaiban használják. Néhány figyelemre méltó különbség a következő:

- A nyomtatási hőmérséklet megváltoztatásakor `M109` (beállított hőmérséklet és várakozás) nem támogatott. Helyette `M104` et ad ki, ami nem várja meg a hőmérséklet elérését. Ezután `M116` tal utasítja a nyomtatót, hogy várja meg, amíg eléri ezt a hőmérsékletet.
- A `G1` kihúzási parancs `E` dimenziója nem áll vissza a nyomtatás során. Más ízeknél ez a paraméter minden 10 méteres izzószál után nullázódik egy `G92 E0` paranccsal, hogy megakadályozza a lebegőpontos kerekítési hibákat a firmware-ben, de ennél nem.
- Az extruderek váltása az `M135` paranccsal történik, nem pedig a `T` parancsokkal.
- A ventilátor sebessége nem jelenik meg. A ventilátor vagy teljesen be van kapcsolva, vagy ki van kapcsolva. A Cura utasítja a nyomtatót, hogy kapcsolja be a ventilátort, ha egyébként legalább 50%-os ventilátorsebességre vágyna.

## Bitek a bytes-ból

Ez egy g-kód íz, amely a Bits from Bytes nyomtatókat célozza meg, amelyek saját egyedi firmware-rel rendelkeztek. G-kódos ízük jelentősen eltér a többitől. A Cura a következő változtatásokat hajtja végre:

- Az extrudálási mennyiségek az adagoló RPM-jével íródnak, nem pedig az `E` paraméterrel.
- A visszahúzások az aktív extrudertől függően `M101` gyel vagy `M201` írhatók.
- A visszahúzási sebességet külön `M108` paranccsal írjuk ki.
- A mozgási mozgásokat `M103` paranccsal jelzi, ahelyett, hogy `G1` et `G0` ra kapcsolnák ki. Nem lesznek `G0` parancsok.
- A nyomtató az `M227` paranccsal automatikus visszahúzásra van beállítva.
- A Cura Windows-stílusú új sorokat fog kiírni kocsivisszaváltással az újsor szimbólum helyett.
- A `G1` kihúzási parancs `E` dimenziója nem áll vissza a nyomtatás során. Más ízeknél ez a paraméter minden 10 méteres izzószál után nullázódik egy `G92 E0` paranccsal, hogy megakadályozza a lebegőpontos kerekítési hibákat a firmware-ben, de ennél nem.

## Mach3

Ez egy g-kód íz, amely közelebb marad ahhoz, ahogyan a CNC-malmok elvárják a g-kódtól. Egyetlen figyelemre méltó különbség van:

- Az extrudálási mennyiségek a `G1` parancs `A` paraméterével íródnak az `E` paraméter helyett.

## Ismétlő

Ez a Repetier g-kódos íze a 3D nyomtatóknak készült. A Repetier szeletelő kimenetét utánozza. Ezek a jelentős különbségek ezzel a g-kódos ízzel:

- Ha a firmware-visszahúzások engedélyezve vannak, az extruderkapcsoló visszahúzásai `G10 S1` használják annak jelzésére, hogy ez egy extruderkapcsoló visszahúzása.
- A gyorsulás módosítása az `M201` és `M202` parancsok használatával történik (a nyomtatási gyorsuláshoz és az utazási gyorsuláshoz) `M204` helyett.
- A rántásmódosítások az `M207` parancs helyett az `M205` paranccsal hajthatók végre.

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában. Ehhez a beállításhoz van egy kiválasztó menü a nyomtatóbeállítások párbeszédpanelen, amely a hozzáadott nyomtatók listájában található a beállítások párbeszédablakban.**
