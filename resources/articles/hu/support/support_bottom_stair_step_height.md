# Támassza meg a lépcsőfokok magasságát

Ha [a Support Placement](support_type.md) beállítása "Mindenhol", akkor a támogatás a modellen nyugszik. Ennek ellenére nem fogja pontosan követni a modell körvonalait. Ehelyett a tartó alsó oldala lépcsőzetes mintát kap. Így a támogatás csak néhány helyen létesít kapcsolatot a modellel.

Ez a beállítás határozza meg ezeknek a lépcsőknek a magasságát.

<!--screenshot {
"image_path": "support_bottom_stair_step_height.png",
"models": [{"script": "standing_ring.scad"}],
"camera_position": [0, 136, 10],
"camera_lookat": [0, 0, 10],
"settings": {
    "support_enable": true,
    "support_bottom_stair_step_height": 1
},
"colours": 64
}-->

![A támasz alján lépcsőfokok alakulnak ki](../images/support_bottom_stair_step_height.png)

A lépcsőfok magasságát a modell felületétől való távolság számolja. Ez azt jelenti, hogy ha van egy függőleges távolság a [Support Bottom Distance](support_bottom_distance.md) beállításban, akkor ezt levonjuk a magasságból, és a modell és a támasz közötti kapcsolat nagyobb lesz. Hasonlóképpen, a [Support Floor](support_bottom_enable.md) a lépcsőfokok hatását is csökkenti.

A [Lépcső támasztékának maximális szélessége](support_bottom_stair_step_width.md) beállítás korlátozza a lépcsők szélességét. Ha a modell felülete olyan sekély, hogy egy kis lépcsőmagasság hatalmas lépésszélességet vonna maga után, a támaszték a lépésmagasság hátralévő részében követi a modell felületét.

Ha csökkenti ezt a beállítást, a támaszték alja simább lesz. Ez növeli a tapadást a tartó és a modell között, ami megnehezíti a támaszték eltávolítását, de egyben stabilabbá is teszi a támasztékot.
