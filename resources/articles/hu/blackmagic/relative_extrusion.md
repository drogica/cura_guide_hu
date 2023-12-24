# Relatív extrudálás

A Cura utasításokat ír a nyomtatónak az objektum g-kódban történő kinyomtatására. Ezek az utasítások bizonyos pozíciókba mozgatják a nyomtatófejet, és összekapcsolják az adagolót. A Cura általában abszolút koordinátákként rögzíti a nyomtatófej koordinátáit és az adagoló elfordulását. Ha azonban ez a beállítás engedélyezve van, az adagoló koordinátái viszonylagosan rögzítésre kerülnek.

Ha ez ki van kapcsolva (azaz abszolút extrudálás), akkor az izzószál pozíciója a nyomtatás elején marad nulla koordinátaként. Az izzószál helyzete az egész fájlban növekszik, ahogy egyre több anyag extrudálódik, és a szálnak egyre távolabb kell mozognia a nyomtatás elején lévő kiindulási ponttól.

Ha azonban ez engedélyezve van, akkor a g-kód minden egyes sorában a kihúzás külön lesz írva, az előző sor pozíciójához képest. Ezután minden sor csak az adott sorhoz extrudált anyagmennyiséget tartalmazza.

A relatív kihúzás megkönnyíti a g-kód szerkesztését a létrehozása után. Ha extra anyagot kell extrudálni valahol a kettő között (vonalszakaszok hozzáadásához vagy eltávolításához vagy az áramlási sebesség beállításához), az új extrudálást egyszerűen fel kell írni a szerkesztett részben. Abszolút extrudálás használata esetén az adagoló pozícióját `G92` segítségével vissza kell állítani, hogy megbizonyosodjon arról, hogy minden további parancs helyes.

Ha azonban a g-kód feldolgozása során bármikor kerekítési hiba lép fel (Curában, a firmware-ben vagy a mozgásban), az abszolút kihúzás ezt automatikusan korrigálja a következő sorban. A relatív extrudálás során ez túlextrudáláshoz vagy alulextrudáláshoz vezet, bár rendkívül csekély mértékben.

Nem minden nyomtató firmware támogatja a relatív extrudálást.

**Abszolút extrudálás használata esetén a Cura továbbra is visszaállítja az izzószál helyzetét 10 méterenként, hogy elkerülje a firmware lebegőpontos kerekítési hibáit.**
