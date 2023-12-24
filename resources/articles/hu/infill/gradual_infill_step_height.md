# Fokozatos kitöltés lépcsőmagassága

Fokozatos kitöltés esetén a kitöltés sűrűsége több lépésben felülről lefelé csökken. Minden lépésnél a feltöltési sűrűség felére csökken. Ez a beállítás jelzi ezeknek a lépcsőknek a magasságát, két olyan hely közötti távolságot, ahol a kitöltés felére csökken.

<!--screenshot {
"image_path": "gradual_infill_step_height_small.png",
"models": [{"script": "curved_top.scad"}],
"camera_position": [0, 137, -62],
"settings": {
    "wall_line_count": 0,
    "bottom_layers": 0,
    "gradual_infill_steps": 3,
    "gradual_infill_step_height": 1.5
},
"colours": 16
}-->

<!--screenshot {
"image_path": "gradual_infill_step_height_large.png",
"models": [{"script": "curved_top.scad"}],
"camera_position": [0, 137, -62],
"settings": {
    "wall_line_count": 0,
    "bottom_layers": 0,
    "gradual_infill_steps": 3,
    "gradual_infill_step_height": 5
},
"colours": 16
}-->

![Fokozatos betöltési lépés magassága 1,5 mm](../images/gradual_infill_step_height_small.png)![Fokozatos betöltési lépés magassága 5 mm](../images/gradual_infill_step_height_large.png)

A fokozatos feltöltés természeténél fogva felfüggeszti a feltöltődés egy részét a levegőben. Ez azonban általában automatikusan megjavítja magát. Az első betétréteg a levegőben lóg, és csak a nyomat oldalaihoz tapad megfelelően. A rárakott rétegek a végein kicsit rátámaszkodhatnak az előző rétegre, de a közepén még megereszkednek. Ez fokozatosan javul, rétegről rétegre.

- Csökkentse a fokozatos feltöltési lépés méretét, hogy gyorsan csökkenjen az alacsony feltöltési sűrűségre. Ezzel nyomtatási időt és anyagfelhasználást takaríthatunk meg.
- Növelje a fokozatos kitöltés lépésének méretét, ha a kitöltésnek nem lesz elég helye ahhoz, hogy megjavítsa magát, mire a kitöltés sűrűségének következő lépése megtörténik. A beállítás értékének növelése megbízhatóbbá teszi a nyomtatást.
