# Felfűtési sebesség

Ez a beállítás megadja a Curának, hogy a nyomtató milyen gyorsan tudja felmelegíteni ezt a fúvókát. Arra használják, hogy megjósolják, mikor kell elkezdeni a fúvóka előmelegítését az extruderek váltása előtt.

![A fúvókák már az extruderek váltása előtt elkezdenek felmelegedni](../images/temperature_regulation.svg)

A fúvókák váltásakor a Cura megkezdi a következő fúvóka előmelegítését, mielőtt azt használni kellene, így az készen áll a használatra, amikor a másik extruder elkészült. Ehhez a fúvóka aktuális hőmérséklete és a fúvóka célhőmérséklete közötti különbséget el kell osztani a felfűtési sebességgel, hogy megkapjuk a fúvóka előmelegítésének időtartamát.

Ha a fúvóka valóban gyorsabban melegszik fel, mint amit ez a beállítás jelez, a fúvóka egy ideig a célhőmérsékleten lesz, mielőtt a másik extruder befejezné a nyomtatást. Ez idő alatt kiszivárog némi anyag, és a műanyag kissé lebomolhat a fúvókában, ami [alulextrudálást](../troubleshooting/underextrusion.md) eredményezhet.

Ha a fúvóka valóban lassabban melegszik fel, mint amit ez a beállítás jelez, a nyomtatónak meg kell várnia az extruder kapcsolójánál, amíg a fúvóka eléri a kívánt hőmérsékletet a nyomtatáshoz. Ez több időt vesz igénybe. Ezen kívül az előző extrudert is a végső nyomtatási hőmérsékleten tartják ezalatt a várakozás alatt, ami azt eredményezi, hogy több anyag szivárog ki, és ismét tönkreteszi a műanyagot a fúvókában. Erre azért van szükség, hogy az anyag ne hűljön tovább, mint amit Cura várt a szeletelés során, ami nagyobb hőmérséklet-különbséget jelentene, mint amit Cura várt, és így a következő alkalommal még hosszabb várakozási időhöz vezet. Ez egy kifutó hatáshoz vezetne, ahol az előrejelzés minden réteggel rosszabb lesz, ezért Curának melegen kell tartania az előző anyagot, amíg el nem éri a másik fúvóka hőmérsékletét.

A tényleges felmelegedési sebesség nem egy állandó sebesség fok/másodpercben. Valószínűbb, hogy ez a fúvóka aktuális hőmérséklete és az építési térfogat hőmérséklete közötti különbségtől függ. Mint ilyen, hidegben gyorsabban melegszik fel, és amikor megközelíti a célhőmérsékletet, lassabban melegszik fel. Ebben nagy szerepe van a nyomtató PID szabályozójának is. A legtöbb szabályozó lelassítja a fűtést közvetlenül a célhőmérséklet elérése előtt, hogy elkerülje a túllépést. Ha ezt hangolja, próbálja meg úgy hangolni, hogy megméri a [készenléti hőmérsékletről](../material/material_standby_temperature.md) a [kezdeti nyomtatási hőmérsékletre](../material/material_initial_print_temperature.md) való felmelegedés idejét. Ez a legfontosabb pálya, amelyet Cura megpróbál megjósolni. Kis nyomatok készítésekor a felfűtési sebességet kissé csökkentheti, hogy beállítsa, hogy ne a készenléti hőmérsékletről induljon, hanem magasabb hőmérsékletről.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
