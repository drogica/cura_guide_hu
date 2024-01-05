# Támogatás csatlakozási távolság

A vékony támasztóelemek általában nem kívánatosak. Hajlamosak felborulni, ami tönkreteheti a nyomatot. Ha több támasztóelem van egymás mellett, összeilleszthetők, így egy sokkal szilárdabb tartóelemet alkotnak.

<!--screenshot {
"image_path": "support_join_distance_low.png",
"models": [{"script": "clamp.scad"}],
"camera_position": [-8, 150, 75],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_join_distance": 0.1
},
"colours": 64
}-->

<!--screenshot {
"image_path": "support_join_distance_high.png",
"models": [{"script": "clamp.scad"}],
"camera_position": [-8, 150, 75],
"settings": {
    "support_enable": true,
    "support_interface_enable": true,
    "support_join_distance": 2
},
"colours": 64
}-->

![Két támasztóelem közel van egymáshoz](../images/support_join_distance_low.png)![Megfelelő csatlakozási távolság esetén ezek összeolvadnak](../images/support_join_distance_high.png)

A tartóelemek összekapcsolása masszívabbá és megbízhatóbbá teszi a támasztékot. A mintától függően csökkenti a nyomtatási időt is. Sok minta esetében szükség van egy extra falra a teljes kerületre vagy a kerület egy részére nyomtatni, és két tartóelem összekapcsolása csökkenti ezt a kerületet.

Ennek a beállításnak a túlzott növelése a nagyon távol lévő tartóelemek összeillesztését okozhatja. Ez növelheti a nyomtatási időt és az anyagfelhasználást.
