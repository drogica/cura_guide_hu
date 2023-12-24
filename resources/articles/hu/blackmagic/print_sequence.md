# Nyomtatási sorrend

Ha több modellt helyez el az építőlemezre, ez határozza meg az objektumok rétegeinek nyomtatási sorrendjét. Két lehetőség van.

## Egyszerre

Minden objektum egyszerre lesz kinyomtatva, ami azt jelenti, hogy a rétegek alulról felfelé az összes objektumnál egyszerre lesznek kinyomtatva. Minden objektumból egy réteget nyomtat, mielőtt a következő rétegre lépne.

Ennek két fő előnye van:

- Az előző rétegnek több ideje van lehűlni, ami jobb minőséget eredményez kis tárgyak nyomtatásánál.
- A teljes build kötet felhasználható a nyomtatáshoz.

## Egyenként

Az objektumok egyenként kerülnek kinyomtatásra, ami azt jelenti, hogy egy objektum minden rétegét kinyomtatja, majd visszakerül az építőlemezre a következő objektum nyomtatásához.

Ennek a módnak a fő előnyei a következők:

- Ha a nyomtatás bármilyen okból meghiúsul, minden olyan objektum, amely a hiba előtt elkészült, teljesen használható.
- Kevesebb mozgásra van szükség a modellek közötti oda-vissza mozgáshoz. Ez némi nyomtatási időt takarít meg, és csökkenti a hegek számát azon a felületen, ahol a fúvóka kilépett és behatolt a tárgyba.

Ez a mód azonban néhány megkötéssel jár, hogy elkerülje a fej és a portál ütközését a modellel.

- Nem nyomtathat a nyomtató portálmagasságánál magasabb objektumokat. A portál magassága a nyomtató Gépbeállítások párbeszédpaneljén állítható be. Ez a portálmagasság azt jelzi, hogy mekkora függőleges távolság van a fúvóka hegye és a nyomtatófejet hordozó rendszer között. Ennek a korlátozásnak az az oka, hogy a nyomtatófejnek le kell mozdulnia az építőlemezre a második objektum nyomtatásához. Ez azt jelenti, hogy az első objektumot eltalálhatja a portál a második objektum nyomtatása közben. Elméletileg megengedhető, hogy az utolsó nyomtatott objektum magasabb legyen, mint a portál, de az egyszerűség kedvéért Cura egyébként sem engedi meg.
- Az objektumokat távolabb kell elhelyezni egymástól, hogy a nyomtatófej ne ütközzen oldalra a korábban nyomtatott modellekkel.
- Az objektumok nyomtatási sorrendje rögzített és optimalizált, hogy lehetővé tegye az objektumok egymáshoz való szorosabb kinyomtatását. Ha a nyomtatófej nem szimmetrikus, ez sok helyet takaríthat meg az építőlemezen.

**Egyenként csak egyszeri extrudálással érhető el. Ha több extrudálású nyomtatót használ, akkor egy kivételével az összes extrudert deaktiválnia kell, hogy ez a beállítás megjelenjen.**
