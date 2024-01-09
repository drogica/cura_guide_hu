# Offset Extruderrel

Ez a beállítás határozza meg, hogy Curának kell-e koordinátákat írnia a nyomtatófejhez vagy a fúvókához.

Ha a nyomtatónak csak egyetlen fúvókája van, akkor a nyomtató koordinátarendszere valószínűleg a fúvókához igazodik. Ez azt jelenti, hogy az [50,50] pozícióba mozgatva a fúvóka hegye ténylegesen ebbe a pozícióba kerül. Ha a nyomtatónak több fúvókája van, és ezek a fúvókák egymás mellett vannak a nyomtatófejben, akkor ez számít.

Egyes nyomtatók ugyanarra a helyre mozgatják a nyomtatófejet, függetlenül attól, hogy éppen melyik fúvóka van aktiválva. Míg a g-kód utasíthatja a nyomtatót, hogy lépjen az [50,50] pozícióba, az aktuálisan aktív fúvóka hegye a [68,50] pozícióba kerülhet, mivel például 18 mm-re van a nyomtatótól jobbra. első fúvóka. Ha ez a helyzet, akkor ezt a beállítást engedélyezni kell.

Más nyomtatók automatikusan úgy állítják be a nyomtatófej helyzetét, hogy az aktív fúvóka a g-kódban jelzett pozícióba kerüljön. Ez azt jelenti, hogy ha a g-kód arra utasítja a nyomtatót, hogy lépjen az [50,50] pozícióba, akkor az éppen aktív extruder ebbe a pozícióba mozog. Maga a nyomtatófej egy kicsit oldalra mozdulna, hogy ott helyezze el az aktív extrudert. Ha nyomtatója így viselkedik, ezt a beállítást le kell tiltani.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
