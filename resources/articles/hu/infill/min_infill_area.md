# Minimális kitöltési terület

Ez a beállítás azt eredményezi, hogy a nagyon kis darabokat a héj mintázatával töltik ki, nem pedig a kitöltési mintával, így teljesen szilárdak.

<!--screenshot {
"image_path": "min_infill_area_disabled.png",
"models": [{"script": "stature.scad"}],
"camera_position": [-64, 224, 82],
"settings": {
    "wall_line_count": 0,
    "min_infill_area": 0
},
"colours": 32
}-->

<!--screenshot {
"image_path": "min_infill_area_150.png",
"models": [{"script": "stature.scad"}],
"camera_position": [-64, 224, 82],
"settings": {
    "wall_line_count": 0,
    "min_infill_area": 150
},
"colours": 32
}-->

![0-ra állítva ennek a modellnek a vékony lábai megtelnek kitöltéssel](../images/min_infill_area_disabled.png)![150-re állítva a lábak megtelnek bőrrel](../images/min_infill_area_150.png)

Előfordul, hogy nagyon kis üreges területeket nem lehet megfelelően kitölteni a kitöltéssel, mivel a kitöltő vonalak olyan rövidek lennének, hogy az anyagnak nincs ideje megfelelően folyni. Ez a beállítás inkább bőrrel tölti fel őket, ami erősebbé teszi őket, és megakadályozza a határvonalat a bőr és a kitöltés között.

A beállítás 0-ra állítása gyakorlatilag letiltja ezt a funkciót.
