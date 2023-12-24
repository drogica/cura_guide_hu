# Szeletelési tolerancia

A szeletelési tűréssel beállíthatja, hogyan kezelje a háló véges mennyiségű rétegre történő felosztásának pontatlanságát. Lehetővé teszi annak kiválasztását, hogy a rétegek szorosan közelítsék-e a felületet, maradjanak a felület által határolva, vagy teljesen magukba foglalják-e a felületet.

## Középső

![Középső](../images/slicing_tolerance_middle.svg)

Közép használatakor a rétegek a lehető legközelebb maradnak az eredeti felülethez. Ez azt jelenti, hogy a rétegek néha kinyúlnak az eredeti felületen, néha pedig belemerülnek az eredeti felületbe. Összességében a rétegek térfogata nagyon szorosan megegyezik az eredeti háló térfogatával.

A középső tűrés eléréséhez a Cura kiszámol egy keresztmetszetet az egyes rétegek vastagságának felénél. A keresztmetszeten belül minden a réteg részévé válik.

## Beleértve

![Beleértve](../images/slicing_tolerance_inclusive.svg)

Az Inclusive használatakor a rétegek *legalább* az eredeti kötet teljes részét tartalmazzák. Ahol a felület lejtős, ott a rétegek enyhén kinyúlnak. A rétegek teljes térfogata szinte mindig nagyobb lesz, mint az eredeti háló térfogata.

Az Inclusive tolerancia eléréséhez a Cura kiszámolja az egyes rétegek magasságának tetején és alján lévő keresztmetszeteket. Minden olyan felület, amely ezen keresztmetszetek *bármelyikén* található, a réteg részének lesz tekintve. A két keresztmetszet közé eső apró részleteket a rendszer figyelmen kívül hagyja, mivel ezek kisebbek egy rétegmagasságnál.

## Kizárólagos

![Kizárólagos](../images/slicing_tolerance_exclusive.svg)

Az Exclusive használatakor a rétegek az eredeti köteten belül lesznek. Ahol a felület lejtős, a rétegek valamivel kisebbek lesznek, mint az eredeti térfogat. A rétegek teljes térfogata szinte mindig kisebb lesz, mint az eredeti háló térfogata.

Az exkluzív tűrés eléréséhez a Cura kiszámolja az egyes rétegek magasságának tetején és alján lévő keresztmetszeteket. Csak azokat a felületeket tekintjük a réteg *részének* , amelyek mindkét keresztmetszetben vannak.

## Használat

Ez a beállítás a rendeltetésszerű használatáról, nem pedig a funkcionális hatásáról kapta a nevét. Ha több darabja van, amelyeknek egymás mellett kell elcsúszniuk, a rétegek elméleti formája fizikailag megakadályozhatja a pontos illeszkedést. Ilyen esetben ezt a beállítást Exkluzívra állíthatja, így a rétegek garantáltan az eredeti kötet határain belül maradnak. A vetemedés, megereszkedés és hasonló deformációs hatások kizárásával ez garantálná, hogy az alkatrészek egymásba illeszkedjenek, és képesek legyenek egymás mellett elcsúszni.

Valójában mindig vannak más hatások, amelyek ezt megakadályozzák. A gyakorlatban ezzel a beállítással két lejtős felület között valamivel több-kevesebb tűrést lehet elérni, amint az a fenti képeken is látható.
