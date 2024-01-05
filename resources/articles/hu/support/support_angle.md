# Támasz túlnyúlási szög

A túlnyúlási szög befolyásolja, hogy mennyi anyagot helyeznek le a nyomat alátámasztására. A szög azt a minimális szöget jelöli, amelyet megtámaszt.

**A beállítás értékének csökkentése több támogatást generál.**

<!--screenshot {
"image_path": "support_angle_low.png",
"models": [{"script": "duct.scad"}],
"camera_position": [136, 10, 10],
"camera_lookat": [0, 10, 10],
"settings": {
    "support_enable": true,
    "support_join_distance": 0.1,
    "support_angle": 40
},
"colours": 64
}-->

<!--screenshot {
"image_path": "support_angle_high.png",
"models": [{"script": "duct.scad"}],
"camera_position": [136, 10, 10],
"camera_lookat": [0, 10, 10],
"settings": {
    "support_enable": true,
    "support_join_distance": 0.1,
    "support_angle": 75
},
"colours": 64
}-->

<!--screenshot {
"image_path": "support_angle_prepare_mode.png",
"models": [{"script": "duct.scad"}],
"camera_position": [113, 77, 0],
"layer": -1
}-->

![Az alacsony túlnyúlási szög nagyobb alátámasztást biztosít](../images/support_angle_low.png)![A nagy túlnyúlási szög kevesebb alátámasztást eredményez](../images/support_angle_high.png)![A támogatott területek piros színnel vannak jelölve](../images/support_angle_prepare_mode.png)

Ennek a beállításnak a csökkentésével a nyomtató több nyomtatott részt támogat, még a meredekebb felületeket is, amelyek nyomtatás közben nem ereszkednek meg. Ha a támaszték olyan részeket támaszt, amelyeket nem kell alátámasztani, az szükségtelenül megnöveli a nyomtatási időt és az anyagfelhasználást, valamint hegeket hoz létre ott, ahol a támasz hozzáért a nyomathoz.

Néha azonban csökkenteni kell az alátámasztási szöget, hogy megakadályozzuk az anyag túlzott megereszkedését. Általában javítja az utolsó rész méretpontosságát, és a túlnyúlásokat is jobban kinézi.

Amikor a támogatással dolgozik, érdemes megnézni, hogyan néz ki a támogatás az Előnézet szakaszban. Ott láthatja, hol fog ténylegesen támogatást generálni. Ennek a beállításnak a módosítása az egyik rendelkezésére álló eszköz annak kiszűrésére, hogy pontosan hol fog támogatást generálni.
