# Támogatás interfész vonalszélesség

A támasztóvonalak szélessége külön konfigurálható a többi támasztóvonal szélességétől.

<!--screenshot {
"image_path": "support_roof_line_width.png",
"models": [
    {
        "script": "trash_bin_lid.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [-47, 79, 110],
"settings": {
    "support_enable": true,
    "support_roof_enable": true,
    "support_roof_line_width": 0.8
},
"layer": 192,
"colours": 64
}-->

![A támasztó interfész vonalai szélesebbek, mint a többi támasztóvonal](../images/support_roof_line_width.png)

A támasztófelület valamivel vékonyabb vonalakkal történő nyomtatása gyakran előnyös az általa alátámasztott túlnyúló felület minősége szempontjából, pusztán azáltal, hogy a támasztófelület felett simább felső felület van. Ez azonban nem feltétlenül növeli a tapadást a tartófelület és a modell között, így a támaszt nem feltétlenül lesz nehezebb eltávolítani.

Hasonlóképpen, a támasztópadló egyenletesebben fog tapadni, csökkentve a hegesedést ott, ahol a támasz a modellen feküdt, anélkül, hogy gyengülne.

Az interfész vonalainak túl vékony kinyomtatása azonban egyenetlen extrudálást okoz, ami csökkenti az interfész támasztó hatását, ami rosszabb túlnyúlási minőséget és kevésbé stabil alátámasztást okoz. Ezenkívül nagy változást idézhet elő a fúvókán keresztüli áramlási sebességben, túlextrudálást okozva, amikor elkezdi nyomtatni a támogatási felületet, és alulextrudálást okozva, ha bármit nyomtat a támasztófelület után.
