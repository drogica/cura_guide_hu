# Spagetti töltelék

Ha ez a beállítás engedélyezve van, a Cura több réteg minden kitöltését egyszerre kinyomja egy magasabb rétegbe. Ez [a kitöltési rétegvastagság](../infill/infill_sparse_thickness.md) extrém formájaként szolgál, de a kitöltés merevségének megőrzése nélkül. Van egy kis funkcionalitása a szélsőséges mennyiségű extrudálás kezelésére.

Ez a funkció nem működik közönséges anyagoknál. Általában vagy a közönséges kitöltési minták erősségét szeretné elérni, vagy teljesen elhagyja a kitöltést. Ennek ellenére két felhasználási esete van.

## Használati esetek

Rugalmas anyagokkal ez a technika nagyon puha textúrákat hozhat létre. A spagettibetét általában lazán elhelyezett gyűrűket hoz létre, amelyek nem tapadnak jól egymáshoz. Ezek a gyűrűk minden irányban egyformán simaak. Ennek a hatásnak az eléréséhez azonban a kitöltési sűrűség nem lehet túl alacsony, különben az összes spagetti a nyomat aljára kerül. A vonalszélességtől és a rétegmagasságtól függően 30% és 60% közötti [áramlási sűrűséget](spaghetti_flow.md) célszerű használni. Az eredmény egy olyan betét lesz, amely minden irányban egyformán merev és meglehetősen puha.

A spagetti töltelék másik alkalmazása az öntés. Ha olyan nyomtatója van, amely tartalmaz egy adott helyekre önthető szerszámot, ez a funkció használható arra, hogy a modellt nagyjából egyenletesen töltse fel ellenőrzött anyaglerakódásokkal. Ha ezt használják, az [áramlási sűrűségnek](spaghetti_flow.md) valószínűleg körülbelül 100%-nak kell lennie, az öntött anyag zsugorodási/tágulási arányától függően.

## A spagetti töltelék egyéb beállításainak módosítása

Mindkét alkalmazás nagyon speciális kezelést igényel a kitöltésnél. Íme néhány beállítás, amelyet valószínűleg az igényeinek megfelelően szeretne módosítani:

- A [kitöltés nyomtatási sebességét](../speed/speed_infill.md) jelentősen csökkenteni kell. Ha a fúvókának egyszerre 10 réteg kitöltését kell extrudálnia, akkor a nyomtatási sebességet legalább 8-szorosára csökkentenie kell.
- Állítsa be [a kitöltőréteg vastagságát](../infill/infill_sparse_thickness.md) a réteg magasságával egyenlőre.
- Növelje kissé a [nyomtatási hőmérsékletet](../material/material_print_temperature.md) (az extruder esetében, amely kinyomtatja a töltetet). Ez lehetővé teszi az anyag megfelelő kiáramlását a fúvókán, és gyorsabb extrudálást tesz lehetővé.
- Állítsa a [varrat igazítását](../shell/z_seam_type.md) véletlenszerűre a szerkezet véletlenszerű szétterítéséhez.

**Cura rétegnézetében a kitöltés nagyon vastag vonalakként fog megjelenni. Ez azért van így, mert Cura azt feltételezi, hogy az anyag ugyanazon a rétegen marad, és ott szétterül. A valóságban le fog esni.**

**Amíg a spagetti kitöltés használatban van, a [kitöltési vonalszélesség](../resolution/infill_line_width.md) beállításának nincs hatása. A vonal szélessége úgy van beállítva, hogy megfeleljen a [kitöltővonal távolságának](../infill/infill_line_distance.md) és [a spagetti áramlási](spaghetti_flow.md) beállításainak.**
