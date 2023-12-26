# Csatlakoztassa a kitöltési vonalakat

Ez a beállítás a kitöltési minta végpontjait köti össze, ahol a kitöltés találkozik a belső fallal vagy burkolattal, egy vonal segítségével, amely a kitöltési terület szélét követi.

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
"image_path": "zig_zaggify_infill_enabled.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "grid",
    "zig_zaggify_infill": true
},
"colours": 64
}-->

![Nincsenek csatlakoztatott betöltő vezetékek](../images/infill_pattern_grid.png)![Csatlakoztatott kitöltő vezetékek](../images/zig_zaggify_infill_enabled.png)

Ez a teljes kitöltési mintát egyetlen vagy nagyon kevés sorrá alakítja. Nem mindig lehetséges egyetlen sorrá konvertálni. Ennek a sornak a kezdőpontja tetszőleges, ezért előfordulhat, hogy nem minden rétegnél azonos, különösen, ha a kitöltés alakja rétegenként eltérő.

A kitöltés csatlakoztatásának van néhány előnye, de vannak hátrányai is:

- A végére erősebb lesz a részed, hiszen gyakorlatilag fele kontúr extra van.
- A kitöltés jobban tapad a falakhoz a megnövekedett felület miatt, ami az alkatrészt is erősebbé teszi.
- Az áramlási sebesség állandóbb lesz, így nagyobb sebességgel nyomtathatja ki a kitöltést áramlási problémák nélkül. Ez különösen fontos olyan anyagok esetében, amelyeket nehéz megfelelően extrudálni.
- A kitöltés nyomtatása során lényegesen kevesebb visszahúzás történik majd, ami megakadályozza az anyag csiszolását.
- A [Kitöltési átfedés](infill_overlap.md) beállítás hatása felerősödik, mivel a kitöltő vonalak nagyobb része átfedi a falakat.
- A kitöltés kinyomtatásához több anyagra lesz szükség.
- Általában több időt vesz igénybe a kitöltés kinyomtatása, mivel az utazási mozgások általában gyorsabbak, mint a kitöltési vonalak nyomtatása.
- A kitöltés általában jobban átvilágít a falakon, mivel a falak nagyobb részére tolódik be.
