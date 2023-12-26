# Y Végállomás pozitív irányban

Ez a beállítás közli a Cura-val, hogy a nyomtató az Y tengely mentén milyen irányba mozog, amikor hazarendeli. Ha ez a beállítás le van tiltva, akkor azt feltételezi, hogy az Y tengely végpontja a felépítési térfogat nulla (vagy negatív) koordinátáján van. Ha a beállítás engedélyezve van, akkor azt feltételezi, hogy az Y tengely végpontja a nyomtató maximális Y koordinátáján van. Amikor a nyomtató hazakerül, e végpontok felé kell haladnia, hogy a nyomtató tudja, hol van a nyomtatófej.

Ezt a beállítást a Cura egyáltalán nem használja. Az X3GWriter beépülő modul azonban használja a homing g-code parancs megfelelő végrehajtásához X3G eszköz elérési út fájl írásakor.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
