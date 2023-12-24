# Draft Shield Limitation

A huzatpajzs a modell teljes magassága felé vagy csak egy meghatározott magasságig nyomtatható. Ezzel a beállítással kiválaszthatja, hogy milyen magas legyen a huzatvédő pajzs.

<!--screenshot {
"image_path": "draft_shield_enabled.png",
"models": [{"script": "headphone_hook.scad"}],
"camera_position": [-56, 139, 305],
"settings": {
    "draft_shield_enabled": true
},
"colours": 32
}-->

<!--screenshot {
"image_path": "draft_shield_height_limitation.png",
"models": [{"script": "headphone_hook.scad"}],
"camera_position": [-56, 139, 305],
"settings": {
    "draft_shield_enabled": true,
    "draft_shield_height_limitation": "limited",
    "draft_shield_height": 20
},
"colours": 32
}-->

![A huzatvédő pajzs ugyanolyan magas, mint a modellé](../images/draft_shield_enabled.png)![A huzatvédő pajzs legfeljebb 20 mm magas](../images/draft_shield_height_limitation.png)

A nyomat alsó oldala a legérzékenyebb a hőmérséklet-ingadozásokra. Itt történik a legtöbb vetemedés, ha a helyiség hideg, és ez a vetemedés azt okozhatja, hogy a nyomat elengedi az építőlemezt. Ezzel a beállítással kiválaszthatja, hogy a huzatvédő pajzs magasságát egy bizonyos magasságra korlátozza. Ezzel némi időt és anyagot takaríthat meg. A huzatvédő pajzs ezután is védi a nyomat alsó oldalát, és blokkolja a levegő konvekcióját a felszálló forró levegő miatt (bizonyos mértékben).

A huzatpajzs soha nem nyomtatható magasabbra, mint maga a tárgy.
