# Támogassa az extrudert

Ha a nyomtatója több extruderrel rendelkezik, akkor ezzel a beállítással kiválaszthatja, hogy ezek közül melyik extruderrel nyomtatja ki a tartószerkezetet.

<!--screenshot {
"image_path": "support_extruder_nr.png",
"models": [
    {
        "script": "question_stick_clip.scad",
        "transformation": ["rotateY(90)"],
        "object_settings": {"extruder_nr": 1}
    }
],
"camera_position": [134, 134, 113],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_use_towers": false,
    "support_extruder_nr": 3
},
"colour_scheme": "material_colour",
"colours": 64
}-->

![A támasz fehér anyaggal, míg a modell kékkel van nyomtatva](../images/support_extruder_nr.png)

Más típusú anyag használata általában megkönnyíti a támasztó eltávolítását anélkül, hogy ez veszélyeztetné a támasztó szilárdságát. A különböző anyagtípusok nem nagyon tapadnak egymáshoz, különösen, ha eltérő a zsugorodási arányuk.

Ezenkívül egyes anyagok nyomtatási támogatásra készültek. Szándékosan rendkívül törékennyé tehetők például, hogy könnyebben letörjenek. Egyes anyagok vízben vagy etanolban oldódnak, így akkor is eltávolíthatja a hordozót, ha nagyon közel van a modellhez nyomtatva.

A modell többi részétől eltérő extruderrel történő nyomtatás támogatása azonban megköveteli, hogy a nyomtató minden rétegben váltson anyagokat, ami megnövelheti a nyomtatási időt. Ha a hordozóanyag színe eltér az építőanyagtól, a nyomaton lévő támasztóanyag-maradványok nagyon jól láthatóak lehetnek.
