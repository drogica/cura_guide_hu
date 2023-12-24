# Törlés visszahúzás engedélyezése

Ha ez a beállítás engedélyezve van, az anyag a törlési folyamat során visszahúzódik. Ez a [normál visszahúzásoktól](../travel/retraction_enable.md) függetlenül konfigurálható.

A törlési eljárás során a fúvóka egészen a nyomtató oldaláig húzódik, oda-vissza mozog, majd egészen vissza. Ez lényegében egy nagyon hosszú utazási lépés. Mivel ez az elmozdulás hosszabb, mint az átlagos utazási mozgások a nyomtatás során, érdemes lehet az anyagot visszahúzni az eljárás során, még akkor is, ha a visszahúzás általában le van tiltva.

Az anyag visszahúzása csökkenti a törlési eljárás során kiszivárgó anyag mennyiségét. A törlési eljárás során kiszivárgott anyagot általában a kefe letörli. Ez az anyag azonban ekkor elveszik. Ennek eredményeként a törlés befejezése után némi alulextrudálás következik be, mivel ez az anyag kiszivárgott ahelyett, hogy a megfelelő helyre került volna.

Másrészt a visszahúzás eltarthat egy ideig, és szükségtelen kopást okozhat az izzószálon. Ha az alulextrudálás nem jelent problémát, a visszahúzás letiltása időt takaríthat meg és javíthatja a megbízhatóságot. Ez jól működhet, ha például a [kitöltést a falak elé nyomtatják](../infill/infill_before_walls.md) , mert a kitöltés során az alulextrudálás nem igazán jelent problémát.
