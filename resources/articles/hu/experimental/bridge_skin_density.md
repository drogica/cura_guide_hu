# A híd bőr sűrűsége

Ez a beállítás szabályozza a nyomat alsó részének sűrűségét, ahol áthidalja a rést. 100%-os sűrűségnél a vonalak közvetlenül egymás mellett helyezkednek el. Kisebb sűrűségnél a vonalak távolabb helyezkednek el egymástól.

<!--screenshot {
"image_path": "bridge_skin_density_100.png",
"models": [{"script": "bridge.scad"}],
"layer": 80,
"settings": {
    "bridge_settings_enabled": true,
    "bridge_skin_density": 100,
    "bridge_skin_material_flow": 100,
    "bridge_wall_material_flow": 100
},
"camera_position": [0, 18, 79],
"colours": 64
}-->

<!--screenshot {
"image_path": "bridge_skin_density_50.png",
"models": [{"script": "bridge.scad"}],
"layer": 80,
"settings": {
    "bridge_settings_enabled": true,
    "bridge_skin_density": 50,
    "bridge_skin_material_flow": 100,
    "bridge_wall_material_flow": 100
},
"camera_position": [0, 18, 79],
"colours": 64
}-->

![100%-os sűrűségnél a vonalak közvetlenül egymás mellett helyezkednek el](../images/bridge_skin_density_100.png)![50%-os sűrűségnél van némi térköz a sorok között](../images/bridge_skin_density_50.png)

Két fő effektus játszik szerepet ennek a beállításnak a hangolásakor: a vonalak közötti tapadás és a hűtés.

Ha a bőrvonalak közvetlenül egymás mellett helyezkednek el, akkor egymáshoz tapadnak. Így az áthidalt rés alsó oldala szebb lesz, mivel a felület folyamatos lesz, nem fűződik. Ezenkívül a második vonal egy kicsit az első vonalra támaszkodhat áthidalás közben, ami egy kicsit kevésbé ereszkedik meg.

Van azonban egy másik hatás is: a hűtés. Ha a vonalak távolabb helyezkednek el egymástól, gyorsabban tudnak lehűlni, és akkor sem ereszkednek meg annyira. Természetesen ez csak akkor érvényes, ha a ventilátor be van kapcsolva, így a magas hőmérsékletű anyagok esetében ez a stratégia nem működik.

Hogy ezek közül melyik hatás erősebb, az az anyag viszkozitásától, a megszilárdulás sebességétől és a ventilátor sebességétől függ. Némi hangolás mindig szükséges.

**Ha a [Bridge Skin Flow](bridge_skin_material_flow.md) kisebb, mint 100%, akkor is lesz némi térköz a sorok között, még akkor is, ha a sűrűség 100%, mert akkor a vonalak vékonyabbak lesznek.**
