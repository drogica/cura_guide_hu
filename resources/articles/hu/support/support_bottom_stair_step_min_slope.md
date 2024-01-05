# Támassza meg a lépcsőfok minimális dőlésszögét

Ezzel a beállítással letilthatja a lépcsőzést a tartó legalsó részén, egészen addig, amíg a modell lejtése el nem ér egy bizonyos szöget.

<!--screenshot {
"image_path": "support_bottom_stair_step_min_slope_10.png",
"models": [{"script": "standing_ring.scad"}],
"camera_position": [0, 82, 10],
"camera_lookat": [0, 0, 10],
"settings": {
    "support_enable": true,
    "support_bottom_stair_step_height": 1,
    "support_bottom_stair_step_min_slope": 10
},
"layer": 250,
"colours": 64
}-->

<!--screenshot {
"image_path": "support_bottom_stair_step_min_slope_30.png",
"models": [{"script": "standing_ring.scad"}],
"camera_position": [0, 82, 10],
"camera_lookat": [0, 0, 10],
"settings": {
    "support_enable": true,
    "support_bottom_stair_step_height": 1,
    "support_bottom_stair_step_min_slope": 30
},
"layer": 250,
"colours": 64
}-->

![A lépcsőzés tiltva van, amíg a lejtés 10°-os nem lesz](../images/support_bottom_stair_step_min_slope_10.png)![A lépcsőzés le van tiltva, amíg a lejtés 30°-os nem lesz](../images/support_bottom_stair_step_min_slope_30.png)

Sekély lejtőkön az alsó lépcsőfokok nagyon szélesek lehetnek. Soha nem lehetnek szélesebbek, mint amit a [maximális szélesség](support_bottom_stair_step_width.md) jelez, de mivel ezt a távolságot minden oldalról megtartják, a lépcsőfokok olyan szélesek lehetnek, hogy jelentős távolságra kell áthidalni a támasztékot. Ha van egy kis völgy, amelyben a támasz felfekszik, akkor akár csak az egész alsó oldal kiugrását okozhatja, így a teljes támasz csak a lépcső sarkaira támaszkodik.

Ilyen esetekben korlátozhatja a lépcsőfokokat, hogy csak a meredekebb lejtőkön legyenek. Ez a beállítás határozza meg, hogy ebből a szempontból mi számít "meredek" lejtőnek.

Ennek a beállításnak a növelése megakadályozza, hogy a Cura lépcsőfokokat hozzon létre sekély felületeken. Ez a támasztékot erősebbé teszi, de nehezebb lesz eltávolítani. Támogatása több heget hagy a felszínen. Csökkentése megkönnyíti az alátámasztás eltávolítását, és szebb felületet hagy a támaszték helyén, de bizonyos esetekben előfordulhat, hogy a támasztéknak nagy távolságokat kell áthidalnia, vagy akár úgy is tűnhet, hogy teljesen a levegőben lóg.

A szép felület elérése érdekében a legjobb, ha ezt a beállítást konzervatív alacsony szögben hagyja, 5° vagy 10° vagy így tovább. Ha a támasz sekély, de nem teljesen sík felületen nyugszik, ellenőrizze a rétegnézetet, és növelje a szöget, ha úgy találja, hogy az alátámasztás nagyon bizonytalannak tűnik.
