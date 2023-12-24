# WP stratégia

A drótnyomtatás megbízhatósága szempontjából a legfontosabb szempont azok a csatlakozási pontok, ahol a keret rétegei csatlakoznak egymáshoz. Számos stratégia létezik ezeknek a kapcsolatoknak a megerősítésére. Ez a beállítás lehetővé teszi a nyomtató által használt stratégia kiválasztását.

## Kompenzálni

Ennek a stratégiának a használatakor a nyomtató megpróbálja kompenzálni az anyag megereszkedését okozó tényezőket. Mivel az anyag megolvadva jön ki a fúvókán, egy kicsit leesik, mielőtt megszilárdul, és a fúvóka mozgásával együtt húzódik. Ez a stratégia úgy deformálja a keret rétegeit összekötő fűrészfog-mintát, hogy az remélhetőleg ismét a megfelelő helyre kerül.

Két kompenzációs tényező áll rendelkezésre: az egyik, amely csak függőlegesen deformálja a fűrészfog mintázatát, hogy [kompenzálja a megereszkedést](wireframe_fall_down.md) , és egy, amely a fűrészfog mintázatát átlós irányban deformálja, hogy [kompenzálja az anyagot a fúvókával együtt húzva](wireframe_drag_along.md) .

## Csomó

Ha ezt a stratégiát választja, akkor minden egyes fűrészfog tetején egy kis felfelé és hátrafelé mozgás történik, hogy ott "csomót" képezzen az anyag. A csomó célja, hogy a tetején lévő vízszintes gyűrűnek helyet biztosítson a fűrészfog mintázatához való rögzítéshez. A csomó oldalról oldalra kissé változhat, így ha a vízszintes gyűrűt nem nagyon pontosan helyezik le, akkor is nagyobb az esélye annak, hogy egymáshoz tapadnak. Ezenkívül a csomó miatt a felfelé irányuló vonal kissé tovább nyúlik felfelé, aminek következtében a vízszintes gyűrű rászorul rá. És végül, a csomó némi szivárgást is produkál a visszahúzódás hiánya miatt ebben az utazási lépésben. Ez egy foltot hoz létre, amelyen a vízszintes gyűrű jobban tud feküdni.

![Hol húzzák a csomót, és mit jelent a mérete](../images/wireframe_top_jump.svg)

Ennek a "csomónak" a mozgása utazási lépések sorozata:

1. Először is, a fúvóka kissé felfelé és hátrafelé mozog.
2. Ha [késés](wireframe_top_delay.md) van a tetején, a fúvóka a beállított késleltetés időtartamára leáll. Ez a szünet a csomó mozgásának végén történik.
3. Harmadszor, a fúvóka visszamozdul a szokásos magasságba. Ugyanakkor a fúvóka előre és távolodik a függőleges vonaltól.

## Visszavonás

Ha ezt a stratégiát választja, az anyag minden felfelé irányuló mozdulat után visszahúzódik a fűrészfog-minta nyomtatása közben. Az ötlet az, hogy az anyag visszahúzásával a drót letörik. Ez csökkenti azt a hatást, hogy az anyag a fúvóka mozgásával együtt húzódik, mivel az előző vonal már nincs rögzítve a fúvókához. Ezután a fúvóka 1 milliméteres kis ugrást tesz, és az átlós mozgást folytatja lefelé az alsó réteg felé.

Ennek a stratégiának az egyik fő hátránya, hogy az átlós lefelé vonal szintén nincs rögzítve. Ez gyakorlatilag használhatatlanná teszi az extrudálást ezen a vonalon. Az anyag egyszerűen foltként végzi az alsó réteget. Az anyag is nagyobb csiszolási hatásnak van kitéve, mivel az anyag ide-oda visszahúzódik anélkül, hogy nagy extrudálás történik közben. Mindez szintén sok időt vesz igénybe.
