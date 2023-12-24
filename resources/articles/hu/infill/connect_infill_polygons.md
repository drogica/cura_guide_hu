# Csatlakoztassa a kitöltési sokszögeket

Ha a kitöltés zárt hurkokból áll, ezek a zárt hurkok összeolvaszthatók egyetlen hurokká. Ennek engedélyezése kis kapcsolatokat hoz létre ott, ahol a sokszögek szomszédosak.

Ez a beállítás csak akkor érhető el, ha a kitöltés egymás melletti hurkokból áll. Ez azt jelenti, hogy vagy:

- A [kitöltési minta](infill_pattern.md) Kereszt vagy Kereszt 3D értékre van állítva.
- A kitöltő sorokat páros számra [szorozzák](infill_multiplier.md) .
- [A kitöltés körül legalább 2 extra fal](infill_wall_line_count.md) található.

<!--screenshot {
"image_path": "connect_infill_polygons_disabled.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "triangles",
    "infill_multiplier": 2,
    "zig_zaggify_infill": true,
    "connect_infill_polygons": false
},
"colours": 32
}-->

<!--screenshot {
"image_path": "connect_infill_polygons_enabled.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "triangles",
    "infill_multiplier": 2,
    "zig_zaggify_infill": true,
    "connect_infill_polygons": true
},
"colours": 32
}-->

![A többszörös kitöltési sorok esetén sok hurok van ebben a kitöltési mintában](../images/connect_infill_polygons_disabled.png)![A beállítás engedélyezése egyesíti a hurkokat](../images/connect_infill_polygons_enabled.png)

Ennek a funkciónak az a célja, hogy megakadályozza a mozgást. Az utolsó sor egyetlen hurok lesz a kitöltés minden csatlakoztatott részéhez, így nem lesz semmilyen utazási mozgás. Ez megkönnyíti a rugalmas szálak használatát, mivel azokat nehezebb visszahúzni, és akkor működnek a legjobban, ha folyamatosan át tudnak folyni a fúvókán.

Ezen hurkok összekapcsolása a kitöltést is erősebbé teheti azáltal, hogy javítja a hurkok közötti belső kapcsolatot. Ha azonban a sokszögek össze vannak kötve, a nyomtatófejnek gyakran 180 fokos fordulatot kell tennie közvetlenül az illesztés előtt. Ezek a fordulatok néha megakadályozzák a kötés teljes összekapcsolását. Ez bizonyos esetekben gyengítheti a kitöltést is. Minden attól függ, hogy a hurkok hogyan illeszkednek át a modell alakján.
