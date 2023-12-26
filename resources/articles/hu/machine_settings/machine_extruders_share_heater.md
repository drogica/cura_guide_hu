# Extruderek Share Heater

Ezzel a beállítással jelezheti, hogy a nyomtatóban lévő összes fúvókán ugyanaz a fűtőelem van. A Cura nem hűti le bizonyos extruderek fúvókáit, ha azok inaktívak. Mivel közös a fűtőberendezésük, feltételezhető, hogy az extrudernek melegnek kell maradnia ahhoz, hogy egy másik extruder folytathassa az extrudálást.

Erre leggyakrabban keverőfúvókáknál van szükség, ahol több filamentet táplálnak ugyanabba a fúvókába. Ennek a fúvókának csak egy fűtőteste van, amely felmelegíti, amelyik izzószál éppen a fúvókában van. Ha a Cura az egyes izzószálak fűtését külön szabályozná, egyidejűleg megpróbálná melegen tartani az aktív izzószál fúvókáját, miközben a többi izzószálat a [készenléti hőmérsékletre](../material/material_standby_temperature.md) hűti le. Ez lehetetlen, és vagy csak az első izzószálnál melegszik fel, vagy állandóan készenléti hőmérsékleten nyomtat, ha a firmware csak az egyik fúvókára adja ki a fűtési parancsokat, függetlenül attól, hogy melyik szerszámra irányulnak. Ha jelzi Curának, hogy az extrudereknek közös a fűtőberendezése, ez megelőzi ezt a problémát. A Cura többé nem engedi a fúvókát készenléti hőmérsékletre, és nem ad ki fűtési parancsot egyetlen extruderre sem.

Cura nem feltétlenül feltételezi, hogy ha az extrudereknek közös a fűtőberendezése, akkor egy fúvókán is osztoznak. Ehhez van egy külön beállítás, amely jelzi, hogy [az extruderek közös fúvókán vannak](machine_extruders_share_nozzle.md) .

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában. Ehhez a beállításhoz van egy jelölőnégyzet a nyomtatóbeállítások párbeszédpanelen, amely a hozzáadott nyomtatók listájában található a beállítások párbeszédablakban.**
