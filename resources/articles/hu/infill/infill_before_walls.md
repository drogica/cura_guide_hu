# Kitöltés a falak előtt

Ez befolyásolja a nyomtatási sorrendet. Ha ez a beállítás engedélyezve van, akkor az alkatrész kitöltése még azelőtt kinyomtatásra kerül, mielőtt az alkatrész falai az adott rétegen megjelennének.

<!--screenshot {
"image_path": "infill_before_walls_disabled.gif",
"models": [
    {
        "script": "cube.scad",
        "transformation": ["scale(0.25)"]
    }
],
"camera_position": [0, 0, 100],
"settings": {
    "top_layers": 0,
    "infill_before_walls": false
},
"layer": 162,
"line": [0, 1, 2, 3, 4, 7, 8, 9, 10, 12, 15, 18, 21, 24, 27],
"colours": 32,
"delay": 250
}-->

<!--screenshot {
"image_path": "infill_before_walls_enabled.gif",
"models": [
    {
        "script": "cube.scad",
        "transformation": ["scale(0.25)"]
    }
],
"camera_position": [0, 0, 100],
"settings": {
    "top_layers": 0,
    "infill_before_walls": true
},
"layer": 162,
"line": [0, 1, 4, 7, 10, 13, 16, 20, 21, 22, 23, 26, 27, 28, 29],
"colours": 32,
"delay": 250
}-->

![A beállítás le van tiltva, ezért a rendszer először a falakat nyomtatja ki](../images/infill_before_walls_disabled.gif)![A beállítás engedélyezve van, tehát először a kitöltés kerül kinyomtatásra](../images/infill_before_walls_enabled.gif)

Ez a beállítás kompromisszum a pontosság és az erősség között:

- Ha a falakat a kitöltés előtt nyomtatják, akkor a falakon nem lehet semmi, amihez rögzíthető, ami jobban megereszkedik. A falak azonban előbb megszilárdulnak, és nem tolják el őket a kitöltéstől, ami megakadályozza, hogy a kitöltés átsüljön a falakon.
- Ha a betétet a falak elé nyomtatják, a falak eltolódnak ott, ahol a kitöltés a falakhoz van rögzítve, ami kevésbé pontosítja a falakat, és a kitöltés átvilágíthat a felületen, így kívülről látható mintázat jön létre. A kitöltés azonban jobban tartja a falakat nyomtatás közben.
