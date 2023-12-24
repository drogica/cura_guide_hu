# Kezdeti rétegmagasság

Ez a beállítás határozza meg a nyomat első rétegének vastagságát. A kezdeti réteget általában vastagabbra nyomtatják, mint a többit, hogy erősebb tapadást hozzon létre az építőlemezzel. Ezzel a beállítással a kezdeti réteg vastagsága növelhető anélkül, hogy csökkentené a nyomat többi részének felbontását.

<!--screenshot {
"image_path": "layer_height_0.png",
"models": [
    {
        "script": "rolling_blind_spacer.scad",
        "transformation": ["scale(0.5)"]
    }
],
"camera_position": [39, 28, 5],
"settings": {"layer_height_0": 0.3},
"colours": 32
}-->

![A kezdeti réteg vastagabb, mint a többi réteg](../images/layer_height_0.png)

A kezdeti réteg vastagságának növelésével a fúvóka több anyagot extrudál ki ugyanazon a távolságon. Ez extra erőt igényel, mivel az anyag szétterül az oldalakon, és kitölti a teljes vonalszélességet. Ez az extra erő hatására az anyag jobban tapad az építőlemezhez. Ezenkívül a vastagabb réteg felfogja a felület síkságának egyenetlenségeit. Ha az építőlemez enyhén meg van hajlítva, a változékonyságot elnyeli az első réteg vastagsága, ellenkező esetben a fúvóka lekaparhatja azt a második rétegben.

Ha túl vastag a kezdeti réteg, akkor az első réteg jobban megereszkedik, ami az elefánt lábait okozza. Az [Initial Layer Horizontal Expansion (Kezdő réteg vízszintes kiterjesztése)](../shell/xy_offset_layer_0.md) beállítás ezt megakadályozhatja, ha kis negatív értéket ad neki.
