# Fokozatos kitöltési lépések

A fokozatos feltöltés csökkenti a felhasznált kitöltés mennyiségét azáltal, hogy csökkenti az alsó rétegek kitöltési sűrűségét. Ezzel nyomtatási időt és anyagot takaríthat meg, miközben nem csökkenti jelentősen a felület minőségét. A vizuális minőség érdekében történő nyomtatáskor a kitöltés elsődleges célja a felső felület megtámasztása. Ez a funkció csak erre a célra fókuszálja a kitöltést.

Ez a beállítás azt jelzi, hogy hány lépésben csökken a kitöltés sűrűsége. Minden lépésnél a feltöltési sűrűség felére csökken. Például 20%-os kitöltési százaléktól és két fokozatos kitöltési lépéstől kezdve az alsó részek feltöltési sűrűsége 10%, illetve 5% lesz.

<!--screenshot {
"image_path": "gradual_infill_disabled.png",
"models": [{"script": "curved_top.scad"}],
"camera_position": [0, 137, -62],
"settings": {
    "wall_line_count": 0,
    "bottom_layers": 0,
    "gradual_infill_steps": 0
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

![Normál kitöltés](../images/gradual_infill_disabled.png)![3 fokozatos kitöltési lépés](../images/gradual_infill_step_height_large.png)

**A "Fokozatos kitöltés" pipa az ajánlott módban ezt a beállítást 5 lépésre állítja, és 90%-ra növeli a kitöltés sűrűségét. Ez nagyon magas sűrűséget okoz a nyomat tetején (90%) és nagyon alacsony sűrűséget a nyomat alján (2,8%).**
