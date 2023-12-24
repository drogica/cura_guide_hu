# Kezdeti réteg vonalszélesség

Ez bizonyos arányban szélesebbé vagy vékonyabbá teszi a kezdeti réteg vonalait.

<!--screenshot {
"image_path": "initial_layer_line_width_factor.png",
"models": [{"script": "hex_foot.scad"}],
"camera_position": [0, 92, 122],
"settings": {
    "adhesion_type": "brim",
    "initial_layer_line_width_factor": 200
},
"colours": 32
}-->

![A kezdeti réteg vonalai kétszer olyan szélesek, mint a többi](../images/initial_layer_line_width_factor.png)

Ennek a beállításnak az a célja, hogy javítsa az építőlemezhez való tapadást. A szélesebb vonalak nyomtatásához a fúvókának több anyagot kell extrudálnia, és az anyagnak szélesebbre kell áramolnia kifelé. Ez azt eredményezi, hogy a fúvóka erősebben nyomja az anyagot az építőlemezre, ami növeli a tapadást az izzószál és az építőlemez között.

- Nemcsak szélesebbek vagy vékonyabbak lesznek a vonalak, de távolabb vagy közelebb kerülnek egymáshoz ugyanazon tényező miatt, így nem okozna túl- vagy alulextrudálást.
- Ez a beállítás minden vonalszélességre hatással van; bőr, falak, tapadás, támaszték, az elsődleges torony stb. Ugyanilyen arányban lesznek szélesebbek vagy vékonyabbak.
