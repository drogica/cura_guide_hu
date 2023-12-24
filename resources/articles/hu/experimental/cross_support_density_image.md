# Keresztkitöltés sűrűségű kép a támogatáshoz

Ebben a beállításban megadhat egy képet, amely meghatározza a sűrűséget a támogatás különböző helyein. A támasztósűrűség bizonyos helyeken a kép fényességétől függően változhat. Ez csak a [keresztmintára](../support/support_pattern.md) működik, mivel ez a minta képes beállítani a sűrűségét anélkül, hogy a vonalakat feldarabolná, ami megszakadt áramlást és csökkentett erőt eredményezne.

<!--screenshot {
"image_path": "cross_support_density_image.png",
"models": [{"script": "wide_bridge.scad"}],
"camera_position": [0, 0, 120],
"layer": 79,
"settings": {
    "support_enable": true,
    "support_pattern": "cross",
    "support_infill_rate": 100,
    "cross_support_density_image": "{root}/resources/articles/images/cross_support_density_image_mask.png"
},
"colours": 32
}-->

![Az oldalsó támaszsűrűség nagyobb](../images/cross_support_density_image.png)![A minta létrehozásához használt képfájl](../images/cross_support_density_image_mask.png)

A kép elérési útja helyi elérési útként van megadva, például `C:\ProjectsD Printing\support_density.png` Windows rendszeren vagy `/home/ghostkeeper/3d_printing/support_density.png` Unix rendszeren. A támogatott fájlformátumok: JPG, PNG, TGA, BMP, PSD, GIF, HDR és PIC. A kép a nyomat fölé van méretezve, hogy pontosan illeszkedjen a nyomtatott jelenet határolókeretéhez. A kép fényereje határozza meg a támaszsűrűséget:

- Ahol a kép fekete, ott a [támaszsűrűség](../support/support_infill_rate.md) kerül felhasználásra.
- Ahol a kép fehér, a támasztósűrűség megközelíti a 0%-ot.

A támaszsűrűség soha nem haladja meg a [támasztóvonal távolság](../support/support_line_distance.md) által meghatározott értéket. Csak csökkenteni lehet. A minta korlátozott abban is, hogy hol csökkentheti a sűrűségét. Noha megpróbálja a lehető legpontosabban megközelíteni a kívánt alátámasztási sűrűséget, ez nem mindig lehetséges. Ha az alátámasztás sűrűsége nagyon alacsony, akkor különösen kevés lehetőség lesz a támasztósűrűség beállítására, így a nyomat nagyon lazán követi a képet. Azokon a helyeken, ahol nagy a támaszsűrűség, nagyon szorosan követni fogják a képet. A választott sűrűség is erősen kvantált. A sűrűség csak megduplázható vagy felére csökkenthető, de a Cura a nagyobb pontosság elérése érdekében [torzítja](https://en.wikipedia.org/wiki/Dither) a mintát.

Ezzel a beállítással nagyon testreszabhatja a támogatást. Ha a nyomat bizonyos részei hajlamosak megereszkedni, vagy nagyon pontosan kell nyomtatni, akkor helyileg növelheti a sűrűséget, hogy jobban alátámassza őket, anélkül, hogy nagyot kellene húznia a nyomtatási időbe, vagy megnehezítené a támaszték lehúzását.

**Ez a beállítás nem fog jól átvinni Cura projektfájlokat. A projektfájl a kép elérési útját tárolja beállítási értékként, de nem tárolja a képet. Ha a projektfájlt egy másik számítógépen nyitják meg, a sűrűségkép valószínűleg nem kerül visszaállításra.**
