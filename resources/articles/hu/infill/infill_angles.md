# Töltse ki a soros irányokat

A kitöltő vonalakat általában 45 fokos szögben irányítják, amennyire csak lehetséges. Ebben a szögben az X és az Y motor együtt dolgozik a nyomtatófej maximális gyorsítása érdekében, ha a közös derékszögű portálmechanizmussal rendelkező nyomtatót használjuk.

Ezzel a beállítással beállíthatja ezt a szöget. Speciálisan növelheti az adott modell szilárdságát, vagy nagyobb gyorsulást érhet el az adott portálrendszerhez (például delta nyomtatókhoz).

<!--screenshot {
"image_path": "infill_pattern_lines.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "lines"
},
"colours": 32
}-->

<!--screenshot {
"image_path": "infill_angles_0_30.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "lines",
    "infill_angles": [0, 30]
},
"colours": 32
}-->

![Vonalkitöltés 45 és 135 fokos alapértelmezett szögekkel](../images/infill_pattern_lines.png)![Vonalkitöltés testreszabott 0 és 30 fokos szögekkel](../images/infill_angles_0_30.png)

A beállítás értékének a szögek vesszővel elválasztott listájának kell lennie, körülötte zárójelekkel. A 0 fokos szög az Y tengellyel párhuzamos egyenest eredményez. A szögek listája felváltva jelenik meg a rétegeken.

- A végső nyomat a kitöltési vonalak irányában lesz a legerősebb. Ha arra van szüksége, hogy a nyomat vízszintes irányban meghatározott erőt hordozzon, hasznos a kitöltési vonalakat az adott irányba irányítani.
- Hagyja a beállítást üres listán az alapértelmezett használatához.
- Az alapértelmezett érték a kitöltési mintától függ:
    - Kereszt és kereszt 3D kitöltési minták esetén az alapértelmezett érték [22]. Ez a lehető legtöbb vonalat az átlókhoz közelíti.
    - A Vonalak és Cikkcakk kitöltési minták esetében az alapértelmezett érték [45 135]. Ez azt eredményezi, hogy a tájolás rétegenként váltakozik a két átló között.
    - Az összes többi minta alapértelmezett értéke [45]. Ez a lehető legtöbb vonalat az átlókhoz közelíti.
