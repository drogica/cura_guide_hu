# Támogatja az interfész vízszintes bővítését

Ez a beállítás azt eredményezi, hogy a támogatási felület minden irányban vízszintesen kibővül a támasz többi részébe.

<!--screenshot {
"image_path": "support_interface_offset.png",
"models": [{"script": "f.scad"}],
"camera_position": [45, 45, 133],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_offset": 2,
    "support_interface_offset": 1
},
"colours": 64
}-->

![A támogatási felület kibővül a támogatásba](../images/support_interface_offset.png)

Ennek a mechanizmusnak két felhasználási esete van.

- Ha a támasztófelület közvetlenül a támasztandó túlnyúlás szélén ér véget, az építőanyag megereszkedhet a szélén. Ha a kezelőfelületet tovább bővítjük, ez megelőzhető.
- Egyes anyagok, amelyeket általában a hordozónyomtatáshoz használnak, rosszul extrudálnak alacsony áramlási sebesség mellett, vagy időre van szükségük az induláshoz. A támogatási felület kis területei nem illenek jól ezekhez az anyagokhoz. Ez a beállítás szó szerint nagyobbá teheti a területeket, így több hely marad ezen anyagok extrudálására.

Technikai korlátok miatt a támogatási felület magán a támogatáson túl nem bővíthető.
