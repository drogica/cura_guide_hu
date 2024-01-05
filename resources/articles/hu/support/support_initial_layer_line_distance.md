# Kezdeti réteg támogatási vonal távolsága

Annak a mintának a sűrűsége, amellyel az első tartóréteget nyomtatják, a támasztóanyag többi részének sűrűségétől külön állítható. Ez a beállítás konfigurálja a távolságot két szomszédos vonal között, ahol a támasz az építőlemezen fekszik.

<!--screenshot {
"image_path": "support_initial_layer_line_distance.png",
"models": [{"script": "umbrella_square_rounded.scad"}],
"camera_position": [0, 64, 125],
"settings": {
    "support_enable": true,
    "support_initial_layer_line_distance": 1.333
},
"layer": 160,
"colours": 64
}-->

![Az első réteg mintája kétszer olyan sűrű, mint a tartó többi részének](../images/support_initial_layer_line_distance.png)

Ez a beállítás hasznos a tartó és az építőlemez közötti tapadás javítására. Az első rétegben a tartómintázat sűrűbbé tétele növeli a tartó és az építőlemez közötti érintkezési felületet, így jobban tapad. A következő rétegeket ezután olyan anyagra lehet helyezni, amelyhez jobban tapadnak.

Mivel ez a beállítás csak az első réteget érinti, így a támaszték szilárdságát, sem az idő- és anyagköltséget nem befolyásolja jelentősen. Nem befolyásolja a túlnyúlások minőségét sem. A túlnyúlások közelében lévő alátámasztás sűrűségének beállításához tekintse meg a [Tartótető vonal távolsága](support_roof_line_distance.md) beállítást.

Célszerű ezt a beállítást a támaszték fő része vonaltávolságának többszörösére tenni. Így a támasztóvonalak illeszkednek az első réteg vonalaihoz, lehetővé téve számukra, hogy az első rétegen pihenjenek, ahelyett, hogy a levegőben lebegnének.
