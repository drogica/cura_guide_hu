# Kezdeti réteg alsó áramlása

A kezdeti réteg áramlása az [Initial Layer Flow](material_flow_layer_0.md) beállítással módosítható, de ez a beállítás lehetővé teszi a kezdeti réteg finomabb részleteinek szabályozását azáltal, hogy csak a bőr áramlását módosítja az első rétegen.

A kezdeti réteg egyes részei nagyobb valószínűséggel leválnak az építőlemezről, mint mások. A nyomat első sorai a legveszélyesebbek. Ezzel a beállítással csökkentheti a bőr áramlását, hogy megelőzze a túlextrudálást, miközben magasabban tartja a nyomat falainak áramlását.

Ha a kezdeti réteg áramlása túl magas, a bőr hullámosodását okozhatja, ami csúnya hatást kelt a nyomat alján, és a nyomat a nyomtatás során leszakadhat az építőlemezről. Ez nem jelent olyan nagy problémát a falaknak. Ezt az áramlást célszerű alacsonyabb szinten tartani, mint a [külső](wall_0_material_flow_layer_0.md) és [belső falak](wall_x_material_flow_layer_0.md) áramlását.
