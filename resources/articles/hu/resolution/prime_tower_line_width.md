# Prime Tower vonal szélessége

Ez a beállítás határozza meg azon vonalak szélességét, amelyekkel az elsődleges torony megrajzolódik.

<!--screenshot {
"image_path": "prime_tower_line_width.png",
"models": [
    {"script": "cube.scad"},
    {
        "script": "cube.scad",
        "object_settings": {"extruder_nr": 1},
        "transformation": ["translateX(40)"]
    }
],
"camera_position": [475, -419, 131],
"camera_lookat": [475, -465, 20],
"settings": {
    "prime_tower_enable": true,
    "[1]prime_tower_line_width": 0.8
},
"colour_scheme": "material_colour",
"colours": 64
}-->

![A kék anyag vonalszélessége nagyobb, mint a sárga anyagé](../images/prime_tower_line_width.png)

Ha vastagabb vonalszélességet választ, az elsődleges torony néha gyorsabban nyomtat. Ha az egyik kontúrral extrudált térfogat elég nagy, a vonalszélesség növelése szükségtelenné tesz egy újabb hurkot. A vonalszélesség túlzott növelése azonban gyengítheti az alaptornyot, mivel nem lehet elég gyorsan extrudálni elég anyagot.
