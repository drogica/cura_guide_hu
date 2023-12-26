# X végállomás pozitív irányban

Ez a beállítás megmondja Curának, hogy a nyomtató milyen irányban mozog az X tengely mentén, amikor hazarendeli. Ha ez a beállítás le van tiltva, akkor azt feltételezi, hogy az X tengely végpontja a felépítési térfogat nulla (vagy negatív) koordinátáján van. Ha a beállítás engedélyezve van, akkor azt feltételezi, hogy az X tengely végpontja a nyomtató maximális X koordinátáján van. Amikor a nyomtató hazakerül, e végpontok felé kell haladnia, hogy a nyomtató tudja, hol van a nyomtatófej.

Ezt a beállítást a Cura egyáltalán nem használja. Az X3GWriter beépülő modul azonban használja a homing g-code parancs megfelelő végrehajtásához X3G eszköz elérési út fájl írásakor.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
