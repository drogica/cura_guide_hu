# Központi eredetű

Ha ez a beállítás engedélyezve van, a nyomtató 0,0 koordinátája az összeállítási kötet közepére van beállítva, nem pedig a bal első sarokba.

Egyes nyomtatókban a firmware a 0,0 koordinátát a build kötet közepének tekinti. Ez gyakori a delta-stílusú nyomtatóknál, amelyek általában hengeres felépítésűek, nem téglatestek.

Ha a nyomtató nulla koordinátája a közepén van, akkor a végső g-kód negatív és pozitív koordinátákat is tartalmaz. A koordináta kezdőpontja Cura build kötetének közepén lesz. Cura középen is megmutatja a háromszínű koordináta jelölőjét. A 3MF fájlok koordinátái azonban továbbra is úgy lesznek kezelve, mintha a koordináta origója a nyomtató bal első sarkában lenne, mivel a 3MF fájlformátum ezt megköveteli.

**Mivel ez egy gépbeállítás, általában nem szerepel a normál beállítások listájában. Ehhez a beállításhoz van egy jelölőnégyzet a nyomtatóbeállítások párbeszédpanelen, amely a hozzáadott nyomtatók listájában található a beállítások párbeszédablakban.**
