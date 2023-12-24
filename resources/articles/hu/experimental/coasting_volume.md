# Coasting Volume

Ez a beállítás határozza meg, hogy a kontúr vége előtt mennyivel hagyja abba az adagoló az anyag adagolását. A kifutás hossza azonban az anyag térfogatában van konfigurálva. Ez szorosabban kapcsolódik a fúvókakamrában lévő térfogathoz.

<!--screenshot {
"image_path": "coasting_enable.png",
"models": [{"script": "phone_holder.scad"}],
"camera_position": [0, -215, 117],
"minimum_layer": 1,
"structures": ["travels", "helpers", "shell", "infill", "starts"],
"settings": {
    "coasting_enable": true,
    "coasting_volume": 0.06,
    "z_seam_position": "backright"
},
"colours": 32
}-->

<!--screenshot {
"image_path": "coasting_volume_0_03.png",
"models": [{"script": "phone_holder.scad"}],
"camera_position": [0, -215, 117],
"minimum_layer": 1,
"structures": ["travels", "helpers", "shell", "infill", "starts"],
"settings": {
    "coasting_enable": true,
    "coasting_volume": 0.03,
    "z_seam_position": "backright"
},
"colours": 32
}-->

![0,06 mm³ anyagborítás](../images/coasting_enable.png)![0,03 mm³ anyag bevonat](../images/coasting_volume_0_03.png)

A szabadonfutó térfogat növelése azt eredményezi, hogy a fúvóka leállítja az extrudálást, mielőtt befejezné a kontúrt. Az eredmény az, hogy a vége felé nagyobb lesz az alulextrudálás. A gördítés funkciója a foltok kompenzálása a kontúr összevarrásakor, így a gördülő térfogat növelése kompenzálhatja a nagyobb foltokat.

Azonban, ha túlságosan megnöveljük a kifutó térfogatot, az erős alulextrudálást okoz a kontúr vége felé. Ez akár a kontúr után nyomtatott anyag alulextrudálásához is vezethet, mivel a fúvókára gyakorolt ​​nyomás ekkor még alacsony.
