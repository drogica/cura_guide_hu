# Tartalmazza az anyaghőmérsékletet

Ez a beállítás közli a szeletelő háttérrel, hogy a fúvóka hőmérsékleti parancsait kell-e írnia a nyomtatás megkezdéséhez a kezdő g-kód előtt. A szelet indításakor automatikusan beáll.

A legtöbb műveletnél a [g-kód indításakor](machine_start_gcode.md) célszerű a fúvókát a megfelelő hőmérsékletre felmelegíteni a nyomtatáshoz. A nyomtatódefiníciók tervezésének megkönnyítése érdekében a Cura automatikusan felmelegíti a fúvókát a start g-kód végrehajtása előtt. Ha azonban a start g-kód bármilyen utalást tartalmaz a fúvóka hőmérséklet-beállítására, akkor a fúvókát nem melegíti fel automatikusan.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában. A módosításnak szintén nincs hatása, mivel a Cura automatikusan módosítja.**
