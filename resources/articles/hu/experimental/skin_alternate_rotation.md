# Alternatív bőrforgatás

Ha a felső és az alsó rész vonalakkal vagy cikk-cakk [mintával](../top_bottom/top_bottom_pattern.md) van kinyomtatva, a vonalak általában átlós irányban helyezkednek el, és a két irányt később váltogatják. Ha ez a beállítás be van kapcsolva, akkor négy irányban váltakozik: két átlós irányban, függőlegesen és vízszintesen.

![Négy irányban váltakozva](../images/skin_alternate_rotation.gif)

Ez a beállítás felülírja a [felső/alsó sor útvonalak](../top_bottom/skin_angles.md) beállítást. A viselkedés azonban ugyanaz. Valójában ez a beállítás teljesen emulálható a szögek `[45, 135, 0, 90]` megadásával.

Általában a nyomat a vonalak irányához képest hosszirányban a legmerevebb. Ha ez a beállítás nincs engedélyezve, akkor ez a két átlós irányban lesz, ami gyengébb lesz az ortográfiai irányokban. Ezeket az átlós irányokat azért választották, mert a 3D nyomtatók legáltalánosabb portálmechanizmusai több motort használnak az átlós mozgáshoz, ami lehetővé teszi, hogy gyorsabban gyorsuljanak ezekben az irányokban.

Ha ez a beállítás engedélyezve van, a vonalak irányai egyenletesebben oszlanak el. Ez egyenletesebben osztja el a tárgy erejét. Ez a tárgyat erősebbé teszi függőleges és vízszintes irányban, de kissé gyengébb az átlós irányban. Valamivel tovább tart az objektum nyomtatása.
