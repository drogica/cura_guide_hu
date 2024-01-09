# Öblítési öblítési sebesség

Ha a nyomtatónak váltania kell, hogy melyik izzószál megy át egy adott fúvókán, akkor ki kell öblítenie a maradék anyagot, amely még a fúvókakamrában volt. Ez a beállítás határozza meg, hogy az izzószál milyen gyorsan tolódik át az adagolón a régi anyag eltávolítása érdekében.

Ez csak a másik típusú anyagra való váltás utáni pillanatra vonatkozik. Ha ugyanilyen típusú anyagot töltünk újra (pl. mert az előző orsó üres volt), [akkor más sebességet](material_end_of_filament_purge_speed.md) használunk.

**Ez a beállítás jelenleg soha nem látható a Cura felületén. Csak a profilok állíthatók be. Szeleteléskor sem használja a Cura. Azok a nyomtatók azonban, amelyek megértik a Cura anyagfájlformátumát, használhatják azt az izzószál-váltási eljárás helyes konfigurálásához.** Egy utófeldolgozó szkripten keresztül az `M600` parancs beilleszthető a nyomtatásba, ami egy izzószál kapcsolót indít el.
