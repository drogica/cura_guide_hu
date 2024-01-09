# Fúvóka nem engedélyezett területek

Ez a beállítás jelzi az építőlemez azon területeit, ahol az aktív fúvóka nem kerülhet. A felhasználó nem helyezhet el semmilyen tárgyat ezeken a területeken, vagy nem helyezhet olyan közel ahhoz, hogy valami nyomtatást okozzon (például perem).

![A szürke foltok nem engedélyezett területeket jelölnek az építőlemezen található kapcsok körül](../images/machine_disallowed_areas.png)

Ez a beállítás csak az *aktív fúvókára* vonatkozik, ami azt jelenti, hogy továbbra is nyomtathat objektumokat ezekhez a tiltott területekhez, még akkor is, ha emiatt más fúvókák áthaladnának ezeken a nem engedélyezett területeken. Mint ilyen, ez a beállítás valóban csak azoknál a nyomtatóknál hasznos, amelyek inaktív állapotban felemelik az inaktív fúvókákat, vagy leállítják őket az építési köteten kívül. A szokásos [tiltott területekkel](machine_disallowed_areas.md) ellentétben ezek a tiltott területek nem mozognak a fúvókák közötti eltolástól függően.

Ezek a tiltott területek azért szükségesek, hogy megakadályozzák a fúvóka tárgyaknak való ütközését. Lehet például néhány klip az építőlemezen, vagy matrica vagy logó. Ha a felhasználó túl közel nyomtatna ezekhez a tárgyakhoz, a fúvóka ütközne velük. A legjobb esetben is [rétegeltolást](../troubleshooting/layer_shift.md) kapsz. A legrosszabb esetben megsérül a fúvóka vagy bármi, aminek a fúvóka ütközik.

A nem engedélyezett területek szürke árnyékként jelennek meg az építőlemezen, jelezve a felhasználónak, hogy nem helyezhet el semmilyen tárgyat. Ezek az árnyékok minden irányba kiterjeszthetők, hogy megakadályozzák a perem vagy a szoknya ütközését, és számos egyéb ok miatt. Más árnyékok is vannak az építőlemezen, például korlátozzák a mozgási tartományt, ha a fúvókák eltolással rendelkeznek.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
