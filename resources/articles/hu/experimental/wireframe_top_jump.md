# WP csomó mérete

Ha a [drótnyomtatási stratégia](wireframe_strategy.md) „Csomó”-ra van állítva, akkor minden egyes fűrészfog tetején egy kis felfelé és hátrafelé irányuló mozgás történik. Ez a beállítás konfigurálja a mozgás nagyságát.

![Hol húzzák a csomót, és mit jelent a mérete](../images/wireframe_top_jump.svg)

Ennek a "csomónak" a mozgása utazási lépések sorozata:

1. Először is, a fúvóka felfelé mozdul a beállítás által jelzett távolsággal. Ugyanakkor a fúvóka ennek a távolságnak a felével hátrafelé fog mozogni.
2. Ha [késés](wireframe_top_delay.md) van a tetején, a fúvóka a beállított késleltetés időtartamára leáll. Ez a szünet a csomó mozgásának végén történik.
3. Harmadszor, a fúvóka visszamozdul a szokásos magasságba. Ugyanakkor a fúvóka a csomó méretének 1,5-szeresével halad előre, és az ebben a beállításban jelzett távolságra kerül a függőleges vonaltól távolodva.

A csomó célja, hogy a tetején lévő vízszintes gyűrűnek helyet biztosítson a fűrészfog mintázatához való rögzítéshez. A csomó oldalról oldalra kissé változhat, így ha a vízszintes gyűrűt nem nagyon pontosan helyezik le, még mindig nagyobb az esélye annak, hogy egymáshoz tapadnak. Ezenkívül a csomó miatt a felfelé irányuló vonal kissé tovább nyúlik felfelé, aminek következtében a vízszintes gyűrű rászorul rá. És végül, a csomó némi szivárgást is produkál a visszahúzódás hiánya miatt ebben az utazási lépésben. Ez egy foltot hoz létre, amelyen a vízszintes gyűrű jobban tud feküdni.
