# Abszolút extruder elsődleges pozíciója

Ha a [prime blob-ot](../platform_adhesion/prime_blob_enable.md) használja, ennek a prime eljárásnak a pozíciója beállítható egy [X](../platform_adhesion/extruder_prime_pos_x.md) és [Y](../platform_adhesion/extruder_prime_pos_y.md) pozícióval. Ez a beállítás határozza meg, hogy ez a pozíció az alaplemezen, vagy a nyomtató aktuális pozíciójához viszonyítva.

Ha ez a beállítás engedélyezve van, az X és Y koordináták egy bizonyos rögzített pozícióra vonatkoznak az építőlemezen. Az extruder mindig oda fog mozogni, hogy elsődleges blobot hozzon létre.

Ha ez a beállítás le van tiltva, az X és Y koordináták ahhoz a pozícióhoz viszonyítva vannak, amely a fúvóka helyzetében van, amikor először vált át az extruderre. Az első extruder esetében ez lenne a [0,0] koordináta. A többi extruder esetében ez a kiindulási helyzetük az extruder definíciós fájljában meghatározottak szerint. Ez a kiindulási helyzet relatív is lehet.

Erősen javasolt az abszolút elsődleges pozíció használata. Az abszolút elsődleges pozíció garantáltan mentes a nyomat más részeivel való ütközéstől, mivel nem lehet tárgyakat elhelyezni az építőlemezen. A relatív alapozó pozíció bárhol az építőlemezen végződhet, és ennek eredményeként előfordulhat, hogy valahol az első réteg tetejére alapoz. A relatív elsőbbségi pozíció használatával némi utazási időt takaríthat meg, de ez tényleg nem éri meg a kockázatot.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
