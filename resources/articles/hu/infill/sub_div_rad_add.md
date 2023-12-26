# Cubic Subdivision Shell

Ezzel a beállítással a Cubic Subdivision kitöltési minta a nyomat szilárdságának javítása érdekében egy kicsit befelé kezdi csökkenteni a kitöltést.

<!--screenshot {
"image_path": "sub_div_rad_add_small.png",
"models": [
    {
        "script": "cylinder.scad",
        "transformation": ["scale(3)"]
    }
],
"camera_position": [0, 0, 275],
"settings": {
    "infill_sparse_density": 70,
    "infill_pattern": "cubicsubdiv",
    "sub_div_rad_add": 0
},
"layer": 500,
"colours": 32
}-->

<!--screenshot {
"image_path": "sub_div_rad_add_large.png",
"models": [
    {
        "script": "cylinder.scad",
        "transformation": ["scale(3)"]
    }
],
"camera_position": [0, 0, 275],
"settings": {
    "infill_sparse_density": 70,
    "infill_pattern": "cubicsubdiv",
    "sub_div_rad_add": 5
},
"layer": 500,
"colours": 32
}-->

![Köbös felosztás további héj nélkül](../images/sub_div_rad_add_small.png)![5 mm-es kiegészítő héj](../images/sub_div_rad_add_large.png)

A kockafelosztás úgy működik, hogy eltávolítja a határokat nyolc szomszédos kocka között, ha egyik kocka sem érinti a kitöltési térfogat határát. Ez a beállítás beljebb helyezi a szegélyt, megakadályozva, hogy a kockák közötti szegélyeket eltávolítsák.

Ez gyakorlatilag azt eredményezi, hogy a köbös felosztási minta gyakrabban rajzolja meg a maximális sűrűséget. Ez növeli a tárgy szilárdságát, de növeli a nyomtatáshoz szükséges időt és anyagot is. Extrém esetben ennek a beállításnak a kellő növelése azt eredményezi, hogy a kockafelosztás mintája megegyezik az egyszerű kockamintával.

Ezt negatív számra is beállíthatja. Ez azt eredményezi, hogy a kockák közötti szegélyeket gyakrabban távolítják el, ami hatékonyan csökkenti a szélek körüli kitöltés mennyiségét.
