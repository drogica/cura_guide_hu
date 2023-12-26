# Villámkitöltés túlnyúlási szöge

A villámkitöltés csak a modell felső részét fogja megtámasztani belülről, ahol túlnyúlik. Ez a beállítás határozza meg a túlnyúlás szögét, amelyet a modell belsejéből villámlik meg.

<!--screenshot {
"image_path": "lightning_infill_support_angle_30.png",
"models": [{"script": "half_sphere.scad"}],
"camera_position": [130, 87, 47],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 30
},
"colours": 64
}-->

<!--screenshot {
"image_path": "lightning_infill_overhang_angle_70.png",
"models": [{"script": "half_sphere.scad"}],
"camera_position": [130, 87, 47],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 30,
    "lightning_infill_overhang_angle": 70
},
"colours": 64
}-->

![Az akár 30°-os túlnyúlás támasz nélkül marad](../images/lightning_infill_support_angle_30.png)![70°-ig nincs alátámasztva, így csak a gömb legtete marad megtámasztva](../images/lightning_infill_overhang_angle_70.png)

Ennek a szögnek a növelése csökkenti a keletkező kitöltés mennyiségét. A felső felület kevésbé lesz alátámasztva, ha nem túl meredek a túlnyúlás. Ez időt és anyagot takarít meg, de a felső felület helyenként megereszkedhet. Az eredmény lehet [párnázás](../troubleshooting/pillowing.md) vagy általában durvább felület.

A [Lightning Infill Support Angle](lightning_infill_support_angle.md) szülőbeállítással ellentétben ez a beállítás nem befolyásolja magának a kitöltési mintának a túlnyúlását.
