# Híd ritka kitöltés max. sűrűsége

Ha nagyon alacsony kitöltési sűrűséggel nyomtat, a felső bőr hajlamos megereszkedni, ami [párnásodást](../troubleshooting/pillowing.md) és általában szabálytalan felületeket okoz a nyomat felső oldalán. Opcionálisan az áthidaló technikák a felső bőrfelületen is alkalmazhatók. Ez a beállítás konfigurálja, hogy az áthidaló technika milyen kitöltési aránynál kezdje el alkalmazni.

<!--screenshot {
"image_path": "bridge_sparse_infill_max_density.png",
"models": [
    {
        "script": "stamp.scad",
        "transformation": ["scale(0.5)"]
    }
],
"layer": 108,
"settings": {
    "bridge_settings_enabled": true,
    "bridge_sparse_infill_max_density": 100
},
"camera_position": [58, 27, 104],
"colours": 64
}-->

![A bőr áthidalja a kitöltést](../images/bridge_sparse_infill_max_density.png)

Ez a beállítás küszöbértékként van konfigurálva, hogy a profilok egyetlen értéket tartalmazhassanak. Míg a felhasználó folyamatosan állítja a kitöltés sűrűségét, a bőr áthidalása automatikusan engedélyezve vagy letiltva lesz.

A felső bőr áthidalása általában simább felső felületet eredményez nagyon alacsony feltöltési arány mellett. Ügyeljen azonban arra, hogy ha ezt használja, elegendő [felső réteg](../top_bottom/top_layers.md) álljon rendelkezésre a felület megfelelő lezárásához anélkül, hogy áthidaló technikát alkalmazna a legmagasabb rétegeken. Az áthidaló technika, különösen a csökkentett [vonalszélesség](bridge_skin_material_flow_3.md) mellett, nem zárja le teljesen a felületet. Ha a felső bőrön nincs elég réteg, akkor lyukak lesznek a nyomatban, és csökken a szilárdság.
