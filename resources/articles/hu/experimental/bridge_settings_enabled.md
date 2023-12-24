# Engedélyezze a Bridge beállításokat

Ha a modellnek van olyan túlnyúlása, amely mindkét oldalon támogatott, a Cura észleli ezt, és módosítja a túlnyúló bőrfelületet a jobb nyomtatás érdekében. Ha ez a beállítás engedélyezve van, akkor ezeknek az áthidaló területeknek az észlelését és az ebből eredő viselkedést úgy hangolhatja, hogy az jobban áthidaljon.

<!--screenshot {
"image_path": "bridge_settings_enabled_default.png",
"models": [
    {
        "script": "rack_straight.scad",
        "scad_params": ["length=40"]
    }
],
"camera_position": [0, 74, -137],
"colours": 32
}-->

<!--screenshot {
"image_path": "bridge_settings_enabled_enabled.png",
"models": [
    {
        "script": "stairwell.scad",
        "scad_params": ["steps=4", "width=10", "height=20"]
    }
],
"layer": 275,
"settings": {
    "bridge_settings_enabled": true
},
"camera_position": [-12, 28, 63],
"colours": 64
}-->

![Amikor a rendszer egy hidat észlel, a bőrvonalak a lehető legjobban áthidalják a rést](../images/bridge_settings_enabled_default.png)![Ha a hídbeállítások engedélyezve vannak, az áthidaló vonalakat különböző beállításokkal nyomtatja ki](../images/bridge_settings_enabled_enabled.png)

A Cura általában meglehetősen kezdetleges áthidaló technikát alkalmaz. A Cura felismeri a több oldalról alátámasztott bőr túlnyúló területeit. A [bőrvonalak iránya](../top_bottom/skin_angles.md) úgy van beállítva, hogy automatikusan áthidalja ezeket a területeket. Ez biztosítja, hogy a túlnyúló terület lehető legnagyobb része több oldalról alátámasztva legyen, és javítja a nyomtatási minőséget.

Ha azonban ez a beállítás engedélyezve van, akkor ezt a viselkedést az igényei szerint pontosabban hangolhatja. Ez lehetővé teszi, hogy módosítsa:

- nyomtatási sebesség
- áramlási sebesség
- sűrűség (mint a kitöltési sűrűség, de a bőrvonalakkal együtt)
- ventilátor sebesség
- a falakhoz, szintén partfalhoz

Ezek a beállítások külön állíthatók a hézagot áthidaló bőrhöz és a falakhoz. Ha [a Bridge Has Multi Layers](bridge_enable_more_layers.md) engedélyezve van, akkor ezek külön is beállíthatók az áthidalt rés feletti második és harmadik réteghez. Lehetővé teszi továbbá annak beállítását is, hogy a nyomat mely részeit tekintsük áthidaló területnek, úgy, hogy beállítja [, hogy a terület mekkora hányadának kell a levegő felett lennie](bridge_skin_support_threshold.md) , és [a falak minimális szélességét](bridge_wall_min_length.md) .

Az áthidaló beállítások engedélyezésével jobban szabályozhatja, hogyan kezelje a híd a nyomatban. Az áthidalási paraméterek nagyon jó hangolásával jelentősen javíthatja a túlnyúlások minőségét, és javíthatja a pontosságot függőleges irányban. Az egyetlen hátránya, hogy ha nem állítja be a hídbeállításokat a nyomtatóhoz, akkor a nyomtatás is rosszabb lesz.
