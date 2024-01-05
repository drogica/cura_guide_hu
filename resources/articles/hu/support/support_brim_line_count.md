# Támogassa a peremvonalak számát

Ez a beállítás beállítja a kontúrok számát, amelyek a támasztóperem támasztóterületén belül lesznek megrajzolva. Több vonallal a perem szélesebb lesz.

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

![5 peremvonal](../images/support_brim_2mm.png)![10 peremvonal](../images/support_brim_4mm.png)

A több peremvonal növeli a támaszték tapadását az építőlemezhez, és csökkenti a támaszték vetemedését. Ennek eredményeként a tartó stabilabb lesz, ami javítja a nyomat megbízhatóságát.
