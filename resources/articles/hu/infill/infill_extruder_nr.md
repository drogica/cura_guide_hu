# Töltse ki az extrudert

Ez a beállítás határozza meg, hogy melyik extrudert használják a kitöltőanyag nyomtatásához. Csak több extruderrel rendelkező nyomtatókhoz érhető el.

<!--screenshot {
"image_path": "infill_extruder_nr.png",
"models": [
    {
        "script": "gear.scad",
        "object_settings": {"extruder_nr": 3}
    }
],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_extruder_nr": 1
},
"colour_scheme": "material_colour",
"colours": 32
}-->

![A modell héja ezüst anyaggal, a betét pedig kék anyaggal kerül nyomtatásra](../images/infill_extruder_nr.png)

Ha a nyomtatója más-más fúvókát tud használni az egyes extrudersorokhoz, a nagyobb fúvókamérettel történő nyomtatás növeli a nyomtatási sebességet és szilárdságot anélkül, hogy a héj vizuális minőségét akadályozná.
