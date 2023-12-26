# Tiltott területek

Ez a beállítás jelzi az építőlemez azon területeit, ahová a nyomtatófej nem kerülhet. A felhasználó nem helyezhet el semmilyen tárgyat ezeken a területeken, vagy nem helyezhet olyan közel ahhoz, hogy valami nyomtatást okozzon (például perem).

![A szürke foltok nem engedélyezett területeket jelölnek az építőlemezen található kapcsok körül](../images/machine_disallowed_areas.png)

Ezekre a tiltott területekre azért van szükség, hogy megakadályozzák a nyomtatófej dolgoknak való ütközését. Előfordulhat például, hogy valahol a nyomtatófejtől elérhető egy törlőkefe, vagy egy kapcsolórekesz, vagy egy kamera, amely kissé túlságosan kinyúlik az építési köteten belül. Ha a felhasználó túl közel nyomtatna ezekhez az objektumokhoz, a nyomtatófej összeütközne velük. A legjobb esetben is [rétegeltolást](../troubleshooting/layer_shift.md) kapsz. A legrosszabb esetben károsíthatja a nyomtatófejet vagy bármit, aminek a nyomtatófej ütközik.

A nem engedélyezett területek szürke árnyékként jelennek meg az építőlemezen, jelezve a felhasználónak, hogy nem helyezhet el semmilyen tárgyat. Ezek az árnyékok minden irányba kiterjeszthetők, hogy megakadályozzák a perem vagy a szoknya ütközését, és számos egyéb ok miatt. Más árnyékok is vannak az építőlemezen, például korlátozzák a mozgási tartományt, ha a fúvókák eltolással rendelkeznek.

Ha csak az aktív fúvóka ütközne az akadályokkal, akkor a hasonló beállítású [Nozzle Disallowed Areas (Fúvóka tiltott területek)](nozzle_disallowed_areas.md) meg tudja akadályozni, hogy a fúvóka nekiütközzen, miközben a nyomtatófej áthaladhat rajta.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
