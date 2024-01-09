# Cool Down Speed

Ez a beállítás megadja a Curának, hogy milyen gyorsan hűl le a fúvóka, ha nem melegszik. Arra használják, hogy előre jelezzék, mikor kell elkezdeni a fúvóka előhűtését az extruderek váltása előtt.

![A fúvókák már az extruderek váltása előtt elkezdenek felmelegedni](../images/temperature_regulation.svg)

Extruder váltáskor a Cura közvetlenül a befejezés előtt elkezdi az aktív fúvóka előhűtését, hogy az egy kicsit kevésbé szivárogjon ki várakozás közben. A Cura azt is megpróbálja megjósolni, hogy a fúvóka mennyire hűlt le, amíg inaktív volt. Így tudja, hogy utána mennyit kell újra felmelegíteni.

Ha a fúvóka ténylegesen gyorsabban hűl le, mint amit ez a beállítás jelez, a fúvóka gyorsabban lesz készenléti hőmérsékleten, mint amit Cura megjósolt. Emiatt tovább tarthat a fúvóka felmelegítése, mint amennyit Cura megjósolt, és a nyomtató a fúvókakapcsolónál várja, hogy a fúvóka tovább melegedjen.

Ha a fúvóka valóban lassabban hűl le, mint amit ez a beállítás jelez, a fúvóka még mindig meleg lehet, amikor Cura parancsot küld a fúvóka előmelegítésére, ami túl gyorsan melegszik fel. Egy ideig nyomtatási hőmérsékleten lesz, mielőtt a fúvókára kerül a sor a nyomtatásra. Ezalatt egy kicsit szivárog, és a műanyag még egy kicsit lebomlik.

A tényleges lehűlési sebesség nem egy állandó sebesség fok/másodpercben. Valószínűbb, hogy ez a fúvóka aktuális hőmérséklete és az építési térfogat hőmérséklete közötti különbségtől függ. Így gyorsabban lehűl, ha meleg van, és lassabban hűl le, ahogy közeledik a készenléti hőmérséklethez. Ha ezt hangolja, próbálja meg úgy hangolni, hogy megméri a [végső nyomtatási hőmérséklettől](../material/material_final_print_temperature.md) a [készenléti hőmérsékletig](../material/material_standby_temperature.md) való lehűléshez szükséges időt. Ez a legfontosabb pálya, amelyet Cura megpróbál megjósolni. Kis nyomatok készítésekor kissé növelheti a hűtési sebességet, hogy beállítsa, hogy gyakrabban maradjon forró.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
