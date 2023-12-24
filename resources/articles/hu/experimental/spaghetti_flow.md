# Spagetti Flow

Ez a beállítás közvetlenül beállítja a spagetti töltelék sűrűségét.

Normál esetben a kitöltés nyomtatása közben a [kitöltési sűrűség](../infill/infill_sparse_density.md) beállítása csak a [kitöltési vonalak közötti távolságot](../infill/infill_line_distance.md) befolyásolja. Mivel a [kitöltési vonal szélessége](../resolution/infill_line_width.md) változatlan marad, de a vonalak közelebb vannak egymáshoz, a kitöltési sűrűség növelése azzal a hatással jár, hogy a betöltési térfogat nagyobb része a végén megtelik anyaggal.

Ez másként működik, ha [a spagetti kitöltés](spaghetti_infill_enabled.md) engedélyezve van. A kitöltési vonal távolsága nemcsak a kitöltővonalak közötti távolságot állítja be, hanem a vonal szélességét is beállítja a beállítás által meghatározott kívánt sűrűség elérése érdekében. Ez a beállítás pontosan meghatározza a teljes feltöltési mennyiségnek azt a hányadát, amelyet meg kell tölteni anyaggal. A beállítás növelésével a vonalak szélesebbek lesznek.

Ha spagettibetétet használ rugalmas töltelék előállításához, ez a beállítás lényegében meghatározza, hogy milyen merev lesz a kitöltőanyag. Az áramlás csökkentése lágyabb töltetet eredményez, míg az áramlás növelése merevebbé teszi a feltöltést. Az áramlás túlzott csökkentése azonban megakadályozza, hogy a töltet egyenletesen oszlassa el. Hajlamos lesz leesni a kötet alja felé, és ott halom spagettit termelni, amely nem növeli a tetejének merevségét.

Ha spagettibetétet használ az öntvényhez, ezt a beállítást valószínűleg 100% közelébe kell beállítani, hogy a modell teljesen megteljen anyaggal. Ennek ellenére kissé módosíthatja, ha az anyag zsugorodni vagy kitágulni kötődik.

**Ez a beállítás továbbra is megszorozódik a [betöltési áramlás](../material/infill_material_flow.md) beállításával.**
