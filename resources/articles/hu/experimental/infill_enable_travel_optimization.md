# Töltse ki az utazásoptimalizálást

A beállítás engedélyezése némileg csökkentheti a nyomat utazási idejét. Az útmozgások hosszának lerövidítésével a nyomat valamivel gyorsabban megy, és a fúvóka is valamivel kevésbé szivárog. A modell szeletelése azonban több időt vesz igénybe.

Általában a Cura meglehetősen naivan optimalizálja a kitöltési vonalak rajzolásának sorrendjét. Cura minden sor után megkeresi a legközelebbi vonalat, és megrajzolja azt. Néhány szokatlan, bonyolult formánál azonban a következő kitöltési vonalhoz vezető út meglehetősen hosszú lehet, mivel a fúvókának [a fésülés](../travel/retraction_combing.md) miatt kitérőt kell tennie. Naiv módon Cura alábecsüli a távolságot, és lehet, hogy hosszabb utazást választ egy rövidebb helyett. Ha ez a beállítás engedélyezve van, a távolságot a rendszer pontosan kiszámítja, így jobb választást lehet tenni.

Ez a beállítás általában csekély hatással van a szeletelés idejére. Azonban a sok apró alkatrészt tartalmazó bonyolult nyomatok esetén (ahol ez a leghasznosabb) nagyságrendekkel megnövelheti a szeletelési időt.
