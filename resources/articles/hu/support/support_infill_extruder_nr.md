# Támogatja az Infill Extrudert

Ha a nyomtatója több extruderrel rendelkezik, a támaszték fő része más extruderrel is nyomtatható, mint a támasztó interfész. Ez a beállítás lehetővé teszi, hogy kiválassza, hogy melyik extrudert használjuk a tartóelemhez.

<!--screenshot {
"image_path": "support_infill_extruder_nr.png",
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
    "support_infill_extruder_nr": 2
},
"colour_scheme": "material_colour",
"colours": 64
}-->

![A tartó teste piros, a felület fehér színnel van nyomtatva](../images/support_infill_extruder_nr.png)

Egyes anyagok jobban megfelelnek a nyomtatás támogatására, mint mások, de ezek az anyagok drágábbak vagy lassabban nyomtathatók. Ha csak a felületet nyomtatja ki a drága anyaggal, de a test nagy részét olcsóbb anyaggal, akkor sok időt és pénzt takaríthat meg. A felület továbbra is a drága anyaggal lesz nyomtatva, így a modellt érintő rész jól fog kinézni, vagy könnyebben leszakadhat, de a támasz nagy része olcsóbb anyagokkal lesz nyomtatva.

Ha oldható anyagokat használ a tartófelület nyomtatásához, de oldhatatlan anyagokat a tartótest nyomtatásához, ne feledje, hogy előfordulhat, hogy a testet nem lehet eltávolítani az üregekből, ha fizikailag lehetetlen a tartótestet áthelyezni egy kis nyílás. Ahol az oldható anyag általában az oldatban lévő üregen keresztül tud kifolyni, előfordulhat, hogy az oldhatatlan anyagok nem tudnak átmenni.
