# Villámfeltöltés aszalt szilva szög

A Lightning kitöltési minta faszerű szerkezetet hoz létre a nyomat belsejében, amely kicsiben kezdődik, de elágazik, hogy elérje a nyomat tetejének minden részét, amelyet belülről meg kell támasztani. Ez a beállítás azt jelzi, hogy a fa ágai milyen messzire nyúlhatnak túl a végpontokon.

<!--screenshot {
"image_path": "lightning_infill_prune_angle_40.png",
"models": [{"script": "half_sphere.scad"}],
"camera_position": [112, 15, 9],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 40,
    "lightning_infill_prune_angle": 40
},
"colours": 32
}-->

<!--screenshot {
"image_path": "lightning_infill_prune_angle_70.png",
"models": [{"script": "half_sphere.scad"}],
"camera_position": [112, 15, 9],
"settings": {
    "infill_pattern": "lightning",
    "wall_line_count": 0,
    "top_layers": 0,
    "lightning_infill_support_angle": 40,
    "lightning_infill_prune_angle": 70
},
"colours": 32
}-->

![40°-nál a Lightning kitöltés elég stabil](../images/lightning_infill_prune_angle_40.png)![70°-nál az ágak meglehetősen meredeken túlnyúlnak](../images/lightning_infill_prune_angle_70.png)

Az aszalt szilva szögének növelése azt jelenti, hogy a kitöltés kisebbre tud indulni alul, miközben továbbra is eléri az egész felső felületet. Sok esetben már nem is kell alulról indulnia, hanem egyszerűen az oldalakon lóghat. A szög növelésének kiemelkedő hatásai a következők:

- Csökkentett nyomtatási idő és anyagfelhasználás.
- Simább falak, mert nem lesz annyi kitöltés, ami belülről érinti a falakat.
- Kissé csökkentett erő.
- Nagyobb a nyomtatási hiba esélye. Ha a túlnyúlás túl meredek, akkor minden vonal végén jelentős túlnyúlás lesz, ami megereszkedik és kilazulhat.

A gyakorlatban az aszalt szilva szöge nagyobb lehet, mint a normál túlnyúlási szögek vagy a többi Lightning-kitöltés túlnyúlási szöge. Mivel a vonalak jól meg vannak támasztva az alábbi rétegen, a nagyobb túlnyúlás nem jelent problémát.
