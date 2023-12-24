# Kereszt 3D zsebméret

A Cross 3D [kitöltési mintát](../infill/infill_pattern.md) a rugalmas nyomatok megkönnyítésére készítették. A minta 4 irányú kereszteződéseket tartalmaz, bár ezek nagyon merevek. Ez a beállítás azt eredményezi, hogy a minta elkerüli a keresztezést, hogy bizonyos helyeken ne legyen túl merev. Ezáltal a minta levegőzsebeket hagy a kereszteződésben. Ez a beállítás határozza meg a zseb méretét.

<!--screenshot {
"image_path": "infill_pattern_cross_3d.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cross_3d",
    "cross_infill_pocket_size": 2
},
"colours": 32
}-->

<!--screenshot {
"image_path": "cross_infill_pocket_size_0_5.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cross_3d",
    "cross_infill_pocket_size": 0.5
},
"colours": 32
}-->

![Az alapértelmezett zsebméret 2 mm](../images/infill_pattern_cross_3d.png)![A zseb mérete 0,5 mm](../images/cross_infill_pocket_size_0_5.png)

A minta változtatja a távolságot a négyirányú kereszteződés körül. Ez a beállítás határozza meg a rétegek zsebének méretét, amikor a vonalak teljesen összeérnek. A zseb maximális méretét a kitöltés sűrűsége határozza meg. A zseb mérete nem lesz nagyobb, mint a kitöltési vonal távolságának kétszeresének négyzetgyöke. Ha nagyobb értéket adunk meg, annak nincs hatása, de nagyobb értékeket is be lehet adni, hogy nagyobb zsebméreteket tegyen lehetővé [, fokozatos kitöltés](../infill/gradual_infill_steps.md) vagy [változó kitöltési sűrűség](cross_infill_density_image.md) esetén.

A beállítás értékének növelése függőleges irányban gyengíti a kitöltést, és jobban szétterül a szilárdság körül, hogy egyenletesebb szilárdságeloszlást hozzon létre.
