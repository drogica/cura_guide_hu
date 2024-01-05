# First Layer Support Extruder

Ha a nyomtatója több extruderrel rendelkezik, akkor az építőlemezen nyugvó tartóréteg más extruderrel is nyomtatható, mint a tartó többi része. Ezzel a beállítással kiválaszthatja, hogy melyik extrudert használja a kezdeti támasztóréteghez.

<!--screenshot {
"image_path": "support_extruder_nr_layer_0.png",
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
    "support_extruder_nr_layer_0": 2
},
"colour_scheme": "material_colour",
"colours": 64
}-->

![A tartó kezdeti rétege piros, a többi fehér színnel van nyomtatva](../images/support_extruder_nr_layer_0.png)

Egyes anyagok jobban megfelelnek a nyomtatás támogatására, mint mások. Ezek gyakran inert anyagok, amelyek nem tapadnak jól más anyagokhoz, így könnyebben eltávolíthatók. Ez a tulajdonság azonban nem kívánatos az építőlemezhez való ragaszkodáshoz. Ezután az építőlemezhez jobban tapadó anyag használható az első réteghez, amelyhez a normál hordozóanyag jobban tapad, mint az üveghez vagy az alumíniumhoz.
