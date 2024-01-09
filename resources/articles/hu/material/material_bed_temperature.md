# Építési lemez hőmérséklete

Egyes nyomtatók fűtött építőlemezzel rendelkeznek. Ez a beállítás határozza meg, hogy az építőlemez mennyire lesz meleg.

Az építőlemez melegítése enyhén folyékony és ragacsos marad az anyagban. Egyes anyagok fagyáskor kristályokat képeznek, ami miatt az anyag fagyáskor jelentősen összezsugorodik. A fűtött ágy éppen fagypont felett tartja az anyagot, hogy megakadályozza ezt a zsugorodást és fenntartsa a folyékony műanyag ragadósságát. Mindez arra szolgál, hogy javítsa a nyomat tapadását az alaplaphoz.

Ha azonban az építõlapot túl melegen tartják, a nyomat nagyon folyékony lesz ott, ahol hozzáér az építõlemezhez. Emiatt az anyag kissé megereszkedik, és [elefántláb](../troubleshooting/elephants_foot.md) jelenik meg a nyomat alsó oldalán. Ez kompenzálható az [Initial Layer Horizontal Expansion](../shell/xy_offset_layer_0.md) beállítással, de hatással van a méretpontosságra. Az építőlemez felmelegítése hőmérséklet-különbséget hoz létre az építőlemezen nyugvó anyag és a modellben magasabban lévő anyag között, ami [vetemedést](../troubleshooting/warping.md) okoz, amikor a magasabban lévő anyag zsugorodni kezd.

Ha ez a beállítás 0 fokra van állítva, a Cura nem ad ki semmilyen parancsot az építőlemez hőmérsékletének megváltoztatására, ami megzavarhatja a firmware-t, ha nincs építőlemez.

**Amikor beállítja az építőlemez hőmérsékletét egy anyagprofilban, ez módosítja az [alapértelmezett építőlemez hőmérséklet](default_material_bed_temperature.md) beállítást. Általában az építési lemez hőmérséklete megegyezik az alapértelmezett építési lemez hőmérsékletével, de néha más minőség kiválasztása kis mértékben módosíthatja az építőlemez hőmérsékletét. Ez az építési lemezhőmérséklet beállítás az a beállítás, amely ténylegesen a nyomtatáshoz használatos.**
