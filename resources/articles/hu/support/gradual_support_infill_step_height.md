# Fokozatos támogatási kitöltés lépcsőmagassága

Fokozatos alátámasztás esetén a támasz sűrűsége több lépésben felülről lefelé időszakosan csökken. Minden lépésnél a támaszsűrűség felére csökken. Ez a beállítás jelzi ezeknek a lépcsőknek a magasságát, két olyan hely közötti távolságot, ahol az alátámasztás sűrűsége felére csökken.

<!--screenshot {
"image_path": "gradual_support_infill_step_height_1mm.png",
"models": [
    {
        "script": "stair.scad",
        "transformation": ["rotateY(-90)", "scaleZ(0.5)"]
    }
],
"camera_position": [49, 91, -38],
"settings": {
    "support_enable": true,
    "support_pattern": "grid",
    "support_wall_count": 0,
    "support_infill_rate": 50,
    "gradual_support_infill_steps": 3,
    "gradual_support_infill_step_height": 1
},
"colours": 64
}-->

<!--screenshot {
"image_path": "gradual_support_infill_step_height_3mm.png",
"models": [
    {
        "script": "stair.scad",
        "transformation": ["rotateY(-90)", "scaleZ(0.5)"]
    }
],
"camera_position": [49, 91, -38],
"settings": {
    "support_enable": true,
    "support_pattern": "grid",
    "support_wall_count": 0,
    "support_infill_rate": 50,
    "gradual_support_infill_steps": 3,
    "gradual_support_infill_step_height": 3
},
"colours": 64
}-->

![1 mm lépcsőmagasság](../images/gradual_support_infill_step_height_1mm.png)![3 mm lépcsőmagasság](../images/gradual_support_infill_step_height_3mm.png)

A fokozatos támogatás természeténél fogva felfüggeszti a támogatás egy részét a levegőben. Ez azonban általában automatikusan megjavítja magát. Az első támasztóréteg a levegőben lóg, és csak a támasz oldalaihoz csatlakozik megfelelően. A tetején lévő rétegek a végein kicsit ráfekszenek az előző rétegre, de a közepén megereszkednek. Ez fokozatosan javul, rétegről rétegre. Ha a fokozatos alátámasztási lépcsőmagasság elég nagy, a támaszték megfelelően szilárd lesz a következő sűrűségi lépésre.

Csökkentse a fokozatos alátámasztási lépés magasságát, hogy gyorsan leereszkedjen az alacsony alátámasztási sűrűségre. Ezzel nyomtatási időt és anyagfelhasználást takaríthatunk meg. Növelje a fokozatos alátámasztási lépés magasságát, ha a támasznak nem lesz elég helye a megjavításhoz, mire a támaszsűrűség következő lépése megtörténik. A beállítás értékének növelése megbízhatóbbá teszi a nyomtatást.
