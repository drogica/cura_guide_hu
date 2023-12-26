# Kitöltési sűrűség

Ez a beállítás konfigurálja a nyomat belsejében lévő térfogat sűrűségét, ami fontos tényező a végső nyomat erőssége és a felső felület minősége szempontjából. Minél nagyobb a kitöltési sűrűség, annál közelebb kerülnek egymáshoz a kitöltési vonalak. Akár 100%-os sűrűség fölé is mehet, de ez túlextrudálást eredményez.

<!--screenshot {
"image_path": "infill_pattern_grid.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "grid"
},
"colours": 64
}-->

<!--screenshot {
"image_path": "infill_sparse_density_low.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_sparse_density": 10
},
"colours": 64
}-->

![20% sűrűségű](../images/infill_pattern_grid.png)![10% sűrűségű](../images/infill_sparse_density_low.png)

A különböző sűrűségek jobban működnek a különböző kitöltési mintákkal. A sok sarokkal és sok keresztezéssel rendelkező kitöltési minták nem működnek jól nagy kitöltési sűrűség esetén. A sarkok problémát jelentenek, mivel az izzószál hajlamos a sarokkal együtt húzódni, és légzsebek keletkeznek a sarok külső részén, ahol az anyagot le kellett volna rakni. A kereszteződések még nagyobb problémát jelentenek, mert amikor az egyik vonal keresztezi a másikat, annak áramlása megszakad, ami alulextrudálást okoz közvetlenül a keresztezés után.

A kitöltési sűrűség növelése (a vonaltávolság csökkentésével) nagy hatással van a nyomtatásra, nevezetesen:

- A nyomat erősebb lesz.
- A felső felület jobban alátámasztva lesz, így simább és vízzáróbb lesz.
- Csökkentett párnázás, mert a hőzsebek kisebbek lesznek.
- A nyomat több anyagot igényel, és ennek eredményeként nehezebb lesz.
- A nyomtatás tovább tart.
