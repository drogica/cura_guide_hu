# WP Flow

Ezzel a beállítással az áramlási sebesség állítható a Wire Printing technikával történő nyomtatás közben. Ez egyszerűen a vonalszélesség és a rétegmagasság szorzójaként szolgál. Közvetlenül meghatározza, hogy mennyi anyagot használnak fel a drótnyomtatáshoz.

Ez a beállítás a teljes nyomat áramlását állítja be, de a [vízszintes részeknél](wireframe_flow_flat.md) vagy a [csatlakozásoknál](wireframe_flow_connection.md) külön is beállítható az áramlás.

A vezetékes nyomtatás nem használja a vonalszélességet vagy a rétegmagasságot a vonalak és rétegek közötti távolság meghatározására. Csak a [magasságot](wireframe_height.md) és [a beillesztési távolságot](wireframe_roof_inset.md) használja. Tehát a vezetékes nyomtatás menetének beállítása helyett módosíthatja a [Rétegmagasság](../resolution/layer_height.md) vagy [a Vonalszélesség](../resolution/line_width.md) beállításokat, vagy a [szokásos Flow értéket](../material/material_flow.md) . Ennek ugyanaz lesz a hatása. Ezek a beállítások azonban azért léteznek, hogy olyan nyomtatási profilt lehessen létrehozni, amely megfelelő áramlást biztosít a vezetékes nyomtatáshoz anélkül, hogy befolyásolná a vezetékes nyomtatást nem használó normál nyomatok nyomtatási minőségét.

Az áramlás növelése vastagabbá teszi a vezetékeket. Ez merevebbé teszi a keretet, miután megszilárdult. Ugyanakkor növeli a keret hőtömegét is, így tovább tart a vezetékek megszilárdulása. Emiatt a vezetékek leereszkednek, és csökken a nyomtatás megbízhatósága, mivel előfordulhat, hogy ekkor már nem csatlakoznak megfelelően a vezetékek.
