# Villámkitöltő támasztószög

A Lightning kitöltési minta csak a nyomat belülről történő támogatására szolgál. Ez a beállítás határozza meg a maximális túlnyúlási szöget, nem csak az általa alátámasztott felületeken, hanem magában a kitöltésben is. Ennek a beállításnak a csökkentése több kitöltést generál. Növelése csökkenti a kitöltés mennyiségét.

A minta belülről támogatja a nyomat felső oldalát, de csak a felső oldalt, amely jelentősen túlnyúlik, ennél a szögnél jobban. A mintának vannak olyan végpontjai is, amelyek bizonyos szögben túlnyúlnak, hogy elágazó fastruktúrát hozzanak létre, és ennek az elágazó szerkezetnek az oldalai egy belső szöggel rendelkeznek, hogy bizonyos területeken tovább érjenek. A túlnyúlás e három aspektusa külön-külön is szabályozható a [villámkitöltés túlnyúlási szöge](lightning_infill_overhang_angle.md) , [a villámfeltöltési aszalt szög](lightning_infill_prune_angle.md) és [a villámfeltöltés kiegyenesítő szög](lightning_infill_straightening_angle.md) beállításaival.

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
"image_path": "lightning_infill_support_angle_60.png",
"models": [{"script": "half_sphere.scad"}],
"camera_position": [130, 87, 47],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 60
},
"colours": 64
}-->

![Alacsony túlnyúlási szög esetén sok támogatásra van szükség](../images/lightning_infill_support_angle_30.png)![Nagy kinyúlási szög esetén meredek túlnyúlások megengedettek](../images/lightning_infill_support_angle_60.png)

Ennek a beállításnak a növelése nagymértékben csökkenti a szükséges anyagmennyiséget, és csökkenti a nyomtatási időt. Ez azonban megereszkedést is okoz. Ez a megereszkedés a modell belsejében található, így nem látszik azonnal. Ha azonban a [felső vastagság](../top_bottom/top_thickness.md) nem elegendő, [az párnázáshoz](../troubleshooting/pillowing.md) vezethet. Mivel a kitöltésben a belső szögek is jobban kilógnak, valószínű, hogy a kitöltés magasabban kezdődik a falak mentén.
