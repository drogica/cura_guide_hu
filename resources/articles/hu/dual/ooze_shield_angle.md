# Ooze Shield Angle

A szivárgáspajzs követni fogja a modell alakját. Közel kell maradnia, különben a pajzstól a modellig való utazás során új anyag szivárog ki. De a modellnek lehetnek vízszintes felületei, így meredek túlnyúlások keletkeznének a szivárgáspajzsban. Ez a beállítás korlátozza a szivárgáspajzs meredekségét, hogy ne essen össze.

![Ahelyett, hogy alul és felül követné a modellt, nem meredekebb a megadott szögnél](../images/ooze_shield.svg)

- A 0 érték a szivárgáspajzsot teljesen függőleges helyzetbe hozza a teljes alakzat körül. Minél kisebb a szög, annál stabilabb lesz a pajzs.
- A 90-es érték arra készteti a szivárgáspajzsot, hogy pontosan követi a modellt. Minél nagyobb a szög, annál jobban megakadályozza a szivárgást a modellen.

Bár elméletileg ésszerű lenne itt hasonló értéket használni, mint a [Support Overhang Angle](../support/support_angle.md) esetében, a szivárgáspajzs csak egy sor. Ez az egyetlen vonal gyengébb, mint az Ön modellje, és jobban ki van téve a vetemedésnek. Célszerű valamivel sekélyebb szöget használni, mint amilyen a szokásosan jól nyomtatna a modellben, hogy megakadályozza a szivárgáspajzs szétválását.
