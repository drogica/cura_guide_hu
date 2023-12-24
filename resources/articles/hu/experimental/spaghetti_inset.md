# Spagetti betét

Ahhoz, hogy a spagetti töltelék minden irányban egyformán táguljon, bizonyos távolságot kell tartani a falaktól. Ez a beállítás határozza meg ezt a távolságot.

Ennek a beállításnak a viselkedése majdnem megegyezik a [kitöltési átfedés](../infill/infill_overlap_mm.md) beállításával. Ha a feltöltési átfedés ennek a beállításnak a negatív értékére van beállítva, akkor az a terület, amelyen a fúvóka áthalad, ugyanaz lesz. A különbség azonban az, hogy ezzel a beállítással a kitöltéshez extrudált teljes mennyiség változatlan marad. Míg a kitöltés átfedésének csökkentése csökkenti a kitöltésként extrudált anyag mennyiségét, ennek a beállításnak a módosítása nem módosítja a kitöltésként extrudált teljes mennyiséget.

Ha a spagettibetétet rugalmas kitöltési mintaként használja, ezt a beállítást úgy kell beállítani, hogy az anyag lefelé haladva ne ütközzen a falakhoz, mielőtt ráfeküdne az anyagra. Ha a betét túl kicsi, a spagetti betét csak a falakhoz tapad, és ott nagy anyagfoltokat hoz létre. Ha azonban a betét túl nagy, akkor az összes anyag középre koncentrálódik, ahelyett, hogy minden oldalról azonos mennyiségű szilárdságot adna.

Ha spagetti tölteléket használ az öntéshez, ezt úgy kell beállítani, hogy a szélesebb öntőfúvókákhoz igazodjon, amelyek jellemzőek az anyagok öntésére alkalmas nyomtatókra, így az anyag ne folyjon át a falon a kitöltő térfogaton kívül.
