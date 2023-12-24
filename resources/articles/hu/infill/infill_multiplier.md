# Kitöltési sorszorzó

Ennek a beállításnak a növelésével a Cura több kitöltési sort helyez el közvetlenül a többi kitöltősor mellé.

<!--screenshot {
"image_path": "infill_multiplier.png",
"models": [{"script": "gear_knurled.scad"}],
"camera_position": [18, 0, 180],
"settings": {
    "top_layers": 0,
    "infill_multiplier": 3
},
"colours": 32
}-->

![3-mal szorozva](../images/infill_multiplier.png)

Ez hatékonyan növeli a kitöltési sűrűséget a [Kitöltési sűrűség](infill_sparse_density.md) beállításnál megadott érték fölé, de ahelyett, hogy a kitöltési sorokat egyenletesen elosztaná, a vonalak közvetlenül egymás mellé kerülnek. A kitöltési sűrűség egyszerű növeléséhez képest ez növelheti a kitöltés szilárdságát, mivel a kitöltő vonalak képesek egymásra támaszkodni az extra merevség érdekében.

Ha páratlan szorzót állít be, az eredeti kitöltő vonalak a helyükön maradnak, de további kitöltő vonalak körbe fognak hurkolni a kitöltőminta lyukaiban. Ha páros szorzót állít be, az eredeti kitöltő vonalak eltávolításra kerülnek, és a hurkok közvetlenül a helyükre kerülnek.

A kitöltési sűrűség ugyanazzal a szorzóval történő növelésével összehasonlítva ez néhány hatással lesz a nyomatára.

- A kitöltés összességében merevebbé válik, hasonlóan a kitöltővonal szélességének növeléséhez, mivel a kitöltővonalak nyíróerő hatására képesek egymásra dőlni.
- A kitöltés jobban átvilágít a bőrön, csökkentve a felület minőségét.
- A kitöltővonalak közötti hézagok nagyobbak, mivel a vonalak jobban össze vannak kötve. Ezáltal a bőr jobban megereszkedik, és lehetővé válik a párnázás.

**Ennek a beállításnak nincs hatása, ha a kitöltési sűrűség 100% vagy magasabb.**
