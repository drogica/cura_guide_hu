# Huzat pajzs magassága

Ha a [Huzatpajzs korlátozása](draft_shield_height_limitation.md) beállítása "Korlátozott", ez a beállítás lehetővé teszi annak megadását, hogy a huzatpajzs milyen magasságban legyen korlátozva.

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

![A huzatvédő pajzs 20 mm-re korlátozódik](../images/draft_shield_height_limitation.png)

A nyomat alsó oldala a legérzékenyebb a hőmérséklet-ingadozásokra. Itt történik a legtöbb vetemedés, ha a helyiség hideg, és ez a vetemedés azt okozhatja, hogy a nyomat elengedi az építőlemezt. Ezzel a beállítással kiválaszthatja, hogy milyen magasságban korlátozza a nyomtatást. A huzatvédő pajzs magasságának csökkentése időt és anyagot takaríthat meg. A huzatvédő pajzs ezután is védi a nyomat alsó oldalát, és blokkolja a levegő konvekcióját a felszálló forró levegő miatt (bizonyos mértékben).

A huzatpajzs soha nem nyomtatható magasabbra, mint maga a tárgy.
