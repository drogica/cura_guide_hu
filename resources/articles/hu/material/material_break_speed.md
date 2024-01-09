# Törés visszahúzási sebesség

Egyes nyomtatóknál, amikor egy anyagot visszahúznak egy izzószál-kapcsolóhoz, az anyagot tisztán le kell törni, hogy összegabalyodás nélkül áthaladhasson az adagolón. Ez a beállítás az eljárás egy részét úgy konfigurálja, hogy tisztán törje meg.

Ez a beállítás beállítja az anyag visszahúzási sebességét, hogy végül letörje az izzószálat a foltról, amely elkerülhetetlenül a fúvókában marad. Míg a fúvókában lévő folt olvadt állapota miatt nem húzható ki, addig a kihúzott rész hegyénél ne legyen vékony szál, mert az beakadhat az adagolóba. Ez a végső visszahúzás eltöri az izzószálat, de remélhetőleg tisztán törik az előző két szakasznak köszönhetően.

![Először az anyagot visszahúzzuk, hogy megállítsuk a szivárgást](../images/filament_switch_anti_ooze.svg)![Másodszor, az izzószálat lassan visszahúzzák, hogy vékony szálat húzzanak, amely könnyen elszakad, és hagyja, hogy ez a szál megszilárduljon](../images/filament_switch_break_preparation.svg)![Harmadszor, az izzószálat gyorsan visszahúzzák, hogy az izzószál elszakadjon](../images/filament_switch_break.svg)

**Ez a beállítás jelenleg soha nem látható a Cura felületén. Csak a profilok állíthatók be. Szeleteléskor sem használja a Cura. Azok a nyomtatók azonban, amelyek megértik a Cura anyagfájlformátumát, használhatják azt az izzószál-váltási eljárás helyes konfigurálásához.** Egy utófeldolgozó szkripten keresztül az `M600` parancs beilleszthető a nyomtatásba, ami egy izzószál kapcsolót indít el.
