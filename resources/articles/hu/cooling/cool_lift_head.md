# Emelje fel a fejet

A [Minimális rétegidő](cool_min_layer_time.md) elérésekor a nyomtatófej lelassul, hogy megakadályozza a Minimális rétegidőnél gyorsabb nyomtatást. Így az előző rétegnek van ideje kihűlni és megszilárdulni, mielőtt a következő réteget feltesszük. A nyomtatófej lelassul, amíg el nem éri a [Minimális sebességet](cool_min_speed.md) .

Ha ez a beállítás engedélyezve van, és a nyomtatófejnek lassabban kell mozognia a Minimális sebességnél a minimális rétegidő fenntartása érdekében, akkor a nyomtatófej kissé felfelé mozdul a réteg kinyomtatása után. Ezután vár egy ideig, amíg el nem éri a minimális rétegidőt, mielőtt a következő réteggel kezdené.

Ha ez a beállítás le van tiltva, a nyomtató azonnal folytatja a következő réteggel. Nem fogja megvárni a minimális rétegidőt, így a rétegek olyan rétegek tetejére lesznek nyomtatva, amelyek talán még nem szilárdultak meg teljesen.

![A minimális rétegezési idő elérésekor a fej felemelkedhet](../images/cool_fan_speed.svg)

A nyomtatófej mindig 3 mm-rel felfelé mozog. Jelenleg nincs beállítás ennek konfigurálására.

## Kompromisszumok

A fúvóka lassítása esetén kompromisszum van, hogy a réteg jobban lehűljön. A minimális rétegidő arra szolgál, hogy a nyomtatófej mozgásának lelassításával némi időt biztosítson az anyag lehűléséhez. Ezalatt a ventilátorok maximális erővel fújnak, hogy gyorsabban lehűljenek, de a forró fúvóka is a műanyagon van. Nagyon kis darabok esetén a forró fúvóka több hőt adhat át a nyomatnak, mint amennyit a ventilátorok el tudnak fújni. Emiatt a műanyag még jobban megolvad, mintha nem lenne minimális rétegezési idő.

A Lift Head segítségével ez a kompromisszum megoldódik. Egy pontig még lassíthat, de nagyon kis rétegek esetén elmozdítja a forró fúvókát, így nem ad tovább hőt a nyomatba. A fejet elég közel tartják ahhoz, hogy a nyomtatófej ventilátorai továbbra is ráfújjanak a nyomatra.

Ennek az a hátránya , hogy hatékonyan csinál egy [Z ugrást](../travel/retraction_hop.md) , ami némi [húrozást](../troubleshooting/stringing.md) eredményez . Míg a fej felemelése javíthatja a megereszkedést és a foltosodást, másfajta rendetlenséget okoz. Egy kis kézi utófeldolgozás késsel megtisztíthatja az általa okozott húrokat.
