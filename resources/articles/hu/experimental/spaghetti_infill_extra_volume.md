# Spagetti töltet extra térfogat

Ezzel a beállítással extra mennyiségű anyagot extrudál minden alkalommal, amikor kitöltés nyomtat. Ez minden lépésben megtörténik, ha a spagettibetétet [lépésekben](spaghetti_infill_stepped.md) nyomtatja ki, vagy különben a kitöltés függőleges oszlopánként egyszer.

Ha öntéshez spagetti tölteléket használunk, ez lehetővé teszi egy [idom](https://en.wikipedia.org/wiki/Sprue_(manufacturing)) anyaggal való feltöltését vagy az indító-leállító mechanizmus miatti veszteségek kompenzálását.

Ha a spagetti tölteléket lágy töltetszerkezetek létrehozására használjuk, ez lehetővé teszi az alulextrudálás kompenzálását a hirtelen áramlási sebesség nagyobb áramlási sebességre történő változása miatt. Nincs azonban olyan mechanizmus, amely kompenzálja az áramlási sebesség hirtelen csökkenését a kitöltés nyomtatása után, így továbbra is foltok maradnak a nyomtatott anyagokon.
