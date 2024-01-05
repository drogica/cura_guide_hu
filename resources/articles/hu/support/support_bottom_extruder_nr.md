# Támogassa a padlóextrudert

Ha a nyomtatója több extruderrel rendelkezik, akkor a tartó alsó oldalára, ahol a támasz a modellen nyugszik, más extruderrel is nyomtatható, mint a tartó tetejére, ahol a modell a tartón nyugszik. Ezzel a beállítással kiválaszthatja, hogy melyik extrudert használja a tartópadlóhoz.

<!--screenshot {
"image_path": "support_bottom_extruder_nr.png",
"models": [
    {
        "script": "question_stick_clip.scad",
        "transformation": ["rotateY(90)"],
        "object_settings": {"extruder_nr": 1}
    }
],
"camera_position": [134, 134, 113],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_use_towers": false,
    "support_extruder_nr": 3,
    "support_bottom_extruder_nr": 2
},
"colour_scheme": "material_colour",
"colours": 64
}-->

![A tartópadló pirossal, a tartótető pedig fehérrel van nyomtatva](../images/support_bottom_extruder_nr.png)

Egyes anyagok jobb kinyúlási tulajdonságokat biztosítanak, mint más anyagok, ha alátámasztásra használják. Például előfordulhat, hogy a felülethez közelebbről nyomtathatnak, mert kémiailag nem kötődnek a felülethez, vagy vízben oldódnak. Az ilyen anyagok azonban gyakran drágák, és hosszabb ideig tart a nyomtatás. Ezzel a beállítással más extruderrel nyomtathatja ki a támasztó alját. Ez megtakaríthatja a drága vagy lassan nyomtatható anyagok egy részét.

A túlnyúlások minősége szempontjából a tartópadló kevésbé fontos, mint a tartótető. Ha egy drága anyagot takarékosan kell használni, a tartópadló jó választás az olcsóbb anyaggal történő nyomtatáshoz.
