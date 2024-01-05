# A támogatás fokozatos kitöltési lépései

A fokozatos alátámasztás csökkenti a felhasznált hordozóanyag mennyiségét azáltal, hogy csökkenti a hordozósűrűséget az alsó rétegekben. Ezzel nyomtatási időt és anyagot takaríthat meg, miközben nem csökkenti jelentősen a túlnyúlás minőségét. A támogatás elsődleges célja a túlnyúló területek támogatása. Ez a funkció a támogatást csak erre a célra összpontosítja.

Ez a beállítás azt jelzi, hogy hány lépésben csökken az alátámasztás sűrűsége. A támasz sűrűsége minden lépésnél felére csökken. Például 20%-os sűrűségtől és két fokozatos alátámasztástól kezdve az alsó részek támaszsűrűsége 10%, illetve 5% lesz.

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

![A támaszték 3 lépésben kisebb sűrűségűre csökken](../images/gradual_support_infill_step_height_1mm.png)

A lépések számának növelése miatt a sűrűség egyre jobban felére csökken, ami alacsonyabb sűrűségű támogatást eredményez. Ez sok anyagot és nyomtatási időt takarít meg, de gyengébb lesz a támogatás.

A támasz egy része a levegőben fog lebegni. A gyakorlatban azonban a legtöbb támasztómintánál ez gyorsan megjavul, mivel a rétegek még a legyengült alsó rétegeken is megfelelően fel tudnak épülni. A [fokozatos alátámasztási lépés magasságának](gradual_support_infill_step_height.md) célja, hogy elegendő időt hagyjon a rétegeknek, hogy megjavítsák magukat, mielőtt a következő fokozatos alátámasztási lépést felhalmozzák.

Ezt a beállítást a legjobb kombinálni legalább egy [támasztófalvonallal](support_wall_count.md) . Ez ad a támasztóvonalaknak valamit, amin kapaszkodni lehet, nem pedig a levegőben.
