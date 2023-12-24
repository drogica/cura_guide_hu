# Kitöltés Y eltolás

Általában a kitöltési minták a 3D modell közepén helyezkednek el. Ez a beállítás az [Infill X Offset-tel](infill_offset_x.md) együtt lehetővé teszi a minta középpontjának eltolását. Ez a beállítás a középpont Y koordinátáját állítja be.

<!--screenshot {
"image_path": "infill_offset_xy_0.png",
"models": [
    {
        "script": "hexagonal_prism.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [0, 0, 90],
"settings": {
    "top_layers": 0,
    "infill_pattern": "triangles",
    "infill_offset_x": 0
},
"colours": 64
}-->

<!--screenshot {
"image_path": "infill_offset_y_2.png",
"models": [
    {
        "script": "hexagonal_prism.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [0, 0, 90],
"settings": {
    "top_layers": 0,
    "infill_pattern": "triangles",
    "infill_offset_y": 2
},
"colours": 64
}-->

![A kitöltés középre van állítva](../images/infill_offset_xy_0.png)![2 mm-rel feljebb tolva](../images/infill_offset_y_2.png)

Ha alacsony kitöltési sűrűséggel nyomtat, ezzel nagyon pontosan pozícionálhatja a kitöltést úgy, hogy az egyes kitöltési vonalak oda kerüljenek, ahol a legnagyobb szükség van az erőre.
