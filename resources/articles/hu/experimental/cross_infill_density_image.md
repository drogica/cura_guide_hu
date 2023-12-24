# Kereszt kitöltési sűrűségű kép

Ebben a beállításban megadhat egy képet, amely meghatározza a sűrűséget a kitöltés különböző helyein. A feltöltési sűrűség bizonyos helyeken a kép fényességétől függően változhat. Ez csak a [Cross (3D) minta](../infill/infill_pattern.md) esetén működik, mivel ez a minta képes beállítani a sűrűségét anélkül, hogy a vonalakat feldarabolná, ami megszakadt áramlást és csökkentett erőt eredményezne.

<!--screenshot {
"image_path": "cross_infill_density_image.png",
"models": [{"script": "hexagonal_prism.scad"}],
"camera_position": [0, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_pattern": "cross_3d",
    "infill_sparse_density": 101,
    "cross_infill_density_image": "{root}/resources/articles/images/cross_infill_density_image_mask.png"
},
"colours": 32
}-->

![A kitöltési sűrűség az objektumonként változik](../images/cross_infill_density_image.png)![A minta létrehozásához használt képfájl](../images/cross_infill_density_image_mask.png)

A kép elérési útja helyi elérési útként van megadva, például `C:\ProjectsD Printing\infill_density.png` Windows rendszeren vagy `/home/ghostkeeper/3d_printing/infill_density.png` Unix rendszeren. A támogatott fájlformátumok: JPG, PNG, TGA, BMP, PSD, GIF, HDR és PIC. A kép az objektumra méretezett úgy, hogy pontosan illeszkedjen az objektum határolókeretéhez. A kép fényereje határozza meg a kitöltési sűrűséget:

- Ha a kép fekete, ott a [kitöltési sűrűséget](../infill/infill_sparse_density.md) használják.
- Ahol a kép fehér, a kitöltési sűrűség megközelíti a 0%-ot.

A kitöltés sűrűsége soha nem haladja meg a [kitöltési vonal távolsága](../infill/infill_line_distance.md) által megadott értéket. Csak csökkenteni lehet. A minta korlátozott abban is, hogy hol csökkentheti a sűrűségét. Noha megpróbálja a lehető legpontosabban megközelíteni a kívánt kitöltési sűrűséget, ez nem mindig lehetséges. Ha a kitöltés sűrűsége nagyon alacsony, akkor különösen kevés lehetőség lesz a kitöltési sűrűség beállítására, ami miatt a nyomat nagyon lazán követi a képet. Azokon a helyeken, ahol nagy a kitöltési sűrűség, nagyon szorosan követik a képet. A választott sűrűség is erősen kvantált. A sűrűség csak megduplázható vagy felére csökkenthető, de a Cura a nagyobb pontosság elérése érdekében [torzítja](https://en.wikipedia.org/wiki/Dither) a mintát.

Ezzel a beállítással nagyon testreszabhatja a kitöltést. Mivel a Cross Infill mintákat legtöbbször rugalmas anyagokkal használják, ez a beállítás nagyon specifikus lágysági vagy keménységi korlátozások elérésére szolgál. Például nyomtathat egy cipőtalpat testreszabott puhasággal, hogy jobban illeszkedjen a lábhoz, vagy egy mechanikus eszközt, amelynek bizonyos részeken meg kell hajolnia.

**Ez a beállítás nem fog jól átvinni Cura projektfájlokat. A projektfájl a kép elérési útját tárolja beállítási értékként, de nem tárolja a képet. Ha a projektfájlt egy másik számítógépen nyitják meg, a sűrűségkép valószínűleg nem kerül visszaállításra.**
