# Támogatás Interface Extruder

Ha a nyomtatója több extruderrel rendelkezik, akkor az interfészrétegek, ahol a tartó érintkezik a modellel, más extruderrel is nyomtathatók, mint a tartó teste. Ezzel a beállítással kiválaszthatja, hogy melyik extrudert használja a támogatási felülethez.

<!--screenshot {
"image_path": "support_interface_extruder_nr.png",
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
    "support_interface_extruder_nr": 2
},
"colour_scheme": "material_colour",
"colours": 64
}-->

![A támogatási felület piros színű, a törzs pedig fehér](../images/support_interface_extruder_nr.png)

Egyes anyagok jobban megfelelnek a nyomtatás támogatására, mint mások. Előfordulhat például, hogy kémiailag nem tapadnak az építőanyaghoz, és könnyebben leszakadhatnak, vagy feloldódhatnak vízben vagy alkoholban. Az ilyen anyagok azonban gyakran drágák, és hosszabb ideig tart a nyomtatás. Ez a beállítás lehetővé teszi, hogy a támasztófelületet a főtesttől eltérő extruderrel nyomtatja ki, így a támaszték nagy része továbbra is gyorsan és/vagy olcsóbb anyagokkal nyomtat, de a speciális hordozóanyag előnyei továbbra is érvényesek.

Ha oldható anyagokat használ a tartófelület nyomtatásához, de oldhatatlan anyagokat a tartótest nyomtatásához, ne feledje, hogy előfordulhat, hogy a testet nem lehet eltávolítani az üregekből, ha fizikailag lehetetlen a tartótestet áthelyezni egy kis nyílás. Ahol az oldható anyag általában az oldatban lévő üregen keresztül tud kifolyni, előfordulhat, hogy az oldhatatlan anyagok nem tudnak átmenni.
