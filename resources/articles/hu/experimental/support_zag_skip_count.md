# Támogatás Chunk Line Count

Ha a támogatás [darabokra van felosztva](support_skip_some_zags.md) , ez a beállítás határozza meg, hogy hány támogatási sor kerüljön egy darabba.

<!--screenshot {
"image_path": "support_skip_some_zags.png",
"models": [{"script": "rack.scad"}],
"camera_position": [0, 184, 10],
"settings": {
    "support_enable": true,
    "support_pattern": "zigzag",
    "support_skip_some_zags": true,
    "support_skip_zag_per_mm": 20
},
"colours": 32
}-->

![Minden darab 8 sort tartalmaz](../images/support_skip_some_zags.png)

A kisebb darabokat általában könnyebb leszakítani, mint a nagyobb darabokat. Kevesebb felületet kell ragasztani a modellhez, így kevesebb erőre lesz szükség a támaszték elhúzásához. Ugyanakkor több darabot is el kell távolítani, így ha a támasz lehúzása általában nem nehéz, ez megnövelheti a támaszték lehúzását. Ezután minden egyes darabot külön kell lehúzni, ahelyett, hogy az összes támasztékot egy nagy darabban húznánk le.

Ha a darabokat nagyon kicsire készítik, a tartószerkezet szerkezeti integritása sérülhet. A támasztómintázat jobban fog hasonlítani a vonalmintázathoz, aminek nagyobb az esélye a felborulásra. Ez több húrozást és rosszabb túlnyúlási minőséget eredményezne azokon a helyeken, ahol a támaszték felborult.
