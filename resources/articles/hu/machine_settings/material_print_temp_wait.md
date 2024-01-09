# Várja meg a fúvóka felmelegedését

A kezdeti réteg [fúvóka hőmérséklete](../material/material_print_temperature_layer_0.md) eltérhet a [nyomat többi részének fúvóka hőmérsékletétől](../material/material_print_temperature.md) . Ha ez a beállítás engedélyezve van, a nyomtató megvárja, amíg eléri ezt a hőmérsékletet, mielőtt folytatná a nyomtatást.

Megvárja, amíg a hőmérséklet felmelegszik vagy lehűl a megfelelő hőmérsékletre. Noha ennek a beállításnak a címkéje azt írja, hogy megvárja a felmelegedést, ugyanúgy le fog hűlni. A fúvóka nem várja meg az egyéb hőmérséklet-változásokat, például a [kezdeti nyomtatási hőmérsékletet](../material/material_initial_print_temperature.md) , a [végső nyomtatási hőmérsékletet](../material/material_final_print_temperature.md) vagy a [készenléti hőmérsékletet](../material/material_standby_temperature.md) . [Egyenkénti módban történő](../blackmagic/print_sequence.md) nyomtatás esetén a fúvóka is megvárja a kezdeti réteghőmérséklet elérését, amikor vissza kell térnie az első réteghez a következő objektumokhoz.

**Mivel ez egy gépbeállítás, ez a beállítás általában nem látható a beállítások listájában.**
