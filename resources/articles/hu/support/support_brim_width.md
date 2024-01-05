# Támogassa a peremszélességet

Ez a beállítás beállítja a tartóperem szélességét. Szélesebb támasztóperem esetén több kontúr rajzolódik ki a támasztóterületen belül a jobb tapadás érdekében.

<!--screenshot {
"image_path": "support_brim_2mm.png",
"models": [{"script": "gazebo2.scad"}],
"camera_position": [-74, 38, -137],
"settings": {
    "support_enable": true,
    "support_use_towers": false,
    "support_brim_enable": true,
    "support_brim_width": 2
},
"colours": 64
}-->

<!--screenshot {
"image_path": "support_brim_4mm.png",
"models": [{"script": "gazebo2.scad"}],
"camera_position": [-74, 38, -137],
"settings": {
    "support_enable": true,
    "support_use_towers": false,
    "support_brim_enable": true,
    "support_brim_width": 4
},
"colours": 64
}-->

![2 mm széles](../images/support_brim_2mm.png)![4 mm széles](../images/support_brim_4mm.png)

A szélesebb perem növeli a támaszték tapadását az alaplaphoz, és csökkenti a támaszték elhajlását. Ennek eredményeként a tartó stabilabb lesz, ami javítja a nyomat megbízhatóságát.
