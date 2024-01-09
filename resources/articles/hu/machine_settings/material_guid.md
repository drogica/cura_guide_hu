# Anyag GUID

Ez a beállítás egyedi azonosítót tartalmaz a nyomtatóba betöltött orsón lévő anyaghoz. Ez egyedileg azonosítja a nyomtatóba betáplált műanyagot, beleértve a gyártót és a színt. Ez ugyanaz lesz az azonos anyagú különböző orsók között. Alapvetően minden egyes webáruházban megjelenő termék egyedi azonosítót kap. A Cura ezt az egyedi azonosítót két célra használja: a konfiguráció szinkronizálására a nyomtatón található tartalommal (ha a nyomtató csatlakozik a Curához), valamint az azonos anyaghoz tartozó profilok csoportosítására.

Ha egy Ultimaker nyomtató csatlakozik a Curához a hálózaton vagy az interneten keresztül, a nyomtató a Cura számára egy GUID-listát ad az aktuálisan a nyomtatóba betöltött anyagokhoz. A Cura ezeket a GUID-ket egyezteti a profiljaiban lévő GUID-ekkel, ami alapján tudja, hogy mely profilokat jelenítse meg a felhasználó számára.

Azt is használják, hogy csoportosítsa az elérhető minőségi szinteket egy bizonyos anyaghoz. A Cura profilrendszere nagyon összetett, és ez az egyik különlegessége: Általában a Cura megjeleníti az aktuális anyagtípushoz elérhető összes minőségi profilt. Ez azt jelenti, hogy ha egy bizonyos gyártó azt jelzi, hogy az anyaga egyfajta PLA, akkor a PLA összes minőségi profilja elérhető lesz. Ha azonban van olyan minőségi profil, amely az aktuális anyagot GUID szerint határozza meg, akkor csak az a minőségprofil lesz elérhető. Ez lényegében azt jelenti, hogy vannak speciálisan erre az izzószálra szabott profilok, és az általános profilokat többé nem szabad megjeleníteni.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
