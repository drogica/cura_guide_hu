# Támassza meg a tetővonal szélességét

A tartótető vonalainak szélessége külön konfigurálható a többi támasztóvonal szélességétől.

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

![A tartótető vonalai szélesebbek, mint a többi támasztóvonal](../images/support_roof_line_width.png)

A tartótető kissé vékonyabb vonalakkal történő nyomtatása gyakran előnyös az általa alátámasztott túlnyúló felület minősége szempontjából, pusztán azáltal, hogy a támasztófelület felett simább felső felület van. Ez azonban nem feltétlenül növeli a tapadást a tartófelület és a modell között, így a támaszt nem feltétlenül lesz nehezebb eltávolítani.

A tetővonalak túl vékony nyomtatása azonban egyenetlen extrudálást okoz, ami csökkenti a tető alátámasztó hatását, ami rosszabb kinyúlási minőséget okoz. Ezenkívül jelentős változást idézhet elő a fúvókán keresztüli áramlási sebességben, túlextrudálást okozva, amikor elkezdi nyomtatni a tartótetőt, és alulextrudálást okozva, ha bármit nyomtat a tartótető után.
