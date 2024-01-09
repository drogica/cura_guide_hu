# Végső nyomtatási hőmérséklet

Közvetlenül egy másik extruderre váltás előtt a fúvókát hagyják kissé lehűlni a végső nyomtatási hőmérsékletre. Valójában ez azt eredményezi, hogy a fúvóka valamivel korábban lehűl, mielőtt az extruder befejezné a nyomtatást. Olyan pillanatban kezd lehűlni, hogy a fúvóka várhatóan eléri a végső nyomtatási hőmérsékletet. Pontosan akkor éri el a végső nyomtatási hőmérsékletet, amikor az extruder átkapcsolása megtörténik. Ezt követően tovább hűl a készenléti hőmérséklet felé.

![A lehűlés megkezdésének pillanatát (előhűtés) úgy kell kiszámítani, hogy a fúvóka lehűljön a végső nyomtatási hőmérsékletre, amikor a fúvóka kapcsoló megtörténik](../images/temperature_regulation.svg)

Ha a végső nyomtatási hőmérséklet valamivel alacsonyabb, mint a normál nyomtatási hőmérséklet, a fúvóka nem szivárog ki annyira, amíg készenléti állapotban vár, miközben a másik extruder nyomtat.
