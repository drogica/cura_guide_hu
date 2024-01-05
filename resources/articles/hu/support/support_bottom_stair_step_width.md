# Támasz lépcsőfokok maximális szélessége

Ha [a Support Placement](support_type.md) beállítása „Mindenhol”, a támogatás a modellen nyugszik. Ennek ellenére nem fogja pontosan követni a modell körvonalait. Ehelyett a tartó alsó oldala lépcsőzetes mintát kap. Így a támogatás csak néhány helyen létesít kapcsolatot a modellel.

Ez a beállítás határozza meg ezen lépések maximális szélességét. A lépcső általában olyan szélességet kap, amely követi a modell felületét egy adott [támasztólépcső lépcsőmagasság](support_bottom_stair_step_height.md) értékkel. Ha azonban ez túl széles, a szélesség a támasztólépcső lépcsőfokának maximális szélességére korlátozódik. Ezután követi a modell felületét a lépés hátralévő részében.

<!--screenshot {
"image_path": "support_bottom_stair_step_width.png",
"models": [{"script": "standing_ring.scad"}],
"camera_position": [0, 136, 10],
"camera_lookat": [0, 0, 10],
"settings": {
    "support_enable": true,
    "support_bottom_stair_step_height": 1,
    "support_bottom_stair_step_width": 0.7
},
"colours": 64
}-->

![A lépcsőfokok szélessége korlátozott, ami a modell követését eredményezi](../images/support_bottom_stair_step_width.png)

Ezt a beállítást általában arra a maximális távolságra kell beállítani, amelyet az anyag áthidalhat anélkül, hogy veszélyeztetné a felette lévő támasztóvonalak stabilitását. A beállítás csökkentése azt eredményezi, hogy a támasz gyakrabban követi a modellt, így a támogatás stabilabb lesz. A beállítás növelésével a támasz gyakrabban ragaszkodik a támasztó lépcsőfok magassága beállított értékéhez, így a támasz könnyebben eltávolítható a modellből.
