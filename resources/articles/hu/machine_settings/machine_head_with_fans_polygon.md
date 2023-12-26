# Gépfej és ventilátor sokszög

Ez a beállítás megmondja Curának, hogy felülről nézve milyen a nyomtatófej alakja. Erre azért van szükség, hogy elkerüljük az ütközéseket [egyenkénti](../blackmagic/print_sequence.md) nyomtatáskor.

![A nyomtatófej méretei](../images/head_dimensions.svg)![Felülről lefelé nézve a nyomtatófej alakja a fúvóka helyzetéhez viszonyítva van](../images/machine_head_with_fans_polygon.png)

Ez a beállítás a sokszöget alkotó koordináták listáját tartalmazza. A koordináták a fej "pozíciójához" vonatkoznak, ehhez képest a fúvókák is relatíve helyezkednek el.

A Cura ezt arra használja, hogy ütközési területet hozzon létre a nyomtatott objektumok körül, egyesével módban. Ez az ütközési terület megakadályozza, hogy tárgyakat túl közel helyezzen egymáshoz, hogy ne lehessen őket kinyomtatni anélkül, hogy a nyomtatófej hozzáütődne a korábban nyomtatott modellhez. Az ütközési terület azonban nem olyan alakú, mint maga a nyomtatófej: A nyomtatófej körül domború héj lesz, hogy megakadályozza az ütközéseket az utazás során is. Szintén szimmetrikusra zsugorodik. Például, ha a fúvóka jobban a nyomtatófej bal oldala felé van (mint a fenti képen), akkor az ütközési terület úgy zsugorodik, hogy egy másik tárgy kerülhet közel a korábban nyomtatott objektumok jobb oldalához. Az objektumok nyomtatási sorrendje ezután úgy lesz beállítva, hogy ütközések nélkül kinyomtathatók legyenek.

**Mivel ez egy gépbeállítás, általában nem jelenik meg a normál beállítások listájában. A nyomtatófej mérete azonban durván leírható a nyomtatóbeállítások párbeszédablakban, amely a beállítások párbeszédablakban található a hozzáadott nyomtatók listájában. Ott csak a nyomtatófej bal, jobb felső és alsó oldalának pozícióját adhatja meg.**
