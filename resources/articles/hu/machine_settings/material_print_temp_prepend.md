# Tartalmazza az építési lemez hőmérsékletét

Ez a beállítás közli a szeletelő háttérrel, hogy írjon-e felépítési lemez hőmérsékleti parancsokat a nyomtatás megkezdéséhez a kezdő g-kód előtt. A szelet indításakor automatikusan beáll.

A legtöbb műveletnél [a g-kód indításakor](machine_start_gcode.md) célszerű az építőlemezt a megfelelő hőmérsékletre melegíteni a nyomtatáshoz. A nyomtatódefiníciók tervezésének megkönnyítése érdekében a Cura automatikusan felmelegíti az építőlemezt a start g-kód végrehajtása előtt. Ha azonban a start g-kód bármilyen hivatkozást tartalmaz az építőlemez hőmérsékleti beállítására, akkor az nem melegíti fel automatikusan az építőlemezt.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában. A módosításnak szintén nincs hatása, mivel a Cura automatikusan módosítja.**
