# Gép szélessége

Ez a beállítás jelzi az X koordináták azon tartományát, amelyen keresztül a fúvóka(k) mozoghatnak. Ez alapvetően a nyomtató használható mérete.

Ez nem egyenlő a polcon lévő nyomtató tényleges szélességével. A tényleges nyomtatónak is van egy kerete vagy egy karja a felépítési térfogata körül, és ez a méret nem tartalmazza ezt a méretet. Csak az építési térfogat mérete, a koordináták, ahol a fúvóka mozoghat.

![Az építési térfogat méretei](../images/build_volume_dimensions.svg)

Ha több fúvókáról van szó, előfordulhat, hogy nem mindegyik fúvóka tudja elérni a teljes gyártási térfogatot. Egyes nyomtatók esetében, ha a nyomtatóban különböző fúvókák vannak eltolva egymáshoz képest, egyes fúvókák nem érnek el egészen az összeállítási kötet egyik oldaláig. Ez a beállítás csupán a térfogatok egyesítését jelzi, amelyet minden fúvóka el tud érni.

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában. A szélesség a nyomtatóbeállítások párbeszédablakban módosítható, amely a beállítások párbeszédpanelen található hozzáadott nyomtatók listájában található.**
