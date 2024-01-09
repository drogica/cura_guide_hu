# Szivárgásgátló visszahúzási sebesség

Egyes nyomtatóknál, amikor egy anyagot visszahúznak egy izzószál-kapcsolóhoz, az anyagot tisztán le kell törni, hogy összegabalyodás nélkül áthaladhasson az adagolón. Ez a beállítás az eljárás egy részét úgy konfigurálja, hogy tisztán törje meg.

Ez a beállítás azt a sebességet állítja be, amellyel az anyag visszahúzódik az első pozíció felé, hogy megakadályozza annak kiszivárgását. Az anyag ezen a ponton még nincs letörve. Célja csak a fúvókakamrára nehezedő nyomás gyors megszüntetése a befelé húzással.

![Először az anyagot vissza kell húzni, hogy megállítsák a szivárgást, ennek a beállításnak megfelelően](../images/filament_switch_anti_ooze.svg)![Másodszor, az izzószálat lassan visszahúzzák, hogy vékony szálat húzzanak, amely könnyen elszakad, és hagyja, hogy ez a szál megszilárduljon](../images/filament_switch_break_preparation.svg)![Harmadszor, az izzószálat gyorsan visszahúzzák, hogy az izzószál elszakadjon](../images/filament_switch_break.svg)

**Ez a beállítás jelenleg soha nem látható a Cura felületén. Csak a profilok állíthatók be. Szeleteléskor sem használja a Cura. Azok a nyomtatók azonban, amelyek megértik a Cura anyagfájlformátumát, használhatják azt az izzószál-váltási eljárás helyes konfigurálásához.** Egy utófeldolgozó szkripten keresztül az `M600` parancs beilleszthető a nyomtatásba, ami egy izzószál kapcsolót indít el.
